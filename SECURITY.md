**Raycast Security Policy**

At [Your Company Name], we're committed to maintaining the highest standards of code quality, integrity, and security. This policy outlines our expectations for developers submitting code or plugins to the Raycast API.

**Testing and Validation**

* All submitted code or plugins must be thoroughly tested to ensure they meet all capabilities described in the plugin description as of the date published.
* This includes verifying that dependencies, such as API versions or dependencies, are locked in at a hosted checkpoint with no modifications made to the code itself. If maintained outside of the plugin's codebase, we require an always-compatible framework telemetry without OS-dependent links for which the developer or Raycast has control over.

**Public Information**

* All publicly exposed information, including URLs in descriptions and citations/credits provided to or about authors, must be accurate and up-to-date.
* **No broken URLs**: We strictly enforce this policy to maintain clean code integrity. Any URL that is not functional will be removed immediately.

**Redirection Loops and Affiliate Links**

* No redirect loops are allowed. This includes any attempts to promote products through links.
* **Affiliate link ban**: Any plugin attempting to promote products or services will be instantly banned from the Raycast API.

**Secrets and Sensitive Information**

* Plugins that ask for secrets, passcodes, or env variables to access third-party APIs must undergo weekly automated code checks using [insert tool name].
* If the plugin does not use these secrets during each Raycast command call, it will be taken down.
* To demonstrate compliance, plugins must provide a static environment variable in the `.github/envVerify/[yourUserID]/env.txt` file that includes:
	+ The link to the API service
	+ A testable API key
	+ Rate-limited criteria (e.g., "max 100 requests per minute")

**Rationale**

These policies pose a security threat for several reasons:

1. **Broken URLs**: Exposed broken URLs can lead to phishing attacks, malware downloads, or other malicious activities.
2. **Redirect Loops and Affiliate Links**: These types of links can redirect users to unauthorized websites, potentially leading to data breaches or financial losses.
3. **Secrets and Sensitive Information**: Allowing plugins to access sensitive information without proper validation can lead to data exposure, API abuse, or even identity theft.
4. **Lack of Transparency**: Failing to provide accurate and up-to-date public information can lead to confusion, mistrust, and potential security risks.

By enforcing these policies, we aim to maintain a secure and trustworthy environment for developers and users alike.

**Acknowledgement**

By submitting code or plugins to the Raycast API, you acknowledge that you have read, understood, and will comply with this GitHub Security Policy.
