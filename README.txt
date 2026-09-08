PLC Vehicle Report Site

Files:
- index.html
- vehicle.html

1) Publish your Google Sheet to the web as CSV, then put the CSV URL in BOTH files:
   const SHEET_CSV_URL = "https://docs.google.com/spreadsheets/d/....../gviz/tq?tqx=out:csv&sheet=Sheet1";

2) Put your payment/checkout URL in vehicle.html:
   const FULL_REPORT_URL = "YOUR_FULL_REPORT_PAYMENT_URL";

3) Replace https://YOUR-DOMAIN.com in canonical URLs.

Expected Google Sheet columns:
Motors Name, Model, Colors, KM, VIN, Engine, LotNumber, Photo1, Photo2, Photo3, Photo4

The vehicle page is:
vehicle.html?id=VIN

Notes:
- Empty photo cells are handled.
- Duplicate photo URLs are removed.
- Search is case/space insensitive.
- Ad placeholders are intentionally included; replace them with the official AdSense code after approval.
- For serious SEO at scale, server-rendered unique vehicle URLs are preferable to query-string-only client rendering.
