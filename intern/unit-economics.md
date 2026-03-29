# dGENIX — Unit Economics & Winstberekening

> Intern document — niet publiek. Gebaseerd op Anthropic API prijzen (april 2026).

---

## 1. Fundament — Wat kost 1 credit?

**1 credit = $0,0002 (0,02 cent)**
→ 5.000 credits per dollar

### Anthropic API prijzen (per 1 miljoen tokens)

| Model | Input | Output |
|---|---|---|
| Haiku 4.5 | $0,80 | $4,00 |
| Sonnet 4.6 | $3,00 | $15,00 |
| Opus 4.6 | $15,00 | $75,00 |

### Creditformule (code: `router.ts → berekenCredits()`)

```
Haiku:  ceil((tokensIn × 4  + tokensUit × 20)  / 1000)
Sonnet: ceil((tokensIn × 15 + tokensUit × 75)  / 1000)
Opus:   ceil((tokensIn × 75 + tokensUit × 375) / 1000)
```

**Verificatie Haiku:**
- 1M tokens input = 1.000.000 × 4 / 1000 = 4.000 credits = $0,80 ✅
- 1M tokens output = 1.000.000 × 20 / 1000 = 20.000 credits = $4,00 ✅

---

## 2. Kosten per interactie (gemiddelde)

**Aannames:**
- Gemiddelde interactie: 800 tokens in + 400 tokens out (inclusief systeemprompt)
- ~85% van gesprekken via Haiku (standaard)
- ~15% via Sonnet (schrijftaken, research)
- Opus: zelden (<1%)

| Model | Credits verbruikt | API kosten ($) | API kosten (€) |
|---|---|---|---|
| Haiku (800in + 400out) | ~11 credits | $0,0022 | ~€0,002 |
| Sonnet (800in + 400out) | ~36 credits | $0,0072 | ~€0,007 |
| Gewogen gemiddeld (85/15) | ~15 credits | $0,0031 | ~€0,003 |

**→ 1 interactie kost gemiddeld ~15 credits en ~€0,003 API-kosten**

---

## 3. Plannen — Margeberekening

**Aanname: 70% kredietbenutting** (gebruiker verbruikt 70% van zijn maandelijkse credits)

| Plan | Prijs | Credits | Gebruikt (70%) | API kost @70% | Bruto marge |
|---|---|---|---|---|---|
| Starter | €19 | 55.000 | 38.500 | ~€0,12/credit × 38.500/5000 = **€6,85** | **€12,15 → 64%** |
| Growth | €39 | 120.000 | 84.000 | **€14,94** | **€24,06 → 62%** |
| Pro | €79 | 240.000 | 168.000 | **€29,88** | **€49,12 → 62%** |

> API kosten berekening: credits × $0,0002 × wisselkoers (€1 = $1,10)
> 38.500 credits × $0,0002 / 1,10 = **€7,00** (iets hoger bij 100% bezetting)

### Bij 100% kredietbenutting (worst case)

| Plan | Prijs | API kost | Marge |
|---|---|---|---|
| Starter | €19 | ~€9,78 | **€9,22 → 49%** |
| Growth | €39 | ~€21,36 | **€17,64 → 45%** |
| Pro | €79 | ~€42,73 | **€36,27 → 46%** |

---

## 4. Credit Packs — Margeberekening

| Pack | Credits | Prijs | API kost (100%) | Marge |
|---|---|---|---|---|
| Small | 15.000 | €7 | ~€2,64 | **€4,36 → 62%** |
| Medium | 40.000 | €18 | ~€7,04 | **€10,96 → 61%** |
| Large | 100.000 | €45 | ~€17,60 | **€27,40 → 61%** |

> Packs worden bij 100% benut (anders kopen mensen ze niet) — marge is bewust gezet op ~61%.

---

## 5. Vaste kosten (maandelijks)

