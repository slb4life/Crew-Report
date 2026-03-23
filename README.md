# Crew Report App

Crew Report App is a standalone SwiftUI iPhone app for tracking construction crew hours, live shifts, payroll, approvals, exports, data recovery files, widgets, reminders, and iCloud sync.

Minimum OS: iOS 17.0.

Privacy policy: see [../PRIVACY_POLICY.md](../PRIVACY_POLICY.md).

## Features

### Crew And Projects

- Add crew members manually or import them from iPhone contacts.
- Prevent duplicate crew-member names from being saved inside the same project so reviews, payroll totals, and exports stay unambiguous.
- Crew cards show each member with a color-coded initials avatar using a consistent personalized color derived from their name.
- Assign each crew member a union and reuse saved union names across the app.
- Create separate projects or jobsites so crew assignments, payroll weeks, reviews, exports, and reminders stay scoped to the right job.
- Archive older projects without removing active jobs from the management list.
- Save reusable project templates, edit them later, create new projects from them, or apply them to the current project without changing crew assignments.

### Time And Payroll Tracking

- Log one full crew work day at a time from Home or Crew in a fixed Monday-to-Sunday payroll week.
- Select who worked, leave everyone else OFF, and enter hours as totals or by start and end time.
- Apply the same hours and notes to all selected crew members with one quick-fill action.
- Start, end, discard, and update break minutes for live shifts one crew member at a time or from the dedicated whole-crew live clock controls in the full-crew logger.
- Choose how a log is recorded: Day, Night, Holiday, or Bank Hours.
- Start a live shift for today, track elapsed time, adjust break minutes, and end or discard the running shift later.
- Highlight today inside the weekly Home calendar strip so the current day stands out while reviewing the week.
- Split Monday through Friday hours automatically according to the configured overtime threshold, including weekly 40-hour mode.
- See the active overtime mode badge on every weekday entry so supervisors always know which rule is in effect.
- Store Saturday entries as overtime and Sunday entries as double time.
- Add and track bank hours from daily logs or manual adjustments in the crew editor.

### Delivery And Exports

- Export reports as PDF, CSV, or Simple Text.
- Control report field visibility separately for Simple Text, PDF, and CSV, including optional shift start/end times, break minutes, and note fields.
- Preview the full report content before sharing. CSV and PDF exports open an inline preview sheet where the report can be reviewed and then shared or closed.
- Simple Text reports use compact OFF markers, including emoji-based absence reasons, to keep text-message exports short and readable.
- Send weekly reports to selected crew members, with each member receiving only their own hours, and optionally send the full weekly summary to the supervisor.
- Save per-project weekly crew delivery defaults and company-wide daily supervisor delivery defaults that route through the linked Supervisor reviewer profile.
- Use quick-send shortcuts to skip the export dialog, crew delivery menu, or recipient picker when repeating the same flow.
- Queue supervisor delivery reminders and reopen the app into the prepared send flow later. Crew Report does not silently send those reports in the background.

### Crew Portal

- Crew members can open a personal Crew Portal from the supervisor side or unlock it on a shared device with a per-member access code.
- Home only shows the shared-device Crew Access entry when the current project has at least one active crew member with a valid, non-expired access code.
- The portal shows the current week summary, hours confirmation, delivery receipts, and personal weekly history with per-week daily log expansion.
- Crew members can update their preferred delivery format directly in the portal.
- Crew members can submit, edit, and cancel requested vacation ranges in the portal, while approved and denied ranges remain read-only.
- Portal access codes support expiration and lockout settings controlled in Settings, are persisted as hashed credentials, and now keep shared-device lockout state in secure storage.

### Holidays And Reviews

- Use the standard observed holiday calendar or set custom project-specific holiday dates.
- Configure automatic holiday pay and bank-entry eligibility per built-in union, including whether holiday hours are added, how many hours are applied, and whether Bank entries can accrue hours.
- Review each payroll week in a calendar-style crew grid with worked days, OFF days, and holiday-paid days.
- Configure a 1-step, 2-step, or 3-step approval workflow in Settings, with Crew Lead, Supervisor, and Final Payroll stages available as needed.
- Create reusable reviewer profiles with role, phone, email, and notes, then assign them as the default identities for Crew Lead, Supervisor, and Payroll approvals.
- Bank ledger approve, reject, and reopen actions now reuse the same Supervisor and Payroll reviewer profiles, and each bank review snapshot keeps the reviewer role and contact metadata in the audit trail.
- Post an approval-stage reminder when a week advances to the next required sign-off stage so follow-up reviews are less likely to stall.
- Weekly approval controls week-approved calculations and bank ledger effects, while exports and delivery remain available from Home and History using the current report settings.
- Set vacation request status (Requested, Approved, or Denied) on each planned time-off range per crew member. Crew cards display a color-coded status badge alongside the vacation dates.

