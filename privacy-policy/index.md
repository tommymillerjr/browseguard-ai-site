# BrowseGuard AI Privacy Policy

Last updated: 2026-06-12


## Summary

BrowseGuard AI is designed to help warn users about suspicious, scammy, or deceptive webpages while minimizing unnecessary data exposure.

The extension primarily uses local browser checks. Local BrowseGuard protection remains the controlling protection layer. AI Advisory output, when available, is optional and informational, does not control enforcement, and should not be treated as a guarantee that a page is safe or unsafe. Real AI/deception runtime is not the basis of the current beta package.

Chrome may describe BrowseGuard AI as able to read and change data on websites because the extension needs page access to check links, forms, login fields, page text signals, URL patterns, and suspicious behavior while users browse. BrowseGuard AI performs local browser safety checks first and is designed not to collect passwords, form values, cookies, auth tokens, full page HTML, or raw private user-entered content. Optional AI Advisory features use minimized, sanitized risk metadata and do not control enforcement.

## What BrowseGuard AI does

BrowseGuard AI checks webpages for risk signals such as suspicious wording, risky forms, possible impersonation patterns, and other scam/deception indicators.

Depending on the page risk level, BrowseGuard AI may:

- show a popup status
- show a warning overlay
- warn before risky interactions
- keep local scan history
- allow the user to trust a page or site
- show AI Advisory wording when enabled and available

Current beta behavior is:

- Low risk remains quiet by default, with visible-value popup copy.
- Medium risk remains visible in popup, history, and Page Report, but is
  non-interruptive by default.
- High risk remains interruptive with warning overlays and Proceed Anyway
  friction.

## Information processed locally

BrowseGuard AI may process the following information locally in the browser:

- current page URL information
- hostname and path information
- page title or visible warning phrases
- local page risk signals
- whether forms, password fields, or suspicious terms are present
- local risk score and risk level
- trusted page/site settings selected by the user
- recent scan history and protection events

This information is used to provide local page safety warnings and extension functionality.

## Information stored locally

BrowseGuard AI may store extension settings and local safety history in browser extension storage, including:

- trusted sites
- trusted pages
- recent scan summaries
- protection events
- repeat-offender counts
- AI Advisory setting
- provider mode setting
- backend endpoint setting if the user configures one

This storage is used so the extension can remember user choices and show recent safety activity.

## AI Advisory behavior

AI Advisory features are optional and informational.

When AI Advisory is disabled, BrowseGuard AI should continue using local protection checks.

When AI Advisory is enabled, BrowseGuard AI is designed to send only a limited, sanitized payload for advisory review when applicable. The intended sanitized payload avoids unnecessary sensitive details and focuses on safety-relevant signals.

The current safety model is:

- AI Advisory output is informational.
- Local BrowseGuard protection remains the controlling protection layer.
- AI Advisory output should not lower local risk.
- AI Advisory output should not suppress local warnings.
- AI Advisory output should not override local blocking behavior.
- Real AI/deception runtime is not the basis of the current beta package.

## Backend/provider behavior

BrowseGuard AI may support backend proxy mode for AI Advisory analysis.

The intended design is that provider access is controlled by the backend, not by bundling provider secrets inside the extension.

The extension should not include private API keys or provider secrets in the packaged extension.

## Information not intentionally collected

BrowseGuard AI is not intended to collect:

- passwords
- form values
- cookies
- auth tokens
- full page HTML
- raw private user-entered content
- payment card numbers
- bank account numbers
- form field values entered by the user
- full private messages
- full email contents
- unnecessary personal information
- browser history outside the extension safety features

BrowseGuard AI should not ask users to enter sensitive information into suspicious pages for testing.

## Limited Use and data-use limits

BrowseGuard AI uses page access and locally stored safety data only to provide
browser safety features, user-selected trust choices, extension settings, and
optional advisory diagnostics.

BrowseGuard AI is designed not to sell, share, or use browsing safety data for
advertising, unrelated profiling, or unrelated product purposes.

## Query strings and fragments

BrowseGuard AI should avoid sending full query strings or hash fragments to advisory systems unless that behavior is explicitly reviewed and approved later.

The safer default is to use limited hostname/path and safety-signal information rather than full URLs containing unnecessary private details.

## Third-party services

BrowseGuard AI may use a backend service for AI Advisory analysis if the user enables/configures that mode.

Any future third-party AI/provider use should be documented before public release, including what limited information is sent and why.

## Tester safety

During beta testing:

- testers should not intentionally visit dangerous websites
- testers should not enter real passwords into suspicious pages
- testers should not enter payment information into suspicious pages
- testers should not submit private personal information into suspicious pages
- controlled test pages are preferred for risky-page examples

## Data control

Users can clear local extension history and change extension settings through the extension UI where supported.

Trusted page/site settings are controlled by the user and are stored locally for extension behavior.

## Children and sensitive use

BrowseGuard AI is designed as a browser safety helper. It is not a replacement for parental supervision, security software, user judgment, or professional security review.

## Limits of protection

BrowseGuard AI cannot guarantee that every page is safe or unsafe.

It may miss risky pages, warn on safe pages, or behave unexpectedly on some websites.

Users should treat BrowseGuard AI as an additional safety helper, not as their only protection.

## Contact

For beta feedback or support, use the project feedback path provided with the beta tester materials.

Project website: https://github.com/tommymillerjr/browseguard-ai-site

Privacy policy URL: https://tommymillerjr.github.io/browseguard-ai-site/privacy-policy/
