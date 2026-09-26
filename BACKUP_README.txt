PURIXA CRM v22.31 BACKUP
========================

This is the corrected complete web/PWA CRM project backup.

IMPORTANT CUSTOMER MASTER RULE
- New Sale: customer is automatically created/linked in Customers.
- New Service: customer created through Service > New Customer is automatically saved/linked.
- New AMC: customer created through AMC > New Customer is automatically saved/linked.
- Existing customers are matched by normalized mobile number first, then by name, to avoid duplicates.
- IMPORTANT FIX: if Firebase/old data contains Sales, Services or AMC records but the Customers collection is empty/incomplete, CRM v22.31 automatically reconstructs the missing Customer Master records and links those transactions.
- Service completion updates the customer's next service date to 3 months later.
- AMC stores the linked customerId and updates the customer's AMC end date.

FILES
- index.html
- manifest.json
- sw.js
- purixa-logo.png
- authorized-signature-clean.png
- icon-192.png
- icon-512.png
- BACKUP_README.txt
- FIREBASE_BACKUP_INFO.txt

VERSION
- CRM: v22.31
- Service worker cache: purixa-crm-v22.31.1

TESTING NOTE
The screenshots supplied by the user show v22.30 with Sales/Service/AMC records present while Customers displays "No customers found". That is the exact orphan-customer problem fixed in this v22.31 build.

SAFE BACKUP PRACTICE
1. Keep this ZIP unchanged as the master backup.
2. Keep a second copy on Mac/USB/Google Drive.
3. Before future edits, make v22.32, v22.33, etc.; never overwrite the master without another backup.
4. Keep the original v22.30 backup separately.
