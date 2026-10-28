# 🚨 DivyaDrishti - Smart Helmet Emergency Lifeline & Anti-Snoop Security Gateway

A zero-dependency, mobile-first static emergency web portal hosted **100% free forever on GitHub Pages**. 
Accessed by scanning the physical **QR code sticker on the rider's smart helmet or motorbike fuel tank**.

---

## 🔒 Security & Privacy Architecture: Solving the Parked Helmet Dilemma

### The Problem:
If a rider parks their motorcycle outside a market or office and leaves their helmet on the bike, curious strangers or stalkers could scan the helmet QR sticker to extract the rider's personal home address, mobile number, and medical allergies. Conversely, in a real life-threatening crash, a rescuer cannot be delayed by passwords or 2FA OTPs when the rider is unconscious.

### The Solution (Dual-Zone Security Model):

```text
┌────────────────────────────────────────────────────────────────────────┐
│                        ZONE 1: PUBLIC SHIELD VIEW                      │
│                  (Default view when anyone scans QR)                   │
├────────────────────────────────────────────────────────────────────────┤
│ • Name Masked: "Sahana S****"                                          │
│ • Vehicle Masked: "Honda Activa (KA 28 ****)"                          │
│ • Blood Group: A+ (Public for Emergency Transfusion)                   │
│ • Home Address: 🔒 BLURRED & PROTECTED                                  │
│ • Critical Drug Allergies: 🔒 BLURRED & PROTECTED                       │
│ • Family Contact: Masked (+91 843171****)                              │
│                                                                        │
│ 🛡️ ANTI-SNOOP GUARD (ZERO DIALER LEAKS):                                │
│   - [🔒 Unlock to Call Family]: Locked against casual clicks!          │
│     Clicking it prompts for PIN / Witness check; NEVER leaks number!   │
│   - [🚑 Call 108 Ambulance]: Always 100% active for anyone              │
│   - [🏥 Locate Nearest Hospital via GPS]: Always 100% active           │
└────────────────────────────────────────────────────────────────────────┘
                                    │
           ┌────────────────────────┴────────────────────────┐
           ▼                                                 ▼
┌──────────────────────────────────────┐  ┌──────────────────────────────┐
│  PATHWAY A: 🚨 Real Crash Rescuer    │  │ PATHWAY B: 🔐 Rider/Medic    │
│  "Accident Witness / Good Samaritan" │  │ "4-Digit PIN Unlock"         │
├──────────────────────────────────────┤  ├──────────────────────────────┤
│ • Zero Passwords Needed (<3 seconds) │  │ • Fast 4-digit PIN (2881)    │
│ • Validates rescuer 10-digit mobile  │  │ • Client-side SHA-256 hash   │
│ • Captures live crash GPS pin        │  │ • Unlocks All Clinical Data  │
│ • Unlocks Drug Allergies & Dossier   │  │ • Unlocks Full Home Address  │
│ • Unlocks Direct Call to Family      │  │ • Unlocks Direct Family Call │
│ • Formats 1-Click WhatsApp SOS       │  │ • Custom QR sticker creation │
└──────────────────────────────────────┘  └──────────────────────────────┘
```

---

## ⚡ How It Works in Real Scenarios

### Scenario 1: Curious Stranger Scans Parked Helmet on Bike
1. Stranger scans QR code with smartphone.
2. The portal loads **Zone 1: Privacy Shield Active**.
3. Home address is blurred (`Protected by DivyaDrishti Security`), phone number is masked (`+91 843171****`), and full name is masked.
4. **Critical Drug Allergies & Clinical Directives are locked and blurred** to prevent snooping on private health conditions.
5. **No Dialer Leak**: If the stranger taps "🔒 UNLOCK TO CALL RIDER'S FAMILY", the portal displays a floating security toast and scrolls to the verification card. It **does NOT open the phone dialer**, ensuring the private phone number is never leaked to a stranger's phone keypad!
6. If they attempt to unlock, a prominent **Legal Warning (Indian Good Samaritan Act & BNS Section 419/420)** warns them that unauthorized access of unattended personal property is monitored with live GPS coordinates.

