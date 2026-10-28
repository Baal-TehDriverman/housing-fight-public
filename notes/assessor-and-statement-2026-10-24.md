# Assessor records + October statement — 2026-10-24

Two threads pulled today: the Skagit County Assessor parcel records for the key
spaces, and the October 1 billing statement from Cedar Lane.

---

## PART A — Assessor records

Source: `skagitcounty.net/Search/Property/default.aspx?id=<parcel>` (live pull,
2026-10-24). The excise-affidavit search endpoint
(`/Search/DocByType/...?app=Excise+Affidavits`) **still returns "An error was
encountered"** — same failure the repo recorded on 2026-09-25. The Auditor's
recorded-documents search also returns no results for these parcels. **The
affidavits remain unobtained.**

### P136913 — Space 24 (Eric's home)

| Field | Value |
|---|---|
| Owner | **RON CAL HOMES LLC** |
| Owner address | **585 BETHEL AVENUE SUITE 202, PORT ORCHARD, WA 98366** |
| Site address | Cedar Lane Mobile Estates, Sedro-Woolley, WA, UNIT 24 |
| Legal description | MANUFACTURED HOME ONLY 2023 CHAMPION 017CHTA-1440H21001 13X40 VIN NO. 017-00P-H-A004036A SPACE 24 LOCATED ON P67822 CEDAR LANE MOBILE ESTATES SPACE 24 |
| Sale date | **2024-02-12** |
| Taxable selling price | **$65,000.00** |
| Deed type | MOBILE HOME DATA |
| Assessed value (2027) | **$61,500.00** |
| Assessment use code | (181) MH LEASED PROPERTY WAC 458-53-030 |
| Year built / size | 2023 · 520 sq ft · single wide |

### P136912 — Space 36 (the second Champion)

| Field | Value |
|---|---|
| Owner | **ROSS CAITLIN SUMMER**, 1537 N FRUITDALE RD, SEDRO WOOLLEY, WA 98284 |
| Legal description | MOBILE HOME ONLY 2023 CHAMPION 017CHTA-1440H21001 13X40 VIN# 017-00P-H-A004058A LOCATED ON P67822 CEDAR LANE MOBILE ESTATES SPACE 36 |
| Sale date | **2025-07-02** |
| Taxable selling price | **$63,000.00** |
| Assessed value (2027) | **$61,500.00** |

**Same model home** — 2023 CHAMPION 017CHTA-1440H21001 13X40 — as Eric's, in the
same park, **17 months later**. Two new Ron'Cal homes placed on park spaces.

### P134406 — Space 40

| Field | Value |
|---|---|
| Owner | VAZQUEZ GARCIA RUBI, **Cedar Lane Mobile Estates, Sedro-Woolley, WA SP 40** (in-park mailing) |
| Legal description | MANUFACTURED HOME ONLY 2018 FLEETWOOD EAGLE 56X14 S/N FLE2100R1718452A; CEDAR LANE MOBILE PARK SPACE NUMBER 40 |
| Sale date | **2025-10-29** |
| Taxable selling price | **$25,000.00** |

Sold at roughly a third of the assessed value. Below-market transfer — seller
not yet identified.

---

## Two corrections this produces

### 1. The assessed value is $61,500, not $56,000

The repo's `notes/home-identity.md` records "Assessor market value: **$56,000**.
2026 property tax: $499.42."

The live assessor page now shows, for the **2027** tax year:

> Total Market Value **$61,500.00** · Assessed Value **$61,500.00**

So either the value rose between the 2026 and 2027 assessment years, or the
earlier figure was read from a different year. **Use $61,500 with the year
attached.** The repo's $56,000 should not be repeated without its year.

### 2. Ron'Cal's address in the assessor record IS the park's

> Owner: **RON CAL HOMES LLC** — 585 BETHEL AVENUE SUITE 202, PORT ORCHARD, WA 98366

