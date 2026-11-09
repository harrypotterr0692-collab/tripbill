# TripBill – Driver Billing PWA

A starter, serverless billing app for Tours & Travels drivers. Each driver installs the same app on their own Android phone. Company settings, bill history and generated bills stay on that phone.

## Features in this starter
- Company name, phone, address and logo
- Driver/customer/vehicle and trip date
- Starting and ending odometer readings
- Automatic kilometres and fare calculation
- Extra charges and notes
- Local bill history
- PDF download and Android share sheet (where supported)
- PWA install support and cached app shell

## Important
- This version stores data locally on each phone. It does **not** sync records between drivers or provide central office reports.
- Host it on an HTTPS static host (GitHub Pages is a free option). A PWA service worker does not work reliably from a local `file://` URL.
- The PDF generator is loaded from a CDN, so connect to the internet the first time you use PDF export. The app shell itself is cached for offline use. If offline PDF generation is required, bundle the jsPDF library locally in a future revision.
- The PDF contains basic invoice details. Confirm local tax/invoice requirements with an accountant before using it as a GST tax invoice.

## Deploy free with GitHub Pages
1. Create a GitHub account and a new public repository, for example `tripbill`.
2. Upload all files from this folder to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Open the published HTTPS URL on each driver's Android phone in Chrome.
6. In Chrome, use **⋮ → Add to Home screen** or **Install app**.

## First use on each phone
1. Open the app and choose **Company setup**.
2. Enter the business name, phone, address and logo; save.
3. Create a bill from **New bill**.
4. Download PDF or use Share PDF to send it to the customer.

## Suggested next improvements
- Admin-controlled company profile shared with all drivers
- Driver-specific login and cloud sync
- Invoice numbering that remains unique across all drivers
- Backup/export and restore
- GST fields and configurable trip pricing rules
