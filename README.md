# verify
Verification of Smartintyg

Detta intyg är digitalt signerat med Ed25519.

Verifiering kan göras oberoende av Smartintygs plattform.

---

## 🔑 Public Key

Denna publika nyckel används för att verifiera signaturen på Smartintyg.

```
MCowBQYDK2VwAyEAPCxYBQ91z4NMHBU3cUW6P+DFCKQRfal/tcEqyAeXstk=
```

Algoritm: Ed25519  
Format: SPKI (base64)

---

## 🧾 Så verifierar du ett intyg

1. Extrahera följande från intyget:
   - certificate_id
   - verification_code
   - participant_name
   - course_name
   - issued_date
   - certificate_hash
   - certificate_signature

2. Skapa JSON:

```json
{
  "certificate_id": "...",
  "verification_code": "...",
  "participant_name": "...",
  "course_name": "...",
  "issued_date": "..."
}
