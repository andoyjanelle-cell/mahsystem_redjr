# RedJr Builders and Construction Supply — Point of Sale & Inventory

A browser-based point-of-sale (POS), order, inventory and reporting system built with plain HTML, CSS and JavaScript. No install or build step is needed.

## Run locally
1. Extract the ZIP and keep `index.html`, `styles.css`, `script.js` and the `images/` folder together.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari).

## Demo access
- Email: `admin@redjr.test`
- Password: `redjr123`

## What's in the system
- **Point of Sale** – tap products or scan/type a SKU and press Enter, change quantities, apply Senior/PWD (20%) or custom discounts, take payment (Cash with change, GCash, Maya, card, bank transfer), print a receipt, hold and resume sales, and print a Today's summary. Shortcuts: `F2` focus search, `F9` charge.
- **Stock updates automatically** when a sale is completed. Cancelling an order returns its items to inventory.
- **Dashboard** – today's sales, transactions, monthly totals, a **Monthly sales bar graph**, recent orders and an inventory watch list.
- **Inventory** – stock table plus a **Stock levels bar graph** (green = in stock, amber = low, red = out, black mark = reorder level). Switch between quantity and % of reorder level. The graph follows the search and stock filter.
- **Reports** – Monthly sales bar graph (6 or 12 months, sales or number of orders), status breakdown and top products.
- **Products / Orders / History** – the delivery/pickup ordering flow, order status updates, product catalog and activity log remain available.
- CSV export for orders, inventory and history.

## Data and going live
- Data is saved in the browser (`localStorage`) so it **stays after refresh**. It is stored per browser and per device; it is not shared between computers.
- The system ships with sample products and 11 months of **demo sales** so the graphs have data. Open the account menu (top-right avatar):
  - **Reset demo data** restores the samples.
  - **Start fresh (go live)** deletes all sales/orders/history but keeps your products and stock. Do this before recording real sales.
- Prices are treated as **VAT-inclusive (12%)**. Receipts are sales receipts only and are not official BIR receipts.
- Login is still a front-end demo, not secure authentication. For multi-user or multi-device use, a backend and database would be needed.

## Deploy to Vercel
1. Upload the project to a GitHub repository.
2. In Vercel choose **Add New → Project**, import the repo, framework preset **Other**, leave the build command blank, output directory `.`.
3. Deploy. No environment variables are needed.

## Product photographs
Product cards load photos from Wikimedia Commons. If a photo cannot load (for example, offline), the bundled illustrations in `images/` are shown instead. Check each source page for license and attribution terms before redistributing:
- Portland cement bags: https://commons.wikimedia.org/wiki/File:Portland_Cement_Bags.jpg
- Concrete block: https://commons.wikimedia.org/wiki/File:Concrete_block.jpg
- Steel nails: https://commons.wikimedia.org/wiki/File:Steel_nails.jpg
- Combination pliers: https://commons.wikimedia.org/wiki/File:Adjustable_pliers_kwb_387710.JPG
- Adjustable wrench: https://commons.wikimedia.org/wiki/File:Adjustable_wrench_2.jpg
- PVC pipe: https://commons.wikimedia.org/wiki/File:PVC_pipe.JPG
- Electrical tape: https://commons.wikimedia.org/wiki/File:Electrical-tape_black.jpg
- Screws: https://commons.wikimedia.org/wiki/File:Screws.jpg
- Paintbrush: https://commons.wikimedia.org/wiki/File:Paintbrush.JPG
- Corrugated GI sheet: https://commons.wikimedia.org/wiki/File:Corrugated_iron_(AM_2016.25.1-8).jpg
