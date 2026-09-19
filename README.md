# 🟢 Slime Time — Farmer's Market Sales Dashboard

A simple, phone-friendly point-of-sale page for selling slime at the market.
It's a **single file** (`index.html`) — no app to install, no server, no accounts.

## What it does

- **Tap-to-add store** with the menu items and prices:
  - Plain Slime — **$5.00**
  - 2 Slimes + Mix-ins — **$9.00**
  - Mix-ins — pick **$0.25 / $0.50 / $0.75 / $1.00** each
  - Bag Charm — **$1.75**
  - Bin of Random Stuff — **$0.50**
- **Cart** with +/− quantity buttons and a running total.
- **Checkout two ways:**
  - **📱 Venmo** — opens Venmo pre-filled to pay **@Susan-Naughton** with the exact
    amount and an itemized note. The customer confirms and pays.
  - **💵 Cash** — records the sale without opening Venmo.
- **🧮 Custom tab** — a calculator for anything not on the menu (ad-hoc price × quantity).
- **📒 Sales tab** — every sale is logged (time, items, payment type, amount) with a
  running "total taken" for the day. Includes **Undo** and **Export Spreadsheet (CSV)**.

## How to use it at the market

1. Open the page on your phone (see hosting options below).
2. Tap items to build the order; adjust quantities in the cart.
3. Tap **Venmo** (customer scans/pays) or **Cash**.
4. At the end of the day, go to **Sales → Export Spreadsheet (CSV)** and open the file
   in Excel / Google Sheets for accounting.

> 💡 Sales are saved in the browser on that one device (via localStorage). Use the same
> phone + same browser all day, and **export the CSV before clearing the log**.

## How to open it on a phone

**Easiest — GitHub Pages (free public link):**
1. In this repo on GitHub: **Settings → Pages**.
2. Under "Build and deployment", set **Source: Deploy from a branch**, branch **main**, folder **/ (root)**, then Save.
3. After a minute you'll get a link like `https://mnaughton1981.github.io/Slime-Time/` —
   open it on the phone and bookmark it / add to home screen.

**Or, offline:** download `index.html` to the phone and open it in the browser. It works
with no internet (the Venmo button still needs a connection to open Venmo).

## Changing prices or items

Open `index.html` and edit the `ITEMS` list near the top of the `<script>` section.
The Venmo handle is the `VENMO_USER` value in that same block.
