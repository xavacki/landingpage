# xavacki studio website — 29 October 2026

Static redesign of the existing landingpage repository, preserving its CNAME, Git history and original
unused assets. No external UI framework, CDN, tracking script or website storage is loaded by the new pages.
The logo is copied from the game splash artwork, not redrawn. Game screenshots/art remain game assets.
Patrick Hand is hosted locally with the supplied OFL. No store availability, ratings or release date is invented.

## Review and publish

The changed pages are index.html, privacy.html, termsofservice.html and delete-account.html. New pages:
cookies.html and legal-notice.html. Shared styling/art is in assets/. Keep CNAME = xavacki.com.
Publish through the existing repository/hosting workflow; no new Sites-hosted copy is registered.
Do not push unrelated pre-existing changes or commit secrets/IDE files. A backup of the original edited
pages is kept outside the repository at /tmp/xavacki-landingpage-before-redesign.tar.gz for this session.

Check clean URLs /privacy, /termsofservice, /delete-account, /cookies and /legal-notice on the live host.
The game’s links use the clean URLs; relative .html navigation also works in a local file preview.

## Operational items (not solved by website copy)

- The accompanying game source adds optional Analytics collection, off before consent, and Settings →
  Analytics & privacy. Build, test on a device and distribute that version. The policy explicitly describes
  earlier builds so it does not imply old installations already have consent controls.
- Verify the actual Analytics user/event retention window and whether activity resets it in property
  560456585. The current Firebase CLI login lacks Analytics Admin read scope. The public policy describes
  the configured rolling-expiry criterion rather than inventing a two- or fourteen-month setting.
- Default backend logs were verified as 30 days and required audit logs as 400 days on 29 October 2026.
- Run the support mailbox review/rights-request process described by the policy. Evaluate when retention
  is necessary rather than keeping unrelated messages indefinitely. Do not delete an active legal hold.
- The operator identity/address and 13+ intended audience come from the game’s existing developer-supplied
  documentation. Confirm actual registration/tax/consumer obligations before real-money sales; this site
  does not establish a company or professional registration.
- Test account deletion and real purchase/refund lifecycle with license testers. No such action is
  performed while editing the website.
- Keep Play Data safety, audience, store listing and deployed SDK/configuration consistent with these pages.
- Validate international provider agreements and safeguards applicable to the actual accounts and regions.

Sources: Google Play User Data policy; Firebase privacy and data-processing terms; Google consent-mode
Android guidance; EU consumer-rights guidance. Public links are included in the relevant pages.
