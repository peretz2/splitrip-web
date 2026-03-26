# SpliTrip — Expense Splitting for Group Travelers

An iOS app designed for Israeli travelers to split group expenses, scan receipts with AI, and settle debts via Bit or PayBox — with full Hebrew and English support.

<!-- <p align="center">
  <img src="screenshots/screenshot1.png" width="200">
  <img src="screenshots/screenshot2.png" width="200">
  <img src="screenshots/screenshot3.png" width="200">
</p> -->

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **UI** | SwiftUI (RTL support) |
| **Data** | SwiftData |
| **Sync** | CloudKit |
| **OCR** | OpenAI GPT-4 Vision |
| **Payments** | Bit & PayBox deep links |
| **Localization** | Hebrew + English |
| **Architecture** | MVVM |

## Key Features

- **Group Expense Splitting** — Add members, log shared expenses, calculate who owes whom
- **Receipt Scanning** — Photograph receipts and extract items/prices via GPT-4 Vision OCR
- **Hebrew OCR** — Accurate recognition of Hebrew text on Israeli receipts
- **Smart Settlement** — Minimized transaction algorithm to reduce number of payments
- **Bit & PayBox Integration** — Deep links to send/request payments directly in Israeli payment apps
- **CloudKit Sync** — Share trip data across devices
- **RTL Layout** — Full right-to-left support for Hebrew interface
- **Multi-Currency** — ILS (₪) default with support for other currencies
- **Universal Links** — Join trips via shared link

## Architecture

```
SpliTrip/
├── Models/          # SwiftData models (Trip, Expense, Member, Settlement)
├── Views/           # SwiftUI views with RTL support
├── ViewModels/      # Splitting algorithms, OCR processing
├── Services/        # GPT-4 Vision, CloudKit, deep links
└── Utils/           # Currency formatting, RTL helpers
```

## Links

- [Join a Trip (Universal Link)](https://peretz2.github.io/splitrip-web/join)
- [Support](https://peretz2.github.io/splitrip-web)
