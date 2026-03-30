# dGENIX — Unit Economics & Winstberekening

> Intern document — niet publiek. Gebaseerd op Anthropic API prijzen + 3x credit markup (april 2026).

---

## 1. Fundament — Creditmodel

**1 credit = $0,0002 (break-even basis)**
→ 5.000 credits per dollar API-kosten

**CREDIT_MARKUP = 3x**
User spendeert 3× meer credits per token dan de werkelijke API-kosten.
→ API-kosten = 33% van credit-waarde bij 100% gebruik
→ Plan-marge afhankelijk van benutting: lagere benutting = hogere marge

Marktbenchmark: Bessemer State of AI 2025 — gezonde AI SaaS heeft API-kosten < 15% van revenue.

---

## 2. Anthropic API prijzen (per 1 miljoen tokens)

| Model | Input | Output | Credit-factor input | Credit-factor output |
|---|---|---|---|---|
| Haiku 4.5 | $0,80 | $4,00 | ×12 / 1000 tokens | ×60 / 1000 tokens |
| Sonnet 4.6 | $3,00 | $15,00 | ×45 / 1000 tokens | ×225 / 1000 tokens |
| Opus 4.6 | $15,00 | $75,00 | ×225 / 1000 tokens | ×1.125 / 1000 tokens |

> Credit-factor = (prijs_per_mtoken × 5 / 1000) × 3 (markup)

**Verificatie Haiku met markup:**
- 1M tokens input → 4.000 credits (break-even) × 3 = **12.000 credits**
- API-kosten: $0,80 → credit-waarde: 12.000 × $0,0002 = $2,40 → markup: **3x** ✅

---

## 3. Kosten per interactie (gemiddeld bericht)

**Aannames:**
- Gemiddelde interactie: 800 tokens in + 400 tokens uit (incl. systeemprompt fragment)
- **~30% Haiku / ~70% Sonnet** (realistisch — assistent voert continu taken uit)

| Model | Credits verbruikt | API kosten ($) | API kosten (€) |
|---|---|---|---|
| Haiku (800in + 400out) | **34 credits** | $0,0022 | ~€0,002 |
| Sonnet (800in + 400out) | **126 credits** | $0,0084 | ~€0,008 |
| Gewogen gemiddeld (30/70) | **~98 credits** | $0,0065 | ~€0,006 |

**→ 1 bericht kost de user gemiddeld ~98 credits en kost ons ~€0,006 aan API**

---

## 4. Plannen — Margeberekening

### Bij 70% kredietbenutting (realistisch)

| Plan | Prijs | Credits | Gebruikt (70%) | API-kosten | Stripe (~3%) | **Bruto marge** |
|---|---|---|---|---|---|---|
| Starter | €19 | 88.000 | 61.600 | ~€3,73 | €0,57 | **€14,70 → ~77%** |
| Growth | €39 | 212.000 | 148.400 | ~€9,00 | €1,17 | **€28,83 → ~74%** |
| Pro | €79 | 495.000 | 346.500 | ~€21,00 | €2,37 | **€55,63 → ~70%** |

> API-kosten: credits_gebruikt / 3 × $0,0002 / 1,10 (EUR/USD koers)

### Bij 100% kredietbenutting (worst case)

| Plan | Prijs | Credits | API-kosten | Stripe (~3%) | **Netto marge** |
|---|---|---|---|---|---|
| Starter | €19 | 88.000 | ~€5,33 | €0,57 | **€13,10 → 69%** |
| Growth | €39 | 212.000 | ~€12,85 | €1,17 | **€24,98 → 64%** |
| Pro | €79 | 495.000 | ~€30,00 | €2,37 | **€46,63 → 59%** |

> API-kosten: 88.000 / 3 × $0,0002 / 1,10 = **€5,33** (Starter voorbeeld)

**→ Worst-case marge (100% gebruik): 69% / 64% / 59% (Starter / Growth / Pro)**
**→ Realistisch (70% gebruik): 77% / 74% / 70%**
**→ In de praktijk gebruikt niemand alle credits volledig op.**

---

## 5. Credit Packs — Margeberekening

| Pack | Credits | Prijs | API-kosten (100%) | Stripe | **Netto marge** |
|---|---|---|---|---|---|
| Small | 25.000 | €9 ex BTW | ~€1,52 | €0,27 | **€7,21 → ~80%** |
| Medium | 60.000 | €20 ex BTW | ~€3,64 | €0,60 | **€15,76 → ~79%** |
| Large | 150.000 | €45 ex BTW | ~€9,09 | €1,35 | **€34,56 → ~77%** |

> Packs worden bij 100% benut — marge consistent met abonnementsmodel.

---

## 6. Vaste kosten (maandelijks)

| Post | Kosten/mnd |
|---|---|
| VPS Hostinger (agent + n8n) | ~€15 |
| Vercel Pro | ~€20 |
| Supabase Pro | ~€25 |
| Nango (OAuth proxy) | ~€0–€50 |
| Stripe fees | variabel (~3% omzet) |
| Domein + misc | ~€5 |
| **Totaal vaste infra** | **~€65–€115/mnd** |

---

## 7. Netto winst naar gebruikersaantal

**Mix:** 60% Starter / 30% Growth / 10% Pro | **Gebruik:** 70% | **Vaste kosten:** €90/mnd

```
Gem. omzet/user   = 0,60×€19 + 0,30×€39 + 0,10×€79 = €31,00
Gem. API/user     = 0,60×€3,73 + 0,30×€9,00 + 0,10×€21,00 = €7,04
Stripe (3%)       = €0,93
Netto/user        = €31,00 - €7,04 - €0,93 = €23,03
```

| Gebruikers | Omzet | API | Stripe | Vaste kosten | **Netto winst** | **Marge** |
|---|---|---|---|---|---|---|
| 10 | €310 | €70 | €9 | €90 | **€141** | **45%** |
| 25 | €775 | €176 | €23 | €90 | **€486** | **63%** |
| 50 | €1.550 | €352 | €47 | €90 | **€1.061** | **68%** |
| 100 | €3.100 | €704 | €93 | €90 | **€2.213** | **71%** |
| 250 | €7.750 | €1.760 | €233 | €90 | **€5.667** | **73%** |
| 500 | €15.500 | €3.520 | €465 | €90 | **€11.425** | **74%** |
| 1.000 | €31.000 | €7.040 | €930 | €90 | **€22.940** | **74%** |

---

## 8. Break-even

```
Break-even = €90 / €23,03 ≈ 4 betalende gebruikers
```

Vanaf **4 gebruikers** is dGENIX winstgevend.

---

## 9. Risico's

| Risico | Impact | Mitigatie |
|---|---|---|
| 100% kredietbenutting | Marge daalt naar 59–69% | Zware users kopen packs bij (packs hebben 77-80% marge). |
| Sonnet-gebruik >70% | API-kosten hoger | Monitor via `usage_logs`. Eventueel markup naar 4x. |
| USD/EUR verslechtert | Hogere API-kosten in euro | Redelijke buffer in 3x markup. Bij >15% verslechtering: markup naar 4x. |
| Anthropic prijswijziging | Directe impact op marge | `CREDIT_MARKUP` in `router.ts` aanpassen + `berekenCredits` bijwerken. |

---

*dGENIX — Intern | Unit Economics v4.0 — april 2026 | CREDIT_MARKUP = 3 | Mix: 30% Haiku / 70% Sonnet*
