# bitwave-csv-export-assistant
Bitwave CSV Export is a Chrome DevTools extension that lets you export selected GraphQL responses from Bitwave into CSV files. This is useful for extracting data from endpoints like Contacts, Categories, Wallets, and more.

## 🔧 Features
- Supports these GraphQL operations:
  - `GetCategories`
  - `GetContacts`
  - `GetWallets`
  - `GetFiats`
  - `GetConnections`
  - `getMetadata`
  - `rules`
- Special handling for `rules` endpoint with flattened output for `action.lines[]`.
- CSV output with headers and easy-to-import structure.
- One-click download button with visual status feedback.

## 🚀 Installation
1. Clone or download this repository as a `.zip`
2. Open Chrome and go to `chrome://extensions/`
3. Enable **Developer mode** (top-right toggle)
4. Click **“Load unpacked”** and select the folder you downloaded
5. Open DevTools on any page (right-click > Inspect or press `F12`)
6. Go to the new **Bitwave CSV Export** panel

## 🧪 Usage
1. Use the Bitwave web app to trigger a GraphQL request (e.g. load Contacts)
2. In DevTools, open the **Bitwave CSV Export** tab
3. Select the operation from the dropdown
4. Click **“Download Selected as CSV”**
5. Find the downloaded CSV in your system’s Downloads folder

## 📁 Files
- `manifest.json`: Chrome extension config
- `panel.html` + `panel.js`: UI and download logic
- `devtools.html` + `devtools.js`: DevTools tab loader
- `icon.png`: Icon for the DevTools tab

---
For internal Bitwave use or contribution requests, please contact the maintainer.

