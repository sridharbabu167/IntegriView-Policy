# Privacy Policy — IntegriView Chrome Extension

**Last updated: October 2026**

## Overview

IntegriView is a Chrome Extension for inspecting, comparing, and auditing SAP Integration Suite artifacts. This policy explains what data the extension handles and how it is stored.

## Data Collected

IntegriView stores the following data **locally in your browser's `localStorage`** on your own machine:

- SAP Integration Suite tenant URLs
- Authentication credentials (username/password for Basic auth, or client ID and client secret for OAuth)
- OAuth token URLs
- GitHub Personal Access Token (PAT)
- Application preferences (theme, collapsed state)

No personally identifiable information (name, email, address) is collected.

## How Data Is Used

Stored credentials are used solely to:

- Authenticate with your own SAP Integration Suite tenant APIs (`*.hana.ondemand.com`) to fetch integration artifacts, package lists, and externalized parameters
- Obtain OAuth tokens from your tenant's authentication endpoint (`*.authentication.sap.hana.ondemand.com`)
- Authenticate with your GitHub repository to read integration artifact files

## Data Storage

All data is stored exclusively in **your browser's `localStorage`**, scoped to the extension origin (`chrome-extension://...`). Data never leaves your machine except as direct API calls to the SAP and GitHub endpoints you configure.

## Data Sharing

We do not:

- Sell or transfer user data to third parties
- Send data to any external server operated by the extension developer
- Use data for purposes unrelated to connecting to your configured SAP IS tenants and Git repository
- Use data to determine creditworthiness or for lending purposes

## Data Removal

To remove all stored data, go to Chrome Settings → Privacy and security → Site data → find the IntegriView extension origin and clear it. Alternatively, uninstalling the extension removes all associated `localStorage` data.

## Contact

For questions about this privacy policy, open an issue at:
https://github.com/sridharbabu167/IntegriView_Extension/issues
