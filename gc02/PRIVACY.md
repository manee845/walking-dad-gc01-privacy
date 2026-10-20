# Privacy notice – The Walking Dad – GC02 Beta

Private Garmin Beta · 20 October 2026

[Deutsch](PRIVACY_DE.md)

This notice covers the private GC02 beta used to test recording and additional Garmin Connect metrics.

## 1. Controller and contact

Manuel von Allmen, Switzerland, is responsible for the app described here and for handling his own support requests. Contact: [support.thewalkingdad@gmail.com](mailto:support.thewalkingdad@gmail.com).

Data you provide to this app or its developer support is provided to Manuel von Allmen, not Garmin. Garmin does not accept responsibility or liability for that app-specific processing; Garmin's own services and processing are separate.

## 2. Scope and purpose

This notice covers The Walking Dad – GC02 Beta, the private Garmin Connect IQ trial for Fenix 6 Pro based on GC02-B1/schema 3. The app records walks and distinguishes manually selected modes: 0 = stroller (Kinderwagen), 1 = baby carrier (Babytrage), and 2 = without baby (Ohne Baby). It does not collect names, baby weights or its own child profiles. The planned “child walking independently” mode is not implemented.

## 3. Processing on the Garmin watch

The app processes timestamps, active duration and distance, companion mode, segment order and segment boundaries. It displays available native Garmin activity values, including heart rate, average/maximum heart rate, speed or pace, ascent and calories. The app does not implement its own step counting. Availability varies by device and activity.

## 4. Location, activity and sensor data

Outside the recovery view, opening the app activates continuous location events, before you manually start an activity. Native walking recording starts after your manual start; a GPS fix is recommended but is not a prerequisite. Poor or missing reception can leave route and distance data incomplete. Location events may continue during pauses and the end-of-activity review and are disabled on successful completion or app exit. Garmin handles native route and sensor recording, which may include additional device, profile and fitness metadata not directly requested by our app.

## 5. Custom FIT developer fields

The app adds technical fields for segment history, mode sequence, UTC time origin, active duration, distance, data quality and mode totals to the native FIT activity. Six additional metrics are configured for the summary: active duration and distance for stroller, baby carrier and without baby. There are twelve SESSION fields and four RECORD fields, including ten technical contributions not intended for user display. These technical data nevertheless remain in the FIT file. Successful display of the six metrics in Garmin Connect has not yet been confirmed for this beta.

## 6. Local storage and recovery

Two checkpoints are written alternately to app storage, read back and checked for integrity. They include a local activity identifier, revision, timestamps, activity/save status, segment history, counters and mode totals. They do not contain a full raw GPS route or heart-rate history. The last selected mode and technical activity counters are stored separately. SHA-256 integrity checking is not encryption. Recovery displays a local partial record; it neither resumes the original native recording nor exports a FIT file from that record.

## 7. Garmin Connect and disclosure

Using Garmin synchronization can transfer saved FIT activities, including the GPS route, native sensor data/metadata and our developer fields, to Garmin Connect. Garmin accounts, synchronization, sharing and other Garmin functions are subject to Garmin’s independent processing and settings. Local saving does not confirm synchronization. See the [Garmin Connect privacy policy](https://www.garmin.com/privacy/connect/). Deleting local checkpoints does not delete a Garmin Connect activity.

When combined with a GPS route, the timing and modes of companion segments can reveal family routines.

## 8. Own servers, accounts and diagnostics

The reviewed app contains no direct HTTP transmission, proprietary cloud server, advertising/tracking or external analytics services and requires no separate The Walking Dad account. It does not directly send activities to the developer. Permissions are Fit (native recording), FitContributor (additional FIT fields) and Positioning (location events). App diagnostics use fixed, data-minimized status/error messages without segment or location dumps. This does not retroactively delete historical logs or system logs created by Garmin.

## 9. Retention and deletion

Local checkpoints have no fixed expiry period. After confirmed native saving and a verified completion record, the app attempts to delete both checkpoints and verifies deletion by reading back. Uncertainty, interruption or deletion errors can leave all or part of the data in place. Explicitly confirmed discarding requests deletion of the relevant local checkpoints and verifies their absence by reading back. Where a native recording is present, it must first be successfully discarded. Recovery discarding affects only the local checkpoints. Errors can leave data partly or wholly in place; deletion is not reported as complete until verified. “Later/Close” in recovery preserves existing data. Checkpoint deletion preserves the mode preference and counters. You manage saved FIT activities and synchronized data using Garmin’s functions. Complete erasure through uninstalling, from backups or system logs, or from physical flash remnants is not guaranteed.

## 10. Email support

When you contact support, Manuel von Allmen processes sender details, your message and voluntary attachments through Gmail (Google) to answer your request. Only Manuel has access to the support mailbox. Please do not send unnecessary location, health, child-related or FIT data. Messages are kept as needed; the mailbox is reviewed at least every six months and unneeded messages are deleted unless justified retention applies. Google generally identifies Google Ireland Limited (Ireland) for Swiss consumer accounts; processing may occur in the US and other countries. See [Google’s privacy policy](https://policies.google.com/privacy?hl=en) and [transfer frameworks](https://policies.google.com/privacy/frameworks?hl=en). Google describes adequacy mechanisms, the Swiss–US Data Privacy Framework and standard contractual clauses for international transfers; their application depends on the particular transfer.

## 11. Hosting this notice

This notice is published as files in the public GitHub repository manee845/walking-dad-gc01-privacy. GitHub processes connection and usage data, including IP addresses, when you access its website. Providers are GitHub B.V. (Netherlands) or GitHub, Inc. (US); processing in the US and other countries is possible. We add no analytics scripts, external fonts or media to the notice files. GitHub's website functions, cookies, retention and independent processing are described in [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). GitHub describes standard contractual clauses and its participation in the Swiss–US Data Privacy Framework for international transfers; the applicable mechanism depends on the transfer.

## 12. Rights and contact

Contact [support.thewalkingdad@gmail.com](mailto:support.thewalkingdad@gmail.com) to request access to personal data we process, or correction, deletion, delivery/portability or to raise objections where provided by law. Where processing relies on consent, you may withdraw it for the future. We assess requests under applicable law and may require suitable identification to prevent unauthorized disclosure. The app does not give the developer access to your entire Garmin account. Direct requests about Garmin’s independent processing to Garmin. You may also contact the competent supervisory authority, including the [FDPIC](https://www.edoeb.admin.ch/en) in Switzerland.

## 13. Changes and date

This notice will be updated when the processing described materially changes. Date: 20 October 2026. The current German and English versions are available in this directory.
