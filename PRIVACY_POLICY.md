# Crew Report Privacy Policy

Last updated: April 9, 2026

Crew Report is a construction crew timekeeping app for iPhone. This Privacy Policy explains what information the app handles, how that information is used, and what choices users have.

## Information Crew Report Handles

Crew Report may store the following information that the user enters into the app:

- Crew member names
- Supervisor, reviewer, payroll-approver, and crew-lead names
- Crew member, supervisor, reviewer, and approver phone numbers
- Crew member, supervisor, reviewer, and approver email addresses
- Company information entered by the user
- Project, jobsite, project-template, archived-project, holiday-calendar, overtime-rule, and jobsite geofence information
- Time entries, live shift information, break minutes, saved shift timing, payroll details, hourly rates, regular, overtime, and double-time totals, banked hours, gross pay totals, bank-ledger review records, bank-forecast summaries, projected bank-impact data, daily-log attachment metadata, clock-in geofence status, and related calculations
- Planned crew schedules, project coverage targets, scheduling conflicts, and other project-planning information entered by the user
- Photo, camera-captured image, and document attachments that the user chooses to import into daily logs or into the separate project library, plus project-library tags, notes, and related metadata
- Approval workflow configuration, reviewer profiles, stage defaults, approver names, review notes, reopen history, review status records, audit-trail metadata, and delivery receipt history
- Crew Portal access-code settings, access-code hash and salt values, expiration dates, shared-device lockout state, weekly confirmation records, portal clock-in requests, and related supervisor approval or denial history
- Planned vacation ranges, vacation request statuses, project or template blackout dates, delivery-format preferences, queued reminder details, and related crew self-service updates entered in the app
- Union or trade classification information
- Notes, saved Quick Fill presets, report-builder presets, report visibility settings, delivery preferences, reminder preferences, sync diagnostics, merge summaries, conflict-review history, manual conflict-resolution choices, and other app content created by the user

## How Information Is Used

Crew Report uses this information only to provide the app's features, including:

- Tracking crew hours and payroll
- Tracking live shifts and break times
- Storing and presenting daily-log and project-library attachments selected by the user
- Supporting weekly crew scheduling, project coverage planning, and vacation or blackout conflict visibility
- Calculating and displaying bank-hour forecasts so future approved vacation and projected auto-use impact can be reviewed separately from actual bank usage
- Managing project-scoped approval workflows and review reminders
- Supporting Crew Portal features, including personal history, delivery preferences, vacation requests, weekly confirmations, direct clock-out actions, trusted sessions, shared-device access protection, and optional supervisor-reviewed clock-in requests
- Supporting vacation-planning tools, including blackout dates, overlap warnings, coverage planning, and supervisor review flows
- Generating reports and exports
- Sending or preparing reports through Apple's system share, message, and mail composers, document export tools, and clipboard fallback when direct sending is unavailable on the device
- Restoring saved app data and local snapshots
- Supporting optional reminders, widgets, Apple Watch companion flows, app lock, contact import, and attachment capture or import
- Verifying optional jobsite geofence status for live shifts and Crew Portal clock-in requests when the user has configured jobsite coordinates and granted location access
- Delivering optional arrival and departure alerts for saved jobsites when the user has enabled jobsite geofences, granted the necessary location access, and allowed notifications
- Syncing app data through the user's private iCloud account when available

Crew Report does not use this information for advertising, profiling, or third-party analytics.

## Contacts Access

Crew Report may request access to Contacts only if the user chooses to import a crew member or a reviewer or supervisor profile from the device address book.

If the user selects a contact, Crew Report may read the selected contact's name, phone number, and email address so those values can be copied into the app.

Contacts access is optional. If permission is denied, the user can still enter names and contact information manually.

## Photos, Camera, and Document Access

Crew Report can let the user attach images or documents to daily logs and to the separate project library.

When the user chooses to add an attachment, Crew Report may present Apple's photo picker, document picker, or camera capture interface. If the user chooses camera capture, iOS may request camera permission.

Only the photos, captured images, or documents that the user explicitly selects or creates for attachment are imported into Crew Report.

## Location Access

Crew Report can optionally request location access when the user enables per-project jobsite geofencing, enables arrival or departure alerts, or when a geofence-aware live shift or Crew Portal clock-in request needs on-site verification.

If location permission is granted, Crew Report may read the device location at the time of the relevant clock-in or shift workflow so it can compare that location against the saved project geofence and record whether the event was on site, off site, or unavailable.

If the user grants the higher level of location permission required for region monitoring, Crew Report may also monitor saved project geofences in the background so it can trigger optional local arrival or departure alerts when the device enters or exits a configured jobsite radius.

Jobsite coordinates and radius are entered by the user as part of project setup. Crew Report does not use location data for advertising, third-party analytics, or unrelated background tracking.

If permission is denied, clock-in and shift workflows can still proceed, but geofence status may be recorded as unavailable and optional arrival or departure alerts may not work.

## Biometric And Device Authentication

Crew Report can optionally require Face ID, Touch ID, or the device passcode when reopening the app.

This authentication is handled by Apple's LocalAuthentication framework. Crew Report does not receive, collect, or store biometric templates or the device passcode. The app only receives the success or failure result needed to unlock the interface.

## Notifications

