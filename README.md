\# 🛡️ Amanix: Real-Time Digital Footprint Risk Analyzer



\*\*Amanix\*\* is a privacy-first browser extension and gamified platform designed to protect teenagers from unintentional data leaks and digital footprint risks on social media platforms (such as Threads and Reddit). 



Developed as a Final Year Project (FYP) at the International Islamic University Malaysia (IIUM).



\---



\## 🚀 Key Features



\* \*\*Real-Time Pattern Detection:\*\* Automatically scans text inputs for sensitive data categories using advanced regular expressions:

&#x20; \* IC / MyKad numbers (`\*\*\*\*\*\*-\*\*-\*\*\*\*`)

&#x20; \* Phone numbers (`\*\*\*-\*\*\*\*\*\*\*`)

&#x20; \* School and campus names (`\[SCHOOL REDACTED]`)

&#x20; \* Physical addresses and live check-ins (`\[LOCATION REDACTED]`)

&#x20; \* Email addresses and `@usernames`

\* \*\*Mosaic Privacy Risk Calculation:\*\* Evaluates cumulative low-risk indicators (e.g., combining school name + birth date + phone number) and applies a danger score bonus to flag multi-faceted exposure.

\* \*\*Friction-Based Nudge Interventions:\*\* High-risk posts trigger funny, relatable meme reaction popups and cooling-off periods to encourage mindful posting habits.

\* \*\*Gamified Rewards Store:\*\* Users earn points and streaks by safely masking data, which can be redeemed for real-world commercial perks (e.g., free campus coffee or beverage vouchers), driving positive behavioral change.

\* \*\*Anonymized Admin Dashboard:\*\* Allows system administrators to monitor overall platform efficacy, total masks applied, and engagement metrics via fully anonymized user IDs (`User\_001`, `User\_002`) to ensure strict teen privacy.



\---



\## 🛠️ Tech Stack



\* \*\*Core:\*\* JavaScript (ES6+), HTML5, CSS3

\* \*\*Extension Architecture:\*\* Manifest V3 (`content\_test.js`, `background.js`, `Manifest.json`)

\* \*\*Data Storage:\*\* `chrome.storage.local` for local, secure state persistence



\---



\## 📦 Installation \& Setup (For Evaluation)



1\. \*\*Clone or Download\*\* this repository to your local machine.

2\. Open Google Chrome and navigate to \*\*`chrome://extensions/`\*\*.

3\. In the top-right corner, enable \*\*Developer mode\*\*.

4\. Click the \*\*Load unpacked\*\* button in the top-left corner.

5\. Select your local `amanix-extension` folder.

6\. Pin Amanix to your toolbar and navigate to supported platforms like Threads or Reddit to test detection!



\---



\## 📂 Project Structure



```text

amanix-extension/

├── Manifest.json         # Extension configuration (Manifest V3)

├── content\_test.js       # Core regex scanning \& DOM masking logic

├── background.js         # Service worker background script

├── dashboard.html        # User rewards \& progress dashboard

├── dashboard.js          # User state \& point redemption logic

├── admin.html            # Anonymized system admin monitoring panel

├── admin.js              # Admin metrics \& aggregated data loader

├── evaluation.html       # Evaluation metrics interface

├── login.html            # User authentication interface

├── login.js              # Authentication logic

├── popup.html            # Extension popup menu

├── styles\_test.css       # Extension stylesheet

├── amanix\_logo.png       # Amanix brand logo

└── \*.gif                 # Reaction meme GIFs for Nudge interventions

