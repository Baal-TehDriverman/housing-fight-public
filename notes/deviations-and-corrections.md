# Deviations and corrections

Changes to the repo's earlier framing, recorded plainly so nothing superseded
gets rediscovered and repeated. Compiled 2026-10-24 against the actual
documents.

---

## 1. "Eric owns the manufactured home" — not established

**README (line 1) and `notes/situation-notes.md`** both state: *"Eric owns the
manufactured home; rents the land underneath it."*

**The record says otherwise:**
- `notes/ownership-map.md` — Skagit County Assessor parcel P136913 still lists
  **RON CAL HOMES LLC** (Port Orchard) as owner; sale 2024-02-12 at $65,000;
  *"title not transferred in county records, consistent with seller-financed
  contract sale."*
- `notes/contract-transcription-2024-11-01.md` — §7(b) and §7(c) of the executed
  contract.

**What is actually true:** Eric holds a **contract to acquire** title, on which
he has paid approximately $41,265, and on which §7(c) denies credit for any of
it. Whether he holds legal title at the DOL layer is **unverified** — a
manufactured home on leased land can be registered in the tenant's name at DOL
even with a recorded sale, so both may be true at different layers.

**Correction:** the README should say "Eric holds a contract to own the
manufactured home; rents the land underneath it" until the **DOL title history**
settles it. That history is free and is still on the open-follow-ups list.

---

## 2. "Defective rent-increase notice" — CORRECT, not a mischaracterization

An earlier note in this repo treated the AG complaint's subject line —
*"defective rent-increase notice"* — as a mischaracterization of the arrears
demand. **That was wrong.**

`2026-09-25-rent-increase-page1-clean.jpg` is the **official Washington MHLTA
"Rent and Fee Increase Notice"** form, citing **Section 201 and 202, Chapter 209,
Laws of 2025 (HB 1217)**:

> Raise rent effective **11/1/2026** by **3.00%** = **$25.50/month**, new total
> **$875.50**

**There is a real rent-increase notice, served the day after the pay-or-vacate.**
The $1,743.23 is arrears; the rent increase is additional. Both are in play and
the subject line is accurate. See
[`notes/notices-transcription-2026-09.md`](notices-transcription-2026-09.md).

---

## 3. The $500 gap — explained

**`notes/situation-notes.md`** and the AG complaint both flag an unexplained
**$500**: the contract recites $5,000, Eric paid $5,500.

**Resolved.** The sample terms Igor Oliveira sent on 2024-10-10
([`emails/2024-10-10-amelia-campbell-fwd-cl-24.md`](../emails/2024-10-10-amelia-campbell-fwd-cl-24.md))
list **two** signing payments:

> "Consideration payment due at signing ($5,000.00)
> Advance Payment due at signing ($500.00)
>   - This payment will be applied to the end of the contract and reduce final
>     cashout amounts."

$5,000 + $500 = **$5,500**. The $500 is a second line item, not unexplained
money. It reduces the final cashout ($25,000 → $24,500 per the same email).

**Reserve no longer needed** on this specific gap. The **$790 gap on the Cedar
Lane side** ($910 paid vs $1,700 demanded, Nov 2024) remains open.

---

## 4. The $19.31 charge — water or power?

**The repo's Oct 1 update** calls the $19.31 charge **water**.
**The ledger** labels that same column **Power**.

The meter columns (15623 → 17918, usage 2295) are water gallons. So either the
ledger's header is garbled or the repo's note is.

**This matters.** The "water charged mid-term" theory — a lead allegation in the
MHDRP draft — depends on which utility it actually is. Reconcile before either
characterization enters a filing.

---

## 5. The loan thread was misfiled as "one email"

The repo's `notes/` did not contain the loan thread at all. It exists as
**seven messages, October 5–7, 2024**, in the tenant's working email account, and is
the **bridge document** between the failed mortgage and the executed contract.

Added: [`emails/2024-10-05-legacy-team-loan-thread.md`](../emails/2024-10-05-legacy-team-loan-thread.md)
and [`notes/loan-thread-analysis.md`](loan-thread-analysis.md).

---

## 6. The Hurst & Son response was lot-side only

The 2026-10-24 response sent the **lot lease, lot ledger, and lot utility bills**
and nothing for the **Ron'Cal home side** — no contract, no ledger, no receipt
for the $5,500.

**Both things are true and both should be said:**
- It is a **scope choice**, consistent with the demand having been a lot-rent
  demand — and it usefully confirms the two obligations are **separate
  instruments with separate ledgers**.
