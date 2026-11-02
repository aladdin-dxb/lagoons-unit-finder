# Lagoons Unit Finder

A one-page tool for DAMAC Lagoons (Dubai). Type a unit number and see:

- where the unit sits on the master plan
- the developer price it was bought at, and when
- every resale, developer sale and lease recorded on it
- the market price range and expected annual rent for its type (from comparable units nearby)
- any period you choose: last 3, 6 or 12 months, or a custom date range
- a PDF report you can send to a buyer or seller

Arabic, English and Chinese.

Built by Aladdin (licensed real estate broker, Dubai) with Claude.

## What is in this repo

This repo has the code only. It does not include the transactions data (`data.json`) or the master plan images, so the page opens empty until you add your own data.

## Where the data comes from

DLD resale deals, developer sales and Ejari leases, pulled from [DXBinteract](https://dxbinteract.com) with your own account.

## Keeping it updated

Deals happen every day, so the data needs a regular update. I run a weekly scheduled task with Claude that:

1. opens DXBinteract in my browser (logged in),
2. pulls the new deals and leases since the last update,
3. merges them into `data.json` without duplicates,
4. republishes the page.

The update scripts and the scheduled-task prompt will be added to this repo.

## Contact

- Instagram: https://www.instagram.com/aladdin.therealtor/
- TikTok: https://www.tiktok.com/@joealaddin
- YouTube: https://www.youtube.com/@joealaddin
- LinkedIn: https://www.linkedin.com/in/ahmedaladdin1/
