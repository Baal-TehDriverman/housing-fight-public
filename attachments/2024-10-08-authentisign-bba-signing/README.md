# Authentisign BBA signing sequence — Oct 8–10, 2024

Amelia Campbell (Keller Williams Western Realty, amelia.campbell@kw.com,
[phone removed]) invited Eric Hill ([Eric's email]) to sign a Buyer
Brokerage Agreement via Authentisign (Lone Wolf Technologies). Three messages
form one signing sequence:

1. **2024-10-08_signature-requested-form41.eml** — Oct 8, 2024, 7:09 p.m. PDT
   (Oct 9, 02:09 UTC — the "Oct 9" date in earlier notes was the UTC date).
   Subject: "Your signature is requested: Eric Hill - Form 41 - Buyer
   Brokerage Services Agreement". Gmail ID `1926f098ccf820b3`. No attachments.
2. **2024-10-10_signature-requested-bba.eml** — Oct 10, 2024, 3:06 p.m. PDT.
   Subject: "Your signature is requested: Eric Hill BBA".
   Gmail ID `1927877c84369bab`. No attachments.
3. **2024-10-10_signing-complete-bba.md** — Oct 10, 2024, 10:27 p.m. PDT.
   Subject: "Signing complete: Eric Hill BBA".
   Gmail ID `1927a0bbb7145e75`.

## Signed status: RESOLVED

The earlier "signed status unknown" note is superseded: the Oct 10 completion
email states the signing is complete, and it carried the signed documents:

- **Form 41 - Buyer Brokerage Services Agreement.pdf** (255,286 bytes)
- **2024 KW Buyer Disclosure Packet 81524.pdf** (5,837,048 bytes)

The completion email's download links expired Oct 18, 2024, but the PDFs in
this folder come from Gmail's attachment store, and their byte sizes match
Gmail's attachment inventory exactly.

## Preservation notes

- The two invitation messages are raw `.eml` files pulled via Gmail
  `format=raw` (byte-faithful MIME).
- The completion message's raw fetch failed twice: the connector cannot
  return the 8 MB+ MIME (message plus both PDFs) through its output channel.
  It is preserved here instead as the connector's full-body capture
  (`2024-10-10_signing-complete-bba.md`: headers, attachment inventory, and
  complete body text, body coverage full) plus both attachments byte-exact.
  No content was reconstructed or altered; only the MIME envelope of that
  one message is represented as a capture rather than a raw `.eml`.

Filed to this repo Oct 28, 2026, at Eric's direction. Nothing here was sent
to anyone.


---

## Sanitized-copy note

Phone numbers printed in the disclosure packet, the phone number and the tenant's personal email in Form 41, and the tenant's street address in Form 41 were redacted from the PDFs' text layers. Authentisign document-envelope IDs remain; they are signing-system references, not account numbers.