### Scenario 2: Severe Highway Crash (Unconscious Rider & Paramedics)
1. Good Samaritan or paramedic arrives at the crash scene and scans the helmet QR sticker.
2. Blood group (`A+`) is immediately visible for trauma blood matching.
3. Good Samaritan enters their mobile number and taps **"CONFIRM REAL CRASH & UNLOCK MEDICAL ALLERGIES"** (or enters rider's 4-digit PIN `2881`):
   - Instantly unlocks the **Paramedic Medical Dossier**:
     - `⚠️ CRITICAL DRUG ALLERGIES: NO PENICILLIN, SULFA DRUGS, OR NSAIDS / ASPIRIN` (prevents fatal anaphylaxis or hemorrhage).
     - `Pre-Existing Conditions: Bronchial Asthma (Carries Inhaler), Type-1 Diabetic`.
     - `Trauma Directives: Do NOT administer blood thinners. Keep cervical spine immobilized.`
   - Instantly unlocks the family's direct phone number and turns the button green: **"CALL RIDER'S FAMILY DIRECTLY (+91 8431712890)"**.
   - Rescuer taps the button to speak directly with the guardian while ambulance is en route!
   - Pre-fills a comprehensive **1-Click WhatsApp Lifeline Message** containing rider vitals, witness contact, and a direct Google Maps pin link!

---

## 🚀 Progressive Web App (PWA) & Offline Capabilities

The portal includes full **Progressive Web App (PWA)** capabilities, making it ideal for GitHub Pages hosting:

- **Offline Loading (`sw.js`)**: Caches core application assets (`index.html`, `logo.jpg`, `manifest.json`, and CDN scripts). If the QR code is scanned in an area with weak or zero cellular reception, the portal loads immediately from the browser cache.
- **Homescreen Installation (`manifest.json` + `icons/`)**: Can be installed onto any Android or iOS device as a standalone native app icon with full-screen presentation.
- **Offline Cellular SMS Fallback**: In rural or mountainous areas where 4G/5G mobile internet is unavailable (preventing WhatsApp), the **"📱 SEND OFFLINE EMERGENCY SMS"** button uses native `sms:` protocol to pre-fill an emergency text with GPS coordinates and vital allergies, dispatched directly over 2G cellular towers with zero mobile data required!

---

## 🌐 Multilingual Accessibility (English / ಕನ್ನಡ / हिंदी)

To ensure that bystanders across India can immediately understand and act during high-stress triage, the portal includes an instant, client-side language switcher:

- **English (Default)**: Universal international first-responder format.
- **Kannada (ಕನ್ನಡ)**: Tailored for local bystanders and Karnataka emergency services.
- **Hindi (हिंदी)**: Broad accessibility across National Highway corridors and North Indian transit routes.
- **Spoken Audio Voice Guidance (Web Speech API)**: Panicked bystanders can tap **"🔊 Spoken First-Aid Voice Guidance"** to hear calming, step-by-step synthesized audio instructions in their selected language (*"Stay calm. Tap 108 for ambulance. Keep helmet on unless breathing is blocked..."*).

---

## 📁 Repository Structure for GitHub Pages

```text
emergency-portal/
├── index.html        # PWA-enabled responsive multilingual portal with Dual-Zone security
├── manifest.json     # Web App Manifest for mobile installation
├── sw.js             # Offline Service Worker with stale-while-revalidate caching
├── logo.jpg          # DivyaDrishti smart helmet visual identity
├── icons/            # PWA application icons
│   ├── icon-192.png  # 192x192 maskable icon
│   └── icon-512.png  # 512x512 maskable icon
└── README.md         # Architecture, deployment guide, and security documentation
```

---

## 🚀 How to Make Live on GitHub Pages ($0.00 Free Tier)

1. **Push to Your GitHub Repository:**
   ```bash
   git add emergency-portal/
   git commit -m "Add Anti-Snoop Security and Emergency Gateway to Lifeline Portal"
   git push origin main
   ```
2. **Enable GitHub Pages:**
   - In GitHub: Go to your repository -> **Settings** -> **Pages**.
   - Under **Build and deployment** -> **Source**: Select `Deploy from a branch`.
   - Branch: `main` / Folder: `/emergency-portal` (or root).
   - Click **Save**.
3. **Your Live Public URL:**
   - GitHub Pages will activate your live HTTPS link:
     `https://<your-username>.github.io/<repo-name>/emergency-portal/`
4. **Print Weatherproof Helmet QR Sticker:**
   - Open your live link on a mobile or PC browser.
   - Expand the **"Print Weatherproof Helmet QR Code Sticker"** section.
   - Download the generated QR code sticker and print it as a 2×2 inch vinyl sticker for your helmet!

---

## 🛠️ Dynamic URL Query & Encrypted Hash Parameters

Supports both clean URL parameters and Base64 `#data=` hash obfuscation:

### Standard Parameters:
```text
https://<username>.github.io/.../emergency-portal/?name=Sahana&phone=8431712890&blood=A%2B&vehicle=KA-28-HM-8281&address=Karmudi%2C%20Koppal
```

### Encrypted / Obfuscated Hash (Recommended for Helmet QR Code):
```text
https://<username>.github.io/.../emergency-portal/#data=eyJuYW1lIjoiU2FoYW5hIiwicGhvbmUiOiI4NDMxNzEyODkwIiwiYmxvb2QiOiJBKyJ9
```

| Parameter | Description | Default Demo Value |
| :--- | :--- | :--- |
| `name` | Full name of rider | `Sahana` |
| `phone` | 10-digit family phone number | `8431712890` |
| `blood` | Blood group | `A+` |
| `vehicle` | Vehicle make & registration | `Honda Activa ( KA 28 HM 8281 )` |
| `address` | Home residence | `Karmudi, Koppal District, Karnataka.` |
| `guardian`| Role of emergency contact | `Father / Guardian` |

---

## 🛡️ Security & Privacy Compliance
- **Zero Server Tracking:** 100% client-side Web Crypto API execution (`crypto.subtle.digest`). Zero user data is stored on third-party tracking databases.
- **Good Samaritan Legal Protection:** Cites Section 134A of the Indian Motor Vehicles Act to eliminate fear of police harassment for rescuers.
- **Session Expiry:** Unlocked records automatically re-lock after 30 minutes in `sessionStorage`.