### History And Reporting

- Browse older payroll periods from a separate History tab without changing the active week on Home.
- Filter history by date range, week, month, year, crew member, union, or holiday-paid weeks.
- Track review history, reopen actions, exports, and text activity inside History.
- Weekly review rows show each member's effective union holiday and overtime rules alongside that week's totals.
- Reuse the same export format and visibility settings from Home when sending or exporting History summaries.
- Show only the relevant hour categories for each entry, including overtime, double time, holiday hours, and bank hours when available.

### Home And Widgets

- See current project totals, active crew, and running shifts from the Home tab.
- Open full-crew day logging, exports, reviews, and send actions directly from the Home screen.
- Crew cards show each union's live holiday and overtime rules so supervisors can confirm the current setup without opening Settings.
- See any queued supervisor reminder on Home, including its due time, and cancel it before it fires.
- Use the widget to monitor project totals, review state, today’s logging status, reminders, and running shifts.
- On supported iOS versions, pin widget instances to specific projects.
- Widget deep links can reopen the app directly into the relevant project and review context.

### Settings And Data

- Save company details and approval defaults so reports, payroll reviews, and supervisor delivery use the same company name and linked reviewer identities.
- Save reusable reviewer identities and stage defaults so approval sheets and bank ledger reviews can preload the right reviewer and retain contact metadata in the audit snapshot.
- Control which sections appear in Simple Text, PDF, and CSV reports.
- Manage saved union names, per-union holiday rules, overtime behavior, default rates, approval workflow stages, delivery defaults, appearance, privacy lock settings, reminder types, and quick-send behavior from Settings.
- Change the app language to English, Portuguese (Portugal), or System Default and see the new copy apply immediately across the app.
- Use Sync Tools to inspect iCloud status, recent merge activity, conflict-review history, merge outcomes, and diagnostics.
- Choose Automatic, Light, or Dark appearance mode.
- Require Face ID, Touch ID, or the device passcode when reopening the app.
- Save the primary on-device store using iOS file protection when available.
- Export a full Data File containing crew, projects, payroll history, reviews, activity, settings, and local sync metadata.
- Restore from a current Data File or from an older backup JSON export when recovering the same device or moving to another device.
- Keep the local datastore on device and sync the app state through iCloud when available, including after a fresh install or a newly restored device signs back in.

## Open in Xcode

1. Open `CrewReportApp.xcodeproj`.
2. Select the `Crew Report App` scheme.
3. Choose an iPhone simulator or a real iPhone running iOS 17 or later.
4. Press Run.

## Notes

- Contact import only works after granting Contacts permission.
- Daily log reminders, running-shift reminders, approval-stage reminders, and queued supervisor delivery reminders only work after granting notification permission.
- Shared-device Crew Access only appears when at least one crew member in the current project has a valid portal access code.
- The overtime threshold badge in daily logging reflects the per-project setting configured in Project Management.
- Vacation request statuses are stored per crew member and persist through iCloud sync, Data File restore, and older backup JSON restore.
- Pending Crew Portal clock-in requests also persist through sync, Data File restore, and older backup JSON restore.
- Crew Portal vacation edits are limited to Requested ranges so approved and denied requests stay supervisor-controlled.
- Crew members without phone numbers appear as unavailable in the report recipient picker.
- Saved project templates stay editable from the Project Templates list before you reuse or apply them.
- Weekly crew delivery defaults are stored per project, while daily supervisor delivery defaults are company-wide and use the linked Supervisor reviewer profile when available.
- The preferred export format also drives the default supervisor attachment format for weekly email and text delivery when an attachment-based format is selected.
- SMS sending only works on devices that support `MFMessageComposeViewController`.
- Mail sending only works on devices that support `MFMailComposeViewController`.
- Queued supervisor reminders reopen Crew Report into a prepared send flow; they do not perform autonomous background SMS or email delivery.
- On the simulator, text and email fall back to copying the prepared report content to the clipboard when direct sending is unavailable.
- Bank ledger totals and other week-approved calculations update only after the configured approval workflow is complete for that week.
- Restoring a Data File replaces the current local data on the device.
- The app lock relies on Apple's device authentication APIs. Crew Report does not receive or store biometric templates.
- The primary local store is written with iOS complete file protection when the device supports it.
- Widget data is shared through the app group container and reflects the latest saved app snapshot.
- Change the bundle identifier and signing team in Xcode before installing on a real iPhone.