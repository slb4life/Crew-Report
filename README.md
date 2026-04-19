# Football iPhone App Starter (Xcode)

This workspace also includes **Crew Report**, a standalone SwiftUI iPhone app with widget, App Clip, and Apple Watch support for tracking construction crew hours, live shifts, payroll, approvals, exports, scheduling, project files, daily-log attachments, data recovery files, reminders, and iCloud sync.

This workspace also includes **ServicePilot**, a standalone SwiftUI iPhone app with widget support for solo service businesses to track jobs, route stops, invoices, payments, expenses, customer portals, and backups.

- Crew Report app notes: [CrewReportApp/README.md](CrewReportApp/README.md)
- Crew Report changelog: [CrewReportApp/CHANGELOG.md](CrewReportApp/CHANGELOG.md)
- Crew Report privacy policy: [PRIVACY_POLICY.md](PRIVACY_POLICY.md)
- ServicePilot project: `ServicePilot.xcodeproj`
- ServicePilot scheme: `ServicePilot`
- ServicePilot base bundle identifier: `com.servicepilot.app`

## Crew Report

- Standalone SwiftUI iPhone app for crew hours, payroll, multi-stage reviews, project-based history, attachments, and report delivery, with companion widget and Apple Watch support.
- Supports live shifts, reusable quick-fill presets, union-driven or project-overridden overtime rules with visible mode badges, crew self-service portal access codes, trusted portal sessions, vacation request statuses, project blackout dates, duplicate crew-name protection, inline CSV/PDF previews, detailed and simple text summaries, approval-stage reminders, Data File recovery, widgets, sync conflict review, and iCloud sync.
- Includes per-project jobsite geofencing with configurable coordinates and radius so live shifts and portal clock-in requests record whether crew are on site.
- Includes a weekly Scheduling Board with drag-and-drop crew assignment, project-level target crew counts, coverage-gap warnings, approved-vacation conflicts, and blackout-date visibility.
- Includes bank-hours forecasting that separates actual used hours from future impact so upcoming approved vacation and auto-use can be reviewed without reducing the current displayed balance early.
- Includes a project-level document and photo library, separate from daily logs, with tags, notes, camera capture, file import, preview, delete, and sync or restore support.
- Includes daily-log photo and document attachments with import, camera capture, preview, sharing, History visibility, Crew Portal visibility, and sync/restore support.
- Includes expiring QR check-in links, App Clip handoff for quick clock-in or clock-out entry, Siri shortcuts, and an interactive home widget shortcut for faster crew actions.
- Adds vacation-planning operations tools including blackout dates, planner overlap and coverage warnings, approval-history context, and a Home-entry vacation request inbox.
- Adds cross-project History operations, including a dedicated dashboard plus batch export with preview and share flows for the currently filtered crew range.
- Adds advanced report builder presets with reusable audience-specific layout options and PDF branding controls.
- Approval, PDF, text, and CSV report rule labels now focus on overtime and holiday behavior; bank activity still appears through bank-hour, payable, and balance totals instead of a separate Bank Rule label.
- Adds Apple Watch triage, approval, reopen, and Crew Portal request actions, while accessory-inline watch widgets surface compact project badges and status.
- Optional geofence arrival and departure alerts can monitor saved jobsites in the background when the user grants the required location permission.
- Weekly report delivery now keeps Home and History aligned around the same detailed/simple text formatting, selected-crew filtering, supervisor routing, and saved text-or-email delivery defaults.
- Weekly send and export actions now stay approval-gated and only surface text or email options that actually have eligible recipients for the selected week.
- Recipient picking now keeps unavailable crew visible with explicit reasons, including missing contact details or no report data for that week.
- Sync conflict review now records the base payload and can show field-level semantic merge details for deletes, restores, concurrent edits, and archive-state merges.
- Widget refresh timing now has an adaptive backstop based on live shifts, reminders, pending review state, snapshot age, and day boundaries instead of relying only on explicit app-side publish calls.
- Supports optional Contacts import, camera/photo/document attachment flows, Face ID / Touch ID / device-passcode app lock, and protected on-device local storage.
- Open `CrewReportApp.xcodeproj` in Xcode and select the `Crew Report App` scheme to run it.

For Crew Report development, archiving, or App Store upload work, use `CrewReportApp.xcodeproj` and the guidance in `CrewReportApp/README.md` plus `APP_STORE_REVIEW.md`. The FootballApp steps below apply only to the separate Football web-wrapper app.

This starter gives you a **real iPhone app shell** for your Football site using SwiftUI + WKWebView.

## FootballApp Starter

### 1) Open the included Xcode project

1. Open `ios-app-starter/FootballApp.xcodeproj` in Xcode.
2. Select the `FootballApp` scheme.

### 2) Set your signing team

1. Select the `FootballApp` target.
2. Open **Signing & Capabilities**.
3. Pick your Apple ID Team.
4. (Optional) change Bundle Identifier from `com.example.FootballApp`.

### 3) Set your web URL

Open `FootballApp/AppConfig.swift` and set `defaultURLString` to your Football site URL.

Examples:
- `http://bsp-nas.local/football/`
- `http://192.168.10.35/football/`

### 4) Info.plist notes

`FootballApp/Info.plist` is already configured with:

- `NSAppTransportSecurity` / `NSAllowsArbitraryLoads = YES` (for local HTTP)
- `NSFaceIDUsageDescription`
- `NSLocalNetworkUsageDescription`

### 5) Run on iPhone

1. Connect iPhone to Mac.
2. In Xcode, select your iPhone as run destination.
3. In Signing & Capabilities, choose your Apple ID Team.
4. Press Run.

### 6) What this app already has

- Loads your Football web app in a native iOS app container.
- Pull-to-refresh.
- Back/Forward controls.
- Open in Safari action.
- Progress spinner + friendly error state.
- Persistent web session/cookies via `WKWebsiteDataStore.default()`.
- App settings screen (editable server URL + reload).
- Optional Face ID / Touch ID app lock.
- Clear Cookies & Cache action.

### 7) Next upgrades (optional)

- Native push notifications.
- Native theme switch (light/dark/manual override).
- Offline fallback page + smart retry strategy.
- Deep links to specific pages (match, player, news).