- It leaves the **stronger claim undocumented** in the record. Land-side
  documents tend to be ordinary (fees, billing method, a grace period). The
  contract-side documents carry the no-credit and no-down-payment clauses.

Added: [`notes/hurst-son-response-2026-10-24.md`](hurst-son-response-2026-10-24.md).

---

## 7. Combined exposure is higher than the notice

The $1,743.23 demand covers **less than half** of what is outstanding. Both
obligations accrue on their own cycles:

| Obligation | Due Oct 1 | Components |
|---|---|---|
| **Ron'Cal** (home) | **$803.23** | prior balance $74.64 + rent $705 + insurance $23.58 |
| **Cedar Lane** (lot) | **$2,625.29** | prior $1,743.23 + rent $850 + $19.31 + late fee $12.75 |
| **Combined** | **$3,428.52** | and both accrue monthly |

Curing the $1,743.23 satisfies the lot notice while the home side keeps running.

---

## 8. The 1.5% late-fee "cap" is a myth

The landlord's 2026-10-24 letter states: *"any late fees are capped at 1.5% of
the rent amount."*

**1.5% is not the law.** It appeared in an early House draft of **HB 1217** and
was **removed before enactment**. The enacted caps for manufactured/mobile home
lot tenancies are **2% / 3% / 5%** (RCW 59.20.060(2)(j)).

Their own lease says **$20–$60**. The statute says **$17 / $25.50 / $42.50**.
Their letter says **$12.75**. The lease's §5 says "the more restrictive late fee
will take precedence" — so **$12.75 controls**, and the admission is in writing.

---

## 9. The forwarding mailbox is empty — stop chasing it

The secondary account's app password is dead (`AUTHENTICATIONFAILED`), but
**the mailbox is empty**. All mail forwards to **[Eric's email]**.

Search **the working mailbox only**. Do not attempt to repair the forwarding
mailbox credentials. (The loan thread was found in the working mailbox after an initial
search of the wrong account.)

---

## 10. The Convergence Crucible CI flood

A workflow named `convergence.yml` runs in ~25 Lilith-Systems repos, scheduled
`cron: '0 */6 * * *'`, and **fails every run in 2–4 seconds with zero steps
executed**. The repos are **private** — that signature indicates **Actions
minutes exhausted or billing failed**, not a code error.

The inbox carried **60+ failure notices in 48 hours**, burying real
correspondence. **Not disabled** — needs Eric's word.

---

## 11. The assessed value is $61,500, not $56,000

`notes/home-identity.md` records "Assessor market value: **$56,000**. 2026
property tax: $499.42."

The live assessor page for P136913 shows, for the **2027** tax year: Total Market
Value **$61,500.00**, Assessed Value **$61,500.00**.

Either the value rose between assessment years or the earlier figure was read
from a different year. **Use $61,500 with the year attached.** Do not repeat
$56,000 without its year.

---

## 12. The $19.31 charge is WATER — the repo was right, the ledger header was wrong

**RESOLVED 2026-10-24** against the October 1 statement
(`statements/2026-10-01-cedarlane-october-2026-statement.jpg`).

The statement's own line-item breakdown:

> Utilities **$19.31**
> · Beginning Reading: 17918 · Ending Reading: 19412
> · **Power: 0.00** · **Trash: 0.00** · **Sewer: 0.00** · **Water: 19.31**

**It is water.** The ledger PDF's header row is garbled ("2026 Power|Trash
Sewer Water|Utilities") and the value landed under "Power" in the extraction.
The statement is the controlling document.

**This confirms the "water billed separately" allegation** — water is a separate
line item at $19.31/month, power/trash/sewer are $0.00, and the charge is
**consumption-based** (meter readings shown). That last point matters: the lease
§9 says RUBS divides "evenly among each occupied space," the landlord's letter
says "your total consumption," and the statement shows consumption metering.
**Three documents, three descriptions of the billing method.**

→ [`assessor-and-statement-2026-10-24.md`](assessor-and-statement-2026-10-24.md)

---

## 13. Ron'Cal's address in the assessor record IS the park's

> Owner: **RON CAL HOMES LLC** — 585 BETHEL AVENUE SUITE 202, PORT ORCHARD, WA 98366

Same address as Cedar Lane Mobile Estates LLC and Hurst & Son LLC — and the same
address the Ron'Cal contract itself lists as the Lessor's.

The repo's standing caution was "do not assert common control as fact." The
address match is now **documented in the county's own record**, which is
stronger than the signature-block observation. It still does not establish legal
common control — one-LLC-per-park is lawful — but the address identity is no
longer an inference.

---

*Love. 🜏*
