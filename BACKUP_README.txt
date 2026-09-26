PURIXA CRM v22.31 BACKUP
========================

This backup contains the complete web/PWA CRM project files.

IMPORTANT BUSINESS RULE
- New Sale customer is automatically created in the Customers master list when needed.
- New Service customer created through the Service "New Customer" flow is automatically saved in Customers and linked to the service.
- New AMC customer created through the AMC "New Customer" flow is automatically saved in Customers and linked to the AMC.
- Existing customers are matched by normalized mobile number to avoid duplicate customer records.
- Service completion updates the customer's next service date to 3 months later.
- AMC stores the linked customerId and updates the customer's AMC end date.

FILES
- index.html              CRM application
- manifest.json            PWA manifest
- sw.js                    Service worker/cache
- purixa-logo.png          Logo
- authorized-signature-clean.png  Signature
- icon-192.png             PWA icon
- icon-512.png             PWA icon
- BACKUP_README.txt        Backup notes

VERSION
- CRM: v22.31
- Service worker cache: purixa-crm-v22.31

SAFE BACKUP PRACTICE
1. Keep this ZIP unchanged as the master backup.
2. Keep a second copy on your Mac/USB/Google Drive.
3. Before future edits, make a new versioned ZIP (v22.32, v22.33, etc.).
4. Do not delete the original v22.30 backup until the new version has been tested.
