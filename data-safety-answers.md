# Play Console answers: PAPO'City: Zombie Car Survival

Answers for the Play Console forms under **Policy and programs → App content**, based on what the game actually does (checked in the code on 17 Nov 2026). Re-check them if you add a new SDK, accounts, purchases or analytics.

## Privacy policy
- URL: the public web address where you host `privacy-policy.html` (see README.md).

## Ads
- **Does your app contain ads?** Yes.

## Advertising ID
- **Does your app use advertising ID?** Yes.
- Purpose: **Advertising or marketing** (AdMob rewarded videos). Also tick **Fraud prevention, security and compliance** if offered (AdMob uses it for invalid-traffic detection).

## Target audience and content
- **Target age groups:** 13–15, 16–17, 18 and over. Do **not** select any group under 13 (ads + cartoon gore would bring the Families policy requirements).
- **Could the app unintentionally appeal to children?** Answer honestly; the cartoon art may lead Google to ask. If asked, explain the game is a violent zombie survival game aimed at teens and adults.
- **Content rating questionnaire (IARC):** category **Game**. Violence: cartoon/fantasy violence with blood towards non-human characters (zombies). No sexual content, no gambling, no user-to-user chat, no purchases of digital goods with real money. Shares location: No (the app itself doesn't; ad SDKs are covered by Data safety).

## Data safety

**Does your app collect or share any of the required user data types?** Yes (through the AdMob and Unity SDKs).

**Is all of the user data collected by your app encrypted in transit?** Yes.

**Do you provide a way for users to request that their data be deleted?** Choose the option that the data is not linked to an account: game data lives only on the device and is deleted by uninstalling; ad data is controlled by the user's advertising ID settings. (If the form requires Yes/No, answer No and explain this in the policy.)

| Data type | Collected | Shared | Optional? | Purposes | Source |
|---|---|---|---|---|---|
| Location → Approximate location | Yes | Yes | No | Advertising or marketing, Fraud prevention, Analytics | AdMob (from IP address) |
| Device or other IDs → Device or other IDs | Yes | Yes | No | Advertising or marketing, Fraud prevention, Analytics | AdMob (advertising ID) |
| App activity → App interactions | Yes | Yes | No | Advertising or marketing, Analytics | AdMob (ad views/clicks) |
| App info and performance → Crash logs | Yes | No | No | Analytics (app stability) | Unity Diagnostics, AdMob |
| App info and performance → Diagnostics | Yes | Yes | No | Analytics, Advertising or marketing | Unity Diagnostics, AdMob |

**Not collected:** name, email, user IDs, phone number, address, precise location, financial info, contacts, photos/videos, audio, files, messages, calendar, health, web browsing, installed apps.

Before submitting, compare with Google's own guidance for the AdMob SDK (search "Google Mobile Ads SDK data disclosure"). If you later add Firebase, Unity Analytics, in-app purchases or accounts, this table must be updated.

## Ads consent (needed before production, not for closed testing)
Players in the EEA, UK and Switzerland must be shown a consent message before personalised ads. Set up a **GDPR message** in AdMob → Privacy & messaging, and the game must call Google's User Messaging Platform (UMP) at start-up. Tell Claude when you are moving to production and it will add the UMP call next to the AdMob code.