| Post | Kosten/mnd |
|---|---|
| VPS Hostinger (agent + n8n) | ~€15 |
| Vercel Pro | ~€20 |
| Supabase Pro | ~€25 |
| Nango (OAuth proxy) | ~€0–€50 (afhankelijk van tier) |
| Stripe fees (2,9% + €0,25/transactie) | variabel |
| Domein + misc | ~€5 |
| **Totaal vaste infra** | **~€65–€115/mnd** |

---

## 6. Winst geselecteerd naar gebruikersaantal

**Aannames:**
- Mix: 60% Starter / 30% Growth / 10% Pro
- Kredietbenutting: 70%
- Vaste kosten: €90/mnd (midden)
- Stripe fees: 3% van omzet

### Formule per gebruiker (gewogen gemiddeld)

```
Gem. omzet/user   = 0,60 × €19 + 0,30 × €39 + 0,10 × €79 = €11,40 + €11,70 + €7,90 = €31,00
Gem. API kost     = 0,60 × €6,85 + 0,30 × €14,94 + 0,10 × €29,88 = €4,11 + €4,48 + €2,99 = €11,58
Stripe (3%)       = €31,00 × 0,03 = €0,93
Bruto per user    = €31,00 - €11,58 - €0,93 = €18,49
```

### Netto winst per maand (na vaste kosten)

| Gebruikers | Omzet | API kost | Stripe | Vaste kosten | **Netto winst** | **Netto marge** |
|---|---|---|---|---|---|---|
| 10 | €310 | €116 | €9 | €90 | **€95** | **31%** |
| 25 | €775 | €290 | €23 | €90 | **€372** | **48%** |
| 50 | €1.550 | €579 | €47 | €90 | **€834** | **54%** |
| 100 | €3.100 | €1.158 | €93 | €90 | **€1.759** | **57%** |
| 250 | €7.750 | €2.895 | €233 | €90 | **€4.532** | **58%** |
| 500 | €15.500 | €5.790 | €465 | €90 | **€9.155** | **59%** |
| 1.000 | €31.000 | €11.580 | €930 | €90 | **€18.400** | **59%** |

> Netto marge stabiliseert boven ~50 users omdat vaste kosten een steeds kleiner deel worden.

---

## 7. Break-even analyse

**Break-even = vaste kosten / bruto marge per user**

```
Break-even = €90 / €18,49 ≈ 5 betalende gebruikers
```

Vanaf 5 gebruikers dekt dGENIX de infrastructuurkosten. Elke gebruiker daarna is nettoprofit.

---

## 8. Doelstelling — 60% marge halen

### Wanneer halen we 60%+ netto marge?

Boven ~100 betalende gebruikers stabiliseert de netto marge op ~57–59%. Met de juiste plan-mix (meer Growth/Pro) is 60%+ haalbaar.

**Scenario: 100 users, mix verschuift naar 40% Starter / 40% Growth / 20% Pro:**

```
Gem. omzet/user   = 0,40 × €19 + 0,40 × €39 + 0,20 × €79 = €7,60 + €15,60 + €15,80 = €39,00
Gem. API kost     = 0,40 × €6,85 + 0,40 × €14,94 + 0,20 × €29,88 = €2,74 + €5,98 + €5,98 = €14,70
Stripe (3%)       = €39,00 × 0,03 = €1,17
Bruto per user    = €39,00 - €14,70 - €1,17 = €23,13

Netto (100 users) = €2.313 - €90 = €2.223 → marge 57%
```

> Add-on skills verhogen de marge verder zonder extra API-kosten voor eenvoudige taken.

---

## 9. Risico's & buffers

| Risico | Impact | Mitigatie |
|---|---|---|
| 100% kredietbenutting | Marge daalt naar ~45% | Acceptabel — users bijkopen dan credits (extra marge) |
| Sonnet gebruik stijgt boven 30% | API kosten stijgen ~2× | Monitor via taaklog — eventueel Sonnet-taken duurder maken |
| Wisselkoers USD/EUR verslechtert | Hogere API kosten | Build in bij volgende prijsronde |
| Gebruikersstop vroegtijdig | Lager dan 70% benutting | Marge stijgt juist — voordeel voor dGENIX |

---

*dGENIX — Intern | Unit Economics v1.0 — april 2026*
