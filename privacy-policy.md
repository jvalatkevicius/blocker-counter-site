---
title: Privacy Policy – Blocker Counter
---

# Privacy Policy

**App:** Blocker Counter for Jira Cloud
**Provider:** [jvalatkevicius](https://github.com/jvalatkevicius)
**Effective date:** 26 September 2026

This policy explains what data the Blocker Counter app ("the app") accesses, why, and how it is
handled. The app is built on Atlassian Forge and runs entirely on Atlassian's cloud infrastructure.

## Summary

- The app does not send any data outside Atlassian. It has no external servers and makes no
  outbound network requests.
- The app does not collect, store, or process personal data such as names, email addresses, or
  issue content.
- The only thing the app stores is a number: the "Issues blocked" count, saved in a read-only
  custom field on your Jira issues.

## Data the app accesses

To calculate counts, the app reads the following from your Jira site:

| Data | Why |
|---|---|
| Issue IDs | To identify which issues to calculate. |
| Issue links of type "Blocks" | To work out which issues block which. |
| Issue status category (for example "Done") | Resolved issues are not counted as blocked work. |
| The app's own "Issues blocked" field value | To avoid rewriting values that have not changed. |

When a user opens the app's administration page, the app asks Jira whether that user has Jira
administrator permission. It uses the answer only to allow or deny access to the page and does not
store it.

Atlassian provides the app with your site's licence status for the app. The app uses it only to
decide whether to keep counts updated.

The app does **not** read issue summaries, descriptions, comments, attachments, or user profile
information.

## Data the app stores

- **"Issues blocked" field values.** A number stored on each issue in your own Jira site, using
  Jira's standard custom field storage.
- **Operational logs.** Like all Forge apps, the app writes diagnostic logs to Atlassian's Forge
  platform, for example "Recalculated 5 issue(s)". These logs can include Jira's internal numeric
  issue IDs and counts. They contain no personal data or issue content. Atlassian retains them
  under its own policies.

The app has no database, cookies, analytics, or tracking of any kind.

## Where data is processed

All processing happens on Atlassian's cloud infrastructure through the Forge platform, within the
same Atlassian environment as your Jira site. The app is eligible for Atlassian's
[Runs on Atlassian](https://go.atlassian.com/runs-on-atlassian) program, which identifies apps that
do not send data outside Atlassian. See Atlassian's
[Privacy Policy](https://www.atlassian.com/legal/privacy-policy) for how Atlassian handles data.

## Sharing with third parties

The app does not share, sell, or transfer data to any third party. The provider has no access to
your Jira data.

## Data retention and deletion

"Issues blocked" values stay in your Jira site while the app is installed. When you uninstall the
app, it stops accessing your site, and Atlassian handles the removal of app data in line with its
policies for Forge apps.

## Your rights

Because the app does not process personal data, the provider does not hold personal data about you.
If you have a question or a data request, use the contact details below.

## Changes to this policy

If the app changes in a way that affects this policy, the policy will be updated and the effective
date above will change.

## Contact

Open an issue at
[github.com/jvalatkevicius/blocker-counter-site/issues](https://github.com/jvalatkevicius/blocker-counter-site/issues).
