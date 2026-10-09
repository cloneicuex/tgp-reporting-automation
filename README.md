# TGP reporting automation

Timer for the CGMI The Grace Place Abuja reporting application.

The application owns recipients, reminder dates, pending-work summaries, review notifications and duplicate-safe delivery history. The scheduled workflow calls its protected notification endpoint at 08:00 Africa/Lagos and hourly for retries. Report and action submissions trigger immediate review emails within the application.

Authentication uses short-lived GitHub OIDC identity restricted to this repository, main branch and notification workflow. No email-provider keys or church records are stored here.

Workflow pushes perform a dry run only. Manual runs default to dry-run; scheduled runs deliver only due notifications.
