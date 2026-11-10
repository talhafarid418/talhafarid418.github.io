# AutoTech Lab — public information site

This repository contains the **public informational homepage and privacy policy** for the AutoTech Lab owner-operated YouTube uploader. It is separate from the private video production repository `talhafarid418/autotech-lab-youtube`. No OAuth secrets, tokens, video files, or upload automation belong here.

## Publish with GitHub Pages

1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Set **Branch: main** and **Folder: / (root)**, then select **Save**.
4. Once GitHub finishes publishing, verify these URLs in a signed-out browser:
   - Homepage: https://talhafarid418.github.io/
   - Privacy policy: https://talhafarid418.github.io/privacy.html

## Google OAuth consent configuration

1. In Google Cloud → Google Auth Platform → **Branding**, enter the site homepage and privacy policy URLs above, complete required details, and save.
2. The **Authorized domains** and site ownership verification requirements depend on Google's checks. GitHub Pages does not guarantee that the shared `github.io` domain will be accepted as a verified authorized domain. If Google rejects it, use a custom domain you control and verify that domain in Google Search Console.
3. In **Audience**, publish the OAuth app when Google permits it, following any required verification process. OAuth publishing status does **not** change YouTube video privacy.
4. If necessary, reauthorize your existing OAuth client to obtain a new refresh token, replace the matching `YOUTUBE_REFRESH_TOKEN` secret in the private production repository, and verify with the **OAuth-only health check** before any production upload.
5. **Never create duplicate daily triggers, bypass the one-shot upload checkpoint, or change the `privacyStatus: private` setting.**

Review the public privacy-policy language against actual data practices, and revise it if practices change. These pages are informational only; they do not sign users into Google or access the YouTube API.
