# Google Sites & Play Store Deployment Guide

**Created for:** Rahel Baig Moghal  
**Location:** `/home/alamgir/Development/website/`  
**Associated Profiles:**
- **LinkedIn:** [linkedin.com/in/rahel-baig-moghal-a49948222](https://www.linkedin.com/in/rahel-baig-moghal-a49948222/)
- **GitHub:** [github.com/Rahel-Baig-Moghal](https://github.com/Rahel-Baig-Moghal)
- **Primary Support Email:** `rahelbaig1@gmail.com`
- **Flagship App:** **Fahm: Quranic Vocabulary** (`com.rahel.fahm`)

---

## 🚀 Two Ways to Build on Google Sites

### Method A: The Instant 1-Click Embed (Recommended & Modern)
Google Sites allows full HTML/CSS/JS embedding:
1. Go to [Google Sites](https://sites.google.com/) and create a **Blank** site.
2. In the right sidebar under **Insert**, click **`<> Embed`**.
3. Select the **Embed code** tab.
4. Copy the entire content of `/home/alamgir/Development/website/index.html` and paste it in.
5. Click **Next** and **Insert**.
6. Expand the embedded card borders so it occupies full width and length.
7. Click **Publish** at top right (e.g. choose site name `rahelbaigmoghal`).

---

### Method B: Native Google Sites Pages (Clean Multi-Page Structure)
If you prefer distinct Google Sites pages, create these pages in the **Pages** tab:

```text
├── Home (Developer Portfolio & Cloud Engineering Showcase)
├── Fahm (Fahm App Showcase & Feature Deep-Dive)
├── Privacy Policy (Mandatory for Google Play Console)
└── Support & Terms (Mandatory for Google Play Console)
```

---

## 📋 Copy & Paste Content for Native Google Sites Pages

### 1. Home Page (`/`)
* **Page Header:**
  * **Title:** Rahel Baig Moghal
  * **Subtitle:** Senior Cloud Architect &middot; AWS Serverless Specialist &middot; Mobile App Creator
* **About / Hero Section:**
  > Architecting resilient AWS cloud solutions, enterprise contact centers with Amazon Connect, and shipping purpose-driven, offline-first mobile applications.
* **Core Competencies (4-Column Layout):**
  1. **Amazon Connect & Telephony:** Enterprise contact flow routing, omnichannel customer journeys, Amazon Lex conversational AI, and real-time agent workspaces.
  2. **AWS Serverless & IaC:** Production Lambda pipelines, DynamoDB single-table design, API Gateway (REST/WebSockets), Aurora Serverless, and AWS SAM CI/CD.
  3. **Offline-First Mobile Development:** React Native iOS & Android development, encrypted local persistence (SQLite/MMKV), and privacy-preserving architectures.
  4. **AI & High-Leverage Engineering:** Harnessing cutting-edge LLMs for automated generational workflows and agentic tooling.
* **Featured Software:** Direct card linking to `/fahm`.
* **Experience & Certifications:**
  * SDE at **ConnectGen, Inc.** (Winner of the *Jack of All Trades* Award)
  * **AWS Certified Cloud Practitioner** & **Amazon Connect Developer Specialist**

---

### 2. Fahm App Page (`/fahm`)
* **Header Title:** Fahm: Quranic Vocabulary (`com.rahel.fahm`)
* **Tagline:** Master the divine words with an offline-first learning companion structured into 170 progressive mastery levels.
* **Key Features:**
  * **170 Progressive Retention Levels:** Systematically curated from high-frequency Quranic nouns and verbs to root meanings.
  * **100% Offline-First:** `android.permission.INTERNET` is explicitly blocked. Works completely without cellular data or Wi-Fi.
  * **Zero Ads, Zero Distractions:** Pure focus designed for spiritual and linguistic study.
  * **Local On-Device SQLite Storage:** All progress and spaced-repetition schedules live safely on your device (`user_progress.db`) with native JSON export/import.
* **Buttons:**
  * [Download on Google Play Store]
  * [Privacy Policy](/privacy-policy)
  * [Support & FAQ](/support)

---

### 3. Privacy Policy Page (`/privacy-policy`) &mdash; *CRITICAL FOR GOOGLE PLAY*
Google Play requires a live, accessible Privacy Policy URL matching the app manifest and permissions:

* **Header:** Privacy Policy for Fahm: Quranic Vocabulary
* **Effective Date:** October 17, 2026
* **Key Policy Clauses:**
  1. **Zero Data Collection:** We do not collect, store, transmit, or share any personal information, account credentials, device identifiers, location data, or usage analytics.
  2. **Zero Internet Permissions:** `android.permission.INTERNET` is explicitly blocked in the app's production manifest.
  3. **Local On-Device Storage:** All user learning streaks, levels, and settings reside in `user_progress.db` on your device. Users can export/import JSON backups or purge all data via app settings.
  4. **Local Notifications:** Daily reminders are scheduled strictly on-device using local OS alarms; no remote push tokens or servers are used.
  5. **Children's Privacy (Google Play Families Policy & COPPA):** Our app is educational, contains zero ads, collects zero data, and is safe for learners of all ages.
  6. **Developer Contact:**  
     * Name: Rahel Baig Moghal  
     * Email: `rahelbaig1@gmail.com`  
     * GitHub: `https://github.com/Rahel-Baig-Moghal` (Private Repository)

---

### 4. Support & Terms Page (`/support`)
* **Title:** App Support & Frequently Asked Questions
* **Contact Email:** `rahelbaig1@gmail.com` (Response SLA: 24–48 hours)
* **FAQ:**
  * *Q: Does Fahm require internet to work?*  
    *A: No, internet permission is blocked. All 170 levels are packaged on-device.*
  * *Q: Where is my study progress stored?*  
    *A: In local SQLite database `user_progress.db`. It never leaves your phone.*
  * *Q: How do I back up my progress?*  
    *A: Export an encrypted JSON file directly from the Profile screen.*
* **Terms Summary:** Personal educational license; all software rights reserved.

---

## 🎯 Google Play Console Submission Inputs

When publishing **Fahm** in Google Play Console, use these exact links:

| Console Field | Value to Input |
|---|---|
| **App Support Website** | `https://sites.google.com/view/<your-site-name>#support` (or `/support`) |
| **Support Email** | `rahelbaig1@gmail.com` |
| **Privacy Policy URL** | `https://sites.google.com/view/<your-site-name>#privacy` (or `/privacy-policy`) |
| **Developer Website** | `https://sites.google.com/view/<your-site-name>` |
| **Target Audience / Families** | Yes (Educational, All Ages) |
| **Data Safety Form** | Select **"No data collected"** & **"No data shared"** |

---

## 💼 LinkedIn Integration

1. **Profile Contact Info:**
   - Go to your LinkedIn profile: `https://www.linkedin.com/in/rahel-baig-moghal-a49948222/`
   - Click the pencil icon on your intro card -> **Contact Info** -> **Add Website**.
   - URL: `https://sites.google.com/view/<your-site-name>`
   - Label: `Portfolio & Apps (Fahm, AWS Cloud)`
2. **Featured Section:**
   - Add a link to your Google Site:  
     *"Creator of Fahm: Quranic Vocabulary & AWS Cloud Architect | Portfolio"*
