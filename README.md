[README (1).md](https://github.com/user-attachments/files/33333433/README.1.md)
<p align="center">
  <img src="docs/logo.png" width="160" alt="Watch & Bark logo">
</p>

<h1 align="center">Watch &amp; Bark</h1>

<p align="center">
  <b>Free job alerts for Google Chrome.</b><br>
  Watch & Bark checks job websites for you and <b>barks</b> the moment a new job is posted.
</p>

<p align="center">
  <img alt="Free" src="https://img.shields.io/badge/price-free-22c55e">
  <img alt="Chrome" src="https://img.shields.io/badge/browser-Chrome-0b1d12">
  <img alt="Manifest V3" src="https://img.shields.io/badge/manifest-v3-16a34a">
  <img alt="Version" src="https://img.shields.io/badge/version-4.0.0-15803d">
</p>

---

## ✨ What it does

- 🐶 **Watches almost any job site**: NHS Jobs, Indeed, LinkedIn, Reed, BMJ Careers, Totaljobs, Glassdoor, Monster, Seek, Naukri, Rozee, Bayt and more. You can watch several sites at once.
- ⏱ **Checks as often as you like**: type any time, from **1 second** to **hours**.
- 🔔 **Barks only for the jobs you want**, using one of three modes:
    - **Every new job**
    - **Keywords**: include, exclude, locations
    - **✨ AI rule**: describe what you want in plain English *(optional)*
- 🔊 **21 alert sounds**: barks, chimes, alarms and more, or **upload your own**.
- 🔄 **Page refresher**: auto-refreshes **any** web page. It can also **bark when a word appears or disappears**, such as "Apply now".
- 📱 **Phone alerts** *(optional)*: through the free [ntfy](https://ntfy.sh) app, Discord or Slack.
- 💤 Snooze, quiet hours, "only check during these hours", and backup or import of your settings.

**100% free. No account, no sign-up, no adverts, no tracking.**

---

## ⬇️ Install (about 2 minutes)

Watch & Bark is installed straight from this GitHub page.

1. **Download.** Click the green **`<> Code`** button at the top of this page, then **Download ZIP**.
2. **Unzip.** Open your **Downloads** folder, right-click the ZIP file and choose **Extract All** → **Extract**. On a Mac, just double-click it.
3. **Open the extensions page.** In Chrome, type `chrome://extensions` in the address bar and press **Enter**.
4. **Turn on Developer mode** with the switch in the **top right** corner.
5. **Load it.** Click **Load unpacked**, choose the folder you unzipped (the one with **`manifest.json`** inside), and click **Select Folder**.
6. **Pin it.** Click the 🧩 puzzle-piece icon at the top of Chrome and click the 📌 pin next to **Watch & Bark**.

The Settings page opens by itself when it's installed. 🎉

> **Tip:** Keep the unzipped folder somewhere safe, such as Documents. Chrome runs the extension from that folder, so don't delete or move it.

---

## 🚀 Set up (2 minutes)

### 1. Add a job website
Search on your favourite job site as usual (job title, location, filters) and **sort by newest** if you can. Copy the page address, paste it into **Settings → Job websites to watch**, then click **Test this page**. When Chrome asks for permission to read that site, click **Allow**.

<img src="docs/sites.png" width="720" alt="Adding a job website">

### 2. Choose how often to check
Type any time, for example `45 seconds`, `5 minutes` or `2 hours`.

<img src="docs/checktime.png" width="720" alt="Check time">

> For big sites like **LinkedIn** and **Indeed**, check every **2–5 minutes** and keep **"Vary the timing slightly"** on, so the site doesn't block you.

### 3. Choose when to bark
<img src="docs/modes.png" width="720" alt="When to bark">

### 4. Pick a sound
Press **▶ Play** to hear it, then click **Save settings**. Use **🐶 Send test bark** to check that your sound works.

<img src="docs/sounds.png" width="720" alt="Sounds">

**That's it.** Keep Chrome open (it can be minimised). When a new job appears, Watch & Bark barks and shows a notification. Click the notification to open the job.

---

## 🐕 Using it

Click the dog icon in your toolbar to see your jobs:

<img src="docs/popup.png" width="360" alt="Popup">

| You'll see | Meaning |
|---|---|
| 🔴 **NEW** | Posted since you last checked |
| ✅ Green reason | Matches what you want, and why |
| Faded / *Skipped* | Didn't match your rule (still shown, nothing is hidden) |
| 💤 **Snooze 1 h** | Pause alerts for an hour |
| ⏱ **Check jobs every** | Change the check time right from the popup |
| ✨ **Ask AI** | Ask about your jobs, e.g. *"which close this month?"* |

### 🔄 Page refresher
Click the **refresh button** in the popup to auto-refresh the page you're on:

- **Every** any number of seconds, minutes or hours, or a **random** time in a range.
- **Bark when text appears / disappears**, e.g. `Apply now`. You can make it stop refreshing once the text is found.
- **Stop after N refreshes**, and **hard refresh** to skip the browser's saved copy.

<img src="docs/refresher.png" width="360" alt="Page refresher">

---

## ✨ AI (optional)

The AI is **optional**. Everything else works without it. The extension is free; the AI uses **your own API key**, so you pay the AI company only for what you use (usually a fraction of a cent each time new jobs appear).

**What it does:**
1. **AI rule**: reads each new job and barks only for good matches, with a short reason.
2. **Write my rule**: type what you want in your own words, and the AI writes a clear rule for you.
3. **Ask AI**: ask questions about the jobs you're watching.

**Get a key (one time):**
- **Anthropic (Claude), the default:** sign up at [console.anthropic.com](https://console.anthropic.com), add a little credit under **Billing**, then open **API keys** → **Create key**.
- **OpenAI:** [platform.openai.com/api-keys](https://platform.openai.com/api-keys) → **Create new secret key**, then choose *OpenAI* as the provider.

Paste the key in **Settings → When to bark → ✨ AI rule**, write your rule, and click **Try this rule on current jobs**.

<img src="docs/ai.png" width="720" alt="AI rule writer">

**Example rules:**
- *Bark for Clinical Fellow or Trust Grade posts at FY2–IMT level in Emergency or Acute Medicine in England. Skip locums and anything closing within 5 days.*
- *Band 5 or 6 ICU or theatre nurse roles in London or Kent. Skip agency and bank shifts.*
- *Remote junior or mid-level React developer roles. Skip unpaid internships.*

> If your rule needs details that aren't in the job list (visa sponsorship, salary, rota), turn on **Read the full job description**.

---

## 📱 Phone alerts (optional, free)

1. Install the free **ntfy** app ([ntfy.sh](https://ntfy.sh)) and subscribe to a topic with a long, random name, e.g. `my-job-alerts-7f3k`.
2. In **Settings → Phone or chat alerts**, paste `https://ntfy.sh/my-job-alerts-7f3k`, then click **Send test**.

You can also paste a **Discord** or **Slack** webhook address.

> Anyone who knows an ntfy topic name can read its messages, so keep the name long and random.

---

## 🔒 Privacy

- Everything is stored **only in your browser**. There's no account and no server of ours.
- Watch & Bark only reads the job websites **you add**, and only after you click **Allow**.
- If you use the AI, job titles and listing text (and full descriptions, if you turn that on) are sent **only to the AI company you choose**, and only when new jobs appear or you ask a question. Your API key never leaves your browser except to that company.
- Phone alerts are sent only to the address you paste in.

---

## 🛠 Troubleshooting

<details><summary><b>I don't hear anything</b></summary>

Click **🐶 Send test bark** in Settings. Check your computer's volume and that Chrome isn't muted, and make sure **quiet hours** aren't on. Chrome must be open; it can be minimised.
</details>

<details><summary><b>"Test this page" finds no jobs</b></summary>

1. Log in to that job site in Chrome.
2. Click **⚙** next to the site → **How to read the page** → **Open in a pinned tab**.
3. Still nothing? Open one job on that site, look at its address, and put a part every job link shares (such as `/job/` or `/vacancy/`) into **Job link contains**.
</details>

<details><summary><b>The icon shows a grey "!"</b></summary>

A site couldn't be read. Open the popup to see which one, visit that site once to make sure you're logged in, then use **Test this page**.
</details>

<details><summary><b>"AI unavailable"</b></summary>

The key is wrong or empty, or your AI account is out of credit. Meanwhile it keeps barking for every new job, so you don't miss anything.
</details>

<details><summary><b>No notification pop-ups</b></summary>

Allow notifications for Google Chrome in **Windows Settings → System → Notifications**, or **macOS System Settings → Notifications**.
</details>

<details><summary><b>Chrome shows a "developer mode extensions" warning</b></summary>

This is normal for extensions installed from GitHub. Close the message (don't choose *Disable*) and Watch & Bark keeps working.
</details>

<details><summary><b>A site blocked me or shows a captcha</b></summary>

Check less often (3–10 minutes), keep **Vary the timing slightly** on, and solve the captcha yourself in a normal tab.
</details>

---

## 🔁 Updating to a new version

1. Download the new ZIP from this page and unzip it.
2. Go to `chrome://extensions` and click **Remove** on the old Watch & Bark.
3. Click **Load unpacked** and choose the new folder.

> To keep your sites and rules, first open **Settings → Backup & share → Export settings**, then **Import** them after updating.

---

## 📁 What's inside

| File | What it does |
|---|---|
| `manifest.json` | Extension details and permissions |
| `background.js` | Checks your job sites, runs the timers and page refresher, sends alerts |
| `extractor.js` | Finds the individual job links on a results page |
| `offscreen.html/js` | Plays the sounds and reads job pages in the background |
| `popup.html/js` | The window that opens from the toolbar |
| `options.html/js` | The Settings page |
| `help.html` | Built-in help & guide |
| `shared.js`, `style.css` | Shared settings and styles |

**Permissions used:** `alarms` and `storage` (timers and your settings), `notifications`, `offscreen` (sounds), `tabs` and `scripting` (page refresher and pinned-tab reading), and access to each website you add, asked for one site at a time.

---

## 🤝 Support

Found a problem or have an idea? Open an **Issue** on this page.

If Watch & Bark helped you, you can say thanks with a small donation through the **❤ Support** link inside the extension.

---

<p align="center">Made with 🐶 for job seekers. Good luck with your search!</p>