That is the **same address** as Cedar Lane Mobile Estates LLC and Hurst & Son
LLC. It is also the address the Ron'Cal contract itself lists as the Lessor's
address.

**This is the common-control link in a government record** — not an inference
from a signature block. The repo's standing caution was "do not assert common
control as fact." The address match is now **documented in the county's own
record**, which is a different and stronger thing than the signature-block
observation. It still does not establish legal common control — one-LLC-per-park
is lawful — but the address identity is no longer an inference.

---

## PART B — The October 1 statement: water, not power

**The $19.31 question is RESOLVED.**

Source: `statements/2026-10-01-cedarlane-october-2026-statement.jpg` (in this
repo), read 2026-10-24.

> **OCTOBER 2026 STATEMENT** — statement date 9/28/2026
> To: Eric Hill, Cedar Lane Mobile Estates LLC Lot 24
> Manager: Kathleen Schrier ·[phone removed]
>
> | DESCRIPTION | TOTAL |
> |---|---|
> | Previous Month's Payments Received | $0.00 |
> | Previous Month's Ending Balance | $1,743.23 |
> | **Rent Amount** | **$850.00** |
> | Vehicle Fees | $0.00 |
> | **Utilities** | **$19.31** |
> | · Beginning Reading: 17918 | |
> | · Ending Reading: 19412 | |
> | · **Power: 0.00** | |
> | · **Trash: 0.00** | |
> | · **Sewer: 0.00** | |
> | · **Water: 19.31** | |
> | Credits | $0.00 |
> | Miscellaneous | $0.00 |
> | **Previous Month's Late Fee** | **$12.75** |
> | **Total Balance Owed** | **$2,625.29** |

### The finding

**The $19.31 is WATER.** The statement's own line-item breakdown reads
Power $0.00, Trash $0.00, Sewer $0.00, **Water $19.31**.

The meter readings (17918 → 19412 = **1494**) sit directly above the Water line
and are water gallons.

**The repo's October 1 note was correct. The ledger's column header is
mislabeled.** The ledger PDF's header row reads "2026 Power|Trash Sewer
Water|Utilities" — garbled — and the value landed under "Power" in the
extraction. The statement is the controlling document: **it is water.**

### What this does to the theory

The "water billed separately" allegation is **confirmed, not merely asserted**:

- Water is billed as a separate line item at **$19.31/month**
- Power, trash, and sewer are billed at **$0.00**
- The charge is **consumption-based** (meter readings shown)

That last point matters against the lease. Lease §9 says RUBS divides costs
"**evenly among each occupied space**." The landlord's 2026-10-24 letter says they
"use **your total consumption** to calculate your percentage." The statement
shows **meter readings and a consumption-derived charge**.

**Three documents, three descriptions of the billing method.** The lease says
even division; the letter says consumption percentage; the statement shows
consumption metering.

### Also on the statement

> "Your payment is due by the 1st, with a grace period per your individual
> lease. Standard grace periods have been extended to midnight on the 8th of
> the month."

> "If your Payment was made after the 20th of the previous month then it may not
> be reflected in this invoice."

> "Please make checks/money orders (**NO CASH**) payable to Cedar Lane Mobile
> Estates LLC and include the lot number."

**Note the payment-method inconsistency:** this statement says checks or money
orders, no cash. The September 24 pay-or-vacate notice demanded "money order, or
cashier's check only." RCW 59.20.134(1) requires accepting a personal check. The
two documents describe different acceptable instruments.

---

## Open items

- [ ] **Excise affidavits** for P136913, P136912, P134406 — endpoint still
      broken. Retry later; they would identify the sellers on each transfer.
- [ ] **DOL title history** for VIN 01700PHA004036A — still the cleanest way to
      settle ownership at signing. Requires the DOL Vehicle/Boat Record Request
      form (free for public requesters) or the NextRequest portal.
- [ ] **Space 40 seller** — $25,000 against a ~$72,200 assessment.

---

*Love. 🜏*