Crew Report may request permission to send local notifications for daily time-entry reminders, running-shift reminders, approval-stage reminders, scheduled supervisor delivery reminders, and optional jobsite arrival or departure alerts.

These are local notifications generated on the device. Crew Report does not use remote push notifications for this reminder feature.

Some reminder notifications may include a deep link so opening the alert can return the user to the relevant project, review week, or send workflow inside the app.

## Local Storage

App data is stored locally on the user's device. This may include crew, payroll, live shift, portal, vacation, project, template, note, attachment, review, export, settings, sync, delivery, scheduling, project-library, bank-forecast, and diagnostics data entered into or generated by the app, including saved union defaults, project overtime overrides, project coverage targets, and jobsite geofence settings.

Crew Report may also keep local attachment files, including project-library files, a local snapshot, and a local backup copy of app data on the device to support recovery, migration, restore, merge review, and troubleshooting flows.

The primary on-device store is written with iOS file-protection settings, including complete file protection when supported by the device and operating system.

## Secure Credential And Lockout Storage

Crew Portal access codes are not stored only as plain reusable codes. Crew Report stores hashed credential data and related security metadata used to validate access on the device.

For shared-device Crew Portal protection, lockout state may also be stored in Apple's secure storage services on the device so failed-attempt limits and lockout timing can be enforced more safely.

## iCloud Sync and Backup

If the user is signed in to iCloud and iCloud is available on the device, Crew Report may sync app data to the user's private iCloud container.

This data is stored in the user's own iCloud account and is used so the user can keep Crew Report data available across their own devices and restore app state when needed.

When local changes and iCloud changes need to be reconciled, Crew Report may store merge summaries, merge-history metadata, conflict-review history, and user-selected conflict-resolution choices on the device so the user can review how conflicts were resolved.

Crew Report does not use a developer-hosted cloud database for user payroll data.

## Widgets, Watch, and App Group Storage

Crew Report includes an optional iPhone widget and Apple Watch companion app.

To support those experiences, the app writes a limited project snapshot into the app group's shared container on the user's device so the widget extension, App Clip, and Apple Watch companion can display current project totals, logging status, reminder status, review-stage information, triage and approval-focus context, running-shift summary information, the active-shift project context used for quick App Clip handoff, and the selected or pinned project context for that widget, App Clip, or watch session.

This shared snapshot stays on the user's device and is not used for advertising or third-party analytics.

## Diagnostics

Crew Report stores on-device diagnostics about sync, merge history, export, backup, restore, attachment handling, report-delivery events, reminder scheduling, watch handoff or supervisor actions, and related approval or portal workflow activity so users can review recent app activity and troubleshoot issues.

These diagnostics are stored locally, may be included in exported local snapshots, and are only shared externally if the user explicitly copies or exports them.

## SMS, Mail, Files, and Sharing

Crew Report can prepare reports, backups, snapshots, diagnostics, and ledger or history exports for sharing through Apple's system features, such as the system message composer, mail composer, share sheets, clipboard fallback, and file export options.

When the user chooses to share or export content, the selected data is handled through Apple's system sharing tools. Crew Report does not operate a developer-hosted messaging service for these exports.

If the user exports a backup, snapshot, or report to Files, iCloud Drive, Mail, Messages, or another destination selected in the system share flow, that transfer is initiated by the user. Any handling after export is governed by the destination service or app the user chooses.

If the device cannot send a message or email directly, Crew Report may copy prepared report content to the clipboard so the user can paste it into another app.

Crew Report does not silently send SMS messages or emails in the background. Scheduled supervisor delivery reminders reopen the app into a prepared send flow so the user can complete the delivery themselves.

## Tracking, Analytics, and Advertising

Crew Report:

- Does not track users across apps or websites
- Does not use IDFA
- Does not include third-party advertising SDKs
- Does not include third-party analytics or behavioral profiling tools

## Data Sharing

Crew Report does not sell personal information.

Crew Report does not share user data with third parties for advertising or marketing purposes.

Information may be processed by Apple services only when required for app functionality selected by the user, such as iCloud storage, local device permissions, device authentication, or system sharing flows.

## User Choices

Users can:

- Deny Contacts permission and enter information manually
- Deny camera permission and continue using manual entry plus existing photo or document imports that remain available through Apple's system pickers
- Deny location permission and continue using the app without on-site geofence verification
- Decline the higher-privilege location access needed for background jobsite arrival or departure alerts and continue using the app without those alerts
- Deny notification permission
- Disable the app lock feature in Settings
- Disable iCloud through Apple device settings
- Cancel scheduled reminders inside the app
- Remove or rotate Crew Portal access credentials and adjust shared-device lockout settings inside the app
- Change or revoke Crew Portal access by removing portal access codes, expiring them, or adjusting lockout settings inside the app
- Delete local app data by removing the app or replacing data with a restored backup
- Control iCloud availability through their Apple device and iCloud settings
- Choose whether to export backups, local snapshots, reports, or diagnostics

## Children's Privacy

Crew Report is not directed to children under 13.

## Changes to This Policy

This Privacy Policy may be updated from time to time. The latest version should be made available wherever Crew Report is distributed or supported.

## Contact

For privacy questions about Crew Report, users can contact the developer through the support method listed on the App Store product page or through the project's GitHub repository:

- https://github.com/slb4life/Crew-Report