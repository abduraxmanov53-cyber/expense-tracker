# Expense Tracker — Flutter (iOS-only, Drift)

This is an iOS-only Flutter expense tracker (local-only) using Drift for SQLite.

Core features included:
- Add / edit / delete expenses (amount, date, category, merchant, notes, receipt image)
- Categories
- Dashboards with charts (fl_chart)
- CSV import/export
- Budgets (per-category monthly)
- Recurring transactions (local scheduler)
- Local-only storage via Drift (no cloud sync)

Setup
1. Install Flutter SDK: https://flutter.dev
2. From project root, run:
   - flutter pub get
   - flutter pub run build_runner build (to generate Drift code)
   - flutter run

Notes
- This project targets iOS only; Android folders are removed.
- iOS Info.plist needs NSCameraUsageDescription and NSPhotoLibraryUsageDescription.
- CI workflow runs on macOS to allow iOS build checks.
