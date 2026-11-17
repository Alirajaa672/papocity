# Legal documents for Google Play: PAPO'City: Zombie Car Survival

| File | What it is | Where it goes |
|---|---|---|
| `privacy-policy.html` | Privacy Policy (required by Google Play because the game has ads and uses the advertising ID) | Host it at a public URL; paste the URL in Play Console → App content → Privacy policy, and in the store listing |
| `terms-of-service.html` | Terms of Service (optional for Play, recommended) | Host it next to the privacy policy |
| `data-safety-answers.md` | Ready answers for the Play Console forms (Ads, Advertising ID, Target audience, Content rating, Data safety) | Copy into Play Console |
| `app-ads.txt` | AdMob seller file | Root of your developer website, before real ads go live |

## 1. Fill in the placeholders first
Search both HTML files for `[` and replace:
- `[SUPPORT EMAIL]`: a support address players can write to (Play Console also asks for a contact email).
- `[BUSINESS ADDRESS]`: your business address (Google requires a physical address for apps with ads/monetisation).
- `[COUNTRY]` (terms only): the country whose law applies.
Check that **Robosoft** is the exact name of the developer as shown in your Play Console account.

## 2. Host them at a public URL
Google needs a normal web page (not a PDF or Google Doc that needs a login). Free options:
- **Google Sites:** create a site, add a page per document, paste the text, publish.
- **GitHub Pages:** create a public repository, upload the two `.html` files, enable Pages; the policy is then at `https://<user>.github.io/<repo>/privacy-policy.html`.
- **Your company website:** upload the files, e.g. `https://your-domain.com/papocity/privacy-policy.html`.
Open the URL on your phone in a private browser window to confirm it loads without signing in.

## 3. Keep them true
These documents describe the game as built on 17 Nov 2026: no accounts, no purchases, save data only on the device, Google AdMob rewarded videos, Unity crash diagnostics, local-network (IP) multiplayer. Update them (and the Data safety form) if any of that changes, e.g. adding in-app purchases, Firebase/analytics, cloud saves or online multiplayer.

These are templates written from the game's actual behaviour, not legal advice. For a commercial release, have them reviewed by someone who knows the law in your country.
