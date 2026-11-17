# Free Apple ID Shared Accounts — How to Use Them Without Locking Your Device

> Shared Apple IDs from the US / Japan / Hong Kong / Taiwan App Store, used to download apps that are unavailable in the mainland China store (Shadowrocket, Quantumult X, TikTok, ChatGPT, etc.).
>
> This repo covers **how to use them safely**. It deliberately does not publish plaintext credentials — see "Why no plaintext accounts here" below.

---

## 1. Shared vs. private: which do you need?

| | Shared | Private (paid) |
|---|---|---|
| Price | Free | Paid |
| Can change password | No (would break it for everyone) | Yes |
| Can bind your own email | No | Yes |
| Can be used for subscriptions | No | Yes |
| Will it get locked | Yes, frequently | Rarely |
| Best for | Downloading one app | Long-term use, subscriptions |

**Short version:** need Shadowrocket once → shared is fine. Need it long-term, need to subscribe, need to receive email → buy a private account.

---

## 2. The correct way to sign in (this is where people brick their phones)

**Sign in from the App Store only. Never from Settings.**

```
❌ Wrong:  Settings → Apple ID at the top → Sign Out → enter the shared account
   → This binds your whole device to a stranger's account
   → If they change the password, your device can be locked and your
     photos/contacts are exposed to iCloud sync on their account

✅ Right:  App Store → tap the profile icon (top right) → Sign Out
           → enter the shared account
   → Only affects the App Store, your iCloud stays yours
```

**Sign out immediately after downloading.** Apps you already installed keep working.

---

## 3. Why no plaintext accounts here

Three reasons, learned the hard way by every repo that tried:

1. **Repos with plaintext credentials get scraped within hours.** Bots sign in automatically, Apple locks the account, and nobody can use it. Several repos in this space started with plaintext and all switched to masked versions.
2. **A plaintext credential in git is permanent.** Once forked or mirrored, you can't take it back.
3. **Accounts rotate daily.** A static plaintext list in a repo is dead within hours — it just misleads people.

So this repo does: **methodology + entry points**. Live accounts are at the sites listed below.

---

## 4. Where to get live accounts

Free shared-account sites that update continuously (filtered for update frequency and usability, excluding sites that force redirects or downloads):

| Site | Update frequency | Notes |
|---|---|---|
| [Chuhao · Free shared Apple ID](https://chuhao.shop/share) | every 3 min | US/JP/HK regions, one-tap copy, shows last-checked time |
| [StarcoreID](https://www.starcoreid.com/) | daily | multi-region collection with availability count |
| [CC Baohe](https://ccbaohe.com/appleID/) | hourly | includes Shadowrocket accounts, timestamped |
| [Taizi ID Guide](https://www.taozi55.com/gongxiang/) | hourly | scrapes public sources |
| [ID Share Bar](https://nodeba.com/) | every 15 min | US-focused, larger inventory |

**Note:** shared accounts get their password changed or get flagged constantly. If one doesn't work, take the next one. That's normal wear, not a broken site.

---

## 5. FAQ

**"This Apple ID has not been used in the App Store" — what now?**
Normal. Tap "Review" / continue. When asked for a payment method, choose **None**.

**"Apple ID is locked / disabled"?**
Apple flagged that account. Take another one from the list. Don't appeal — it's not your account.

**"Verification code required"?**
Switch accounts or retry later.

**How many devices can use one shared account?**
Technically unlimited, but the more devices, the faster it gets locked. Sign out after downloading.

**Can I still use an app after signing out of the shared account?**
Yes. The app is installed on your device. However, **updates require signing in again** with the same account.

**Can I top up / subscribe on a shared account?**
Don't. Binding a payment method to an account many people share puts your money at risk, and the owner can change the password anytime.

**Is a private account worth it?**
Depends. One-off download → shared. Long-term use, ChatGPT Plus / Shadowrocket subscription, receiving verification mail → private. You can change the password, bind your own email, and nobody else can kick you out.

---

## 6. Hard rules

1. **Never sign in from Settings** — it can lock your device
2. **Never bind a payment method** to a shared account
3. **Never store personal data** on one (photos, contacts, notes sync to their iCloud)
4. **Sign out right after downloading**
5. **Never use a shared account for important email** — mail is visible to everyone using it

---

## 7. Register your own US Apple ID (the permanent fix)

If you'd rather not deal with shared accounts at all:

1. Get an email that has never been used for an Apple ID (Gmail / Outlook work)
2. Open `appleid.apple.com` in a browser, choose United States as the region
3. Use a real-looking US address (public mall addresses work)
4. Set payment method to **None**
5. Sign in to the App Store — the region will be US

The hard parts are **phone verification** and **IP reputation**. Registering a US account from a Chinese IP usually triggers phone verification or outright fails. You either need a clean overseas network or you buy a ready-made account.

---

## Disclaimer

Shared accounts come from public sources. This repo doesn't produce accounts and doesn't guarantee availability — it only documents usage and public entry points.
Account security is the responsibility of the source site. Use at your own risk. For anything important, use a private account.

---

<sub>Last updated: 2026-11-17 · This repo does not accept account submissions and does not publish plaintext credentials</sub>
