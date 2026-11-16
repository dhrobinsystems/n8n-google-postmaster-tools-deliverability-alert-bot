# ⚠️ Disclaimer & Liability Limitation

**Repository:** `n8n-google-postmaster-tools-deliverability-alert-bot`
**Author:** DH Robin (dhRobin Systems)
**Last updated:** November 2026

Use at your own risk. The code, workflows, and scripts in this repository (`n8n-google-postmaster-tools-deliverability-alert-bot`) are provided for educational and architectural demonstration purposes.

* **No Liability:** The author and dhRobin Systems accept no responsibility or liability for any direct, indirect, incidental, or consequential damages that result from using, misusing, or deploying these scripts. That includes, without limitation, deliverability problems that are missed, detected late or misjudged, false alarms, sending decisions (pausing, throttling or continuing campaigns) made from a derived health grade, lost email revenue, domain or IP reputation damage, API charges, and any message posted to a connected service.

* **No Warranty:** All software, n8n JSON blueprints and JavaScript modules are provided "AS IS", without warranty of any kind, express or implied. This includes, but is not limited to, warranties of merchantability, fitness for a particular purpose, and non-infringement. Google Postmaster Tools data can be delayed, sampled, incomplete or unavailable for low-volume domains, and Google changes the API and its metrics over time. The health grade, thresholds and redaction patterns are illustrative defaults, not guarantees.

* **Production Testing Required:** Always test thoroughly in an isolated staging environment, such as a test Google Cloud project, a non-critical Postmaster domain and a test Slack channel, with `SANDBOX_MODE=true` and `DRY_RUN=true` enabled, before you connect live Google or Slack credentials. Treat every grade and alert as a prompt to investigate in Postmaster Tools, not as Google's own assessment.

* **Not Google's Reputation Score:** The HIGH / MEDIUM / LOW / BAD grade is computed by this workflow from the metrics Google still publishes. It isn't Google's domain or IP reputation (which Google retired from Postmaster Tools v2), and it isn't endorsed by Google.

* **Third-Party APIs & Compliance:** You alone are responsible for complying with the terms of service, rate limits, data privacy regulations (GDPR/CCPA), email sender requirements and anti-spam laws, and security policies of Google, Slack and any connected services. That includes protecting OAuth client secrets and refresh tokens, granting only the scopes you need, keeping domain and traffic data inside appropriate channels, and following Google's bulk-sender guidelines.

* **No Affiliation:** This project is independent. It is not affiliated with, endorsed by, or sponsored by Google LLC, Slack Technologies, LLC, Salesforce, Inc., or n8n GmbH. Gmail and Postmaster Tools are trademarks of Google LLC. All product names and trademarks belong to their respective owners and are used only to describe compatibility.

* **Fictional Sample Data:** All domain names (under the reserved `.example` suffix), metric values, compliance results, dates and stored states in the pinned sample data and documentation are fictional and exist only for testing. Any resemblance to real organisations is coincidental. Placeholder values such as `YOUR_GOOGLE_OAUTH_CLIENT_ID`, `YOUR_GOOGLE_OAUTH_CLIENT_SECRET`, `YOUR_GOOGLE_OAUTH_REFRESH_TOKEN`, `YOUR_GOOGLE_POSTMASTER_API_KEY`, `YOUR_SENDING_DOMAIN.example` and `YOUR_SLACK_WEBHOOK_URL` must be replaced with your own values, which you keep in environment variables or n8n credentials.

* **Not Professional Advice:** Nothing in this repository is legal, compliance or deliverability consulting advice. Consult qualified professionals for decisions in those areas.

## Open-Source License Notice

This project is released under the MIT License. You may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the conditions in [LICENSE](./LICENSE). The MIT License's own warranty disclaimer and limitation of liability apply in addition to this document. If the two conflict, the terms more protective of the author apply to the extent permitted by law.

---

Full text: DISCLAIMER.md · Licensed under the MIT License. License: MIT © 2026 DH Robin (dhRobin Systems) · Provided as-is, see the disclaimer.
