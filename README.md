# 🎀 Pookie — always-listening personal AI for Android

Say **"Pookie, call mom"** with the screen off. Pookie wakes up, thinks with Claude, and does it.

## Get the app on your phone (no computer needed)

1. Go to **github.com** → sign in → **New repository** → name it `pookie` → **Create**.
2. Upload every file and folder from this project (keep the folders, including `.github`).
   On a phone: *Add file → Upload files*. If your browser can't upload folders, use the zip method:
   open github.com on a PC once, or use the GitHub mobile app / "Desktop site" mode.
3. Open the **Actions** tab → wait ~5 minutes for **Build Pookie APK** to turn green ✅.
   (If it asks, click "I understand my workflows, enable them".)
4. Open the **Releases** section on the repo page → **Pookie (latest build)** → download `app-debug.apk`.
5. Open the downloaded file → allow "Install unknown apps" for your browser → Install.

## First-time setup in the app (5 minutes)

1. Paste your **Anthropic API key** (console.anthropic.com → API keys). Tap **Save**.
2. Tap the four permission buttons, one by one:
   1. microphone / calls / texts / contacts
   2. **Accessibility → Pookie → ON** (this lets Pookie tap, type and scroll in apps)
      *If it is greyed out:* tap "If step 2 is greyed out", then ⋮ (top right) → **Allow restricted settings**, and try again.
   3. display over other apps
   4. battery unrestricted (very important, or Android will kill Pookie)
3. Tap **▶ Start Pookie**. A small "Pookie" notification appears — that's the always-on listener.
4. Lock your phone and say: **"Pookie, what time is it?"**

## Better wake word (optional, recommended)

The default "basic mode" uses Android's speech recognition to hear "Pookie". It works, but can use more battery
and some phones make a small beep. For a proper, low-battery, offline wake word:

1. Make a free account at **console.picovoice.ai** and copy your **AccessKey**.
2. In the console go to **Porcupine** → create wake word **"Pookie"** (English) → platform **Android** → download the `.ppn` file.
3. In the app: paste the AccessKey, tap **Choose Pookie.ppn file**, pick the file, tap **Save**, then Stop and Start Pookie.

## What Pookie can do

Calls and SMS to your contacts · WhatsApp messages (opens chat and presses Send) · open any installed app ·
YouTube / Google search · navigation · timers and alarms · flashlight · volume · open Wi-Fi/Bluetooth/other settings ·
Home/Back/Recents/notifications/quick settings/lock/screenshot · read the screen, tap buttons by name, type text,
scroll and swipe in any app (multi-step tasks, up to 6 rounds) · answer anything.

## Honest limits

- A phone that is fully powered off can't listen. Screen off / locked is fine.
- Android won't let any app start a microphone service silently right after a reboot on newer versions:
  after restarting your phone, tap the "Tap to wake Pookie up" notification once (or open the app).
- Android shows the "Pookie is listening" notification at all times. That is required and can't be hidden.
- Pookie can't read your notifications or messages out loud yet, and is told never to do payments or delete data.
- Some phone brands (Xiaomi, Oppo, Vivo, Realme, Samsung) have extra battery managers. Set Pookie to
  "No restrictions" / "Autostart: on" / "Lock in recents" or they may kill it. See dontkillmyapp.com.
- This is a debug build for your own use. Your API key is stored only on your phone.
