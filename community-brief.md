# GitHub community feedback forum — brief digest

## Overview

The GitHub community feedback forum (github.com/community) is GitHub's public space where users post suggestions, bug reports, and questions about GitHub products — including GitHub Mobile, GitHub Discussions, GitHub Codespaces, GitHub Sponsors, GitHub Issues, and more. Posts are organized into categories (for example Accessibility, GitHub Education, and Apps, API and Webhooks), where GitHub product teams review submissions alongside community discussion. Newly submitted feedback typically receives an automated acknowledgment comment explaining how feedback is cataloged and where to track the changelog and product roadmap.

## Discussion #210962 — "1"

Category: Accessibility. This discussion (labeled as a Bug, topic area Actions) was opened by user bo913032-ux on 2026-10-22, and its body contains only an attached file upload (content.pdf) with no descriptive text. It received the standard automated "Your Product Feedback Has Been Submitted" acknowledgment and no substantive replies. Comment count: 1.

## Discussion #201375 — "I am in China. and https://github.com/settings/education/benefits does not work in China. So, i have to use VPN to access services."

Category: GitHub Education. The poster, itzosmann, reports that the GitHub Education benefits verification page is unreachable from China without a VPN, yet the verification system rejects the application for using a VPN and for a location mismatch, even though a school email was already verified. Community replies suggest turning the VPN off immediately before submitting, applying from a university network, and contacting GitHub Education support (support.github.com/contact/education or education@github.com) with enrollment documents so the verification can be handled manually via the document path. Comment count: 3.

## Discussion #190228 — "Error Assigning Copilot via API: \"The agent encountered an error and was unable to start working on this issue: This may be caused by a repository ruleset violation\""

Category: Apps, API and Webhooks. danmcpherson reported that assigning Copilot to an issue via the REST API (and likewise via GraphQL, GitHub CLI, or third-party bots) returns HTTP 201 but then fails in the issue timeline with a "repository ruleset violation" error, even though no rulesets exist at the repository or organization level; assigning via the web UI works fine. The thread shows many users hitting the same failure intermittently over several months, with reports that OAuth/app-installation tokens worked while fine-grained PATs failed, alternating periods of recovery and relapse, and workarounds such as calling the agent-tasks REST API endpoint and switching models. No official root cause or fix was confirmed in the thread. Comment count: 34.

## Sources

- Discussion #210962: https://github.com/orgs/community/discussions/210962
- Discussion #201375: https://github.com/orgs/community/discussions/201375
- Discussion #190228: https://github.com/orgs/community/discussions/190228

## Open questions

- For discussion #190228, GitHub staff never confirmed a root cause or a fix for the intermittent "repository ruleset violation" failure when assigning Copilot via the API; it is unclear from the discussion alone whether this was resolved on GitHub's side or whether the suggested workarounds (OAuth tokens, the agent-tasks REST endpoint) were ever officially endorsed.
- For discussion #201375, there is no indication from the discussion alone of what the GitHub Education verification workflow supports for users in regions where a VPN is required to access GitHub, nor whether a manual document-based verification path is generally available beyond the community-suggested support ticket route.
- For discussion #210962, the attached content.pdf referenced in the discussion body could not be read through the API, so the substance of the reported accessibility bug remains unknown.
