# 📱 Mifos Mobile 7.0 – Internship Progress Report - 2025 

<p align="center">
  <img src="https://img.shields.io/badge/Internship-Mifos%20Initiative-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Duration-12%20Weeks-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Ongoing-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/PRs%20Merged-✔️%2045+-informational?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Tech-Kotlin%20Multiplatform%20%7C%20Compose%20Multiplatform-orange?style=for-the-badge" />
</p>  

---

## 🔗 Quick Links  

- 📂 **All Pull Requests** → [View on GitHub](https://github.com/openMF/mifos-mobile/pulls/Nagarjuna0033)  
- 📌 **Jira Board** → [View Tasks](https://mifosforge.jira.com/jira/software/c/projects/MM/boards/65?assignee=712020%3A5519b873-099b-42e4-b415-5d8562d644a6)  
- 𝕏 **Updates** → [Follow me](https://twitter.com/arjun3_b)  
- 💻 **GitHub Profile** → [@Nagarjuna0033](https://github.com/Nagarjuna0033)

---

## 📌 Description  

An open-source mobile banking application powered by the Mifos Initiative, designed to enhance financial inclusion by providing unbanked and underbanked populations seamless access to banking services. It offers account management, loan applications and repayments, savings and deposits management, fund transfers, and transaction tracking through integration with the Mifos X backend via RESTful APIs.  

Targeted primarily at emerging markets, Mifos-Mobile empowers users to conveniently manage finances, even in remote areas, while actively supported by a global community dedicated to extending and improving digital financial services.  

---

<a id="tech-stack"></a>  
## 🛠️ Tech Stack  
The project is built on modern, cross-platform technologies ensuring scalability, maintainability, and performance.  

| **Category**             | **Technology / Framework** | **Purpose** |
|---------------------------|----------------------------|-------------|
| **Language**              | Kotlin (Multiplatform)     | Shared business logic across Android, iOS, Desktop |
| **UI Framework**          | Compose Multiplatform, Jetpack Compose | Declarative UI for all platforms |
| **Architecture**          | MVI (Model-View-Intent)   | Unidirectional state management with clear separation of concerns |
| **Networking**            | Ktor + Ktorfit            | Type-safe HTTP client for API requests |
| **Asynchronous Handling** | Kotlin Coroutines + Flows | Structured concurrency and reactive streams |
| **Dependency Injection**  | Koin                      | Lightweight DI framework for modular and testable code |
| **Database**              | Room (Multiplatform migration) | Local persistence and caching |
| **Serialization**         | Kotlinx Serialization     | JSON parsing and serialization |
| **Image Loading**         | Coil                      | Efficient image loading and caching |
| **Barcode/QR Scanning**   | ML Kit                    | QR and barcode recognition |
| **Design System**         | Material 3 + Custom Mifos Design System | Consistent UI/UX across the app |
| **CI/CD**                 | GitHub Actions            | Automated builds, linting, and deployment |
| **Project Management**    | Jira + GitHub Projects    | Issue tracking, sprint planning, progress tracking |

---

<a id="goals--mid-point-milestone"></a>  
## 🎯 Goals & Mid-Point Milestone  

**Goals**  
1. **Scheduled Payments** – Allow users to schedule recurring payments and transfers.  
2. **Transaction Categorization** – Automatic categorization of expenses for better financial tracking.  
3. **Redesign Dashboard with given Figma designs & Customizable Dashboard** – Let users arrange and prioritize frequently used features.  
4. **In-App Customer Support** – Real-time chat and customer support for immediate user assistance.  
5. **Cross-Platform Release** – Launch the app on iOS and Desktop platforms.  

---

<a id="weekly-progress"></a>  
## 📅 Weekly Progress  

| Week | Dates | Focus Area | Key Deliverables | PRs Opened |
|------|--------|------------|------------------|------------|
| [1](#week-1-1st--6th-june) | 1–6 Jun | Codebase exploration & Loan migration | Explored architecture, migrated loan feature, reviews | 1 |
| [2](#week-2-7th--13th-june) | 7–13 Jun | Loan module (android-client) | Testing research, CMP migration | 2 |
| [3](#week-3-14th--20th-june) | 14–20 Jun | Loan module (merge) | Finalized loan migration, design discussions | 1 |
| [4](#week-4-21st--27th-june) | 21–27 Jun | Theming & Components | Setup theme/typography, created base components | 4 |
| [5](#week-5-28th--4th-july) | 28 Jun–4 Jul | Auth Screens | Onboarding, Login, Status components | 3 |
| [6](#week-6-5th--11th-july) | 5–11 Jul | Auth Flow + Sprint 1 | Signup, OTP, Password reset | 5 |
| [7](#week-7-12th--18th-july) | 12–18 Jul | Sprint 2 start | Home dashboard, navigation fixes | 2 |
| [8](#week-8-19th--25th-july) | 19–25 Jul | Sprint 2 | Passcode & Savings UI | 4 |
| [9](#week-9-26th-jul--1st-aug) | 26 Jul–1 Aug | Sprint 2–3 | Account UIs & Loan modules | 8 |
| [10](#week-10-2nd--8th-aug) | 2–8 Aug | Sprint 3–4 | Loan Apply, Transactions, Settings | 9 |
| [11](#week-11-9th--15th-aug) | 9–15 Aug | Sprint 5–6 | Loan product flows & docs upload | 5 |
| [12](#week-12-16th--22nd-aug) | 16–22 Aug | Share & Transfers | Share account + Third Party transfer | 7 |
| [13](#week-13-23rd--29th-aug) | 23-29 Augh | Clean up modules | Focused on **loan module improvements**, **UI consistency**, and **authentication enhancements** | 14 |
---

## 📂 Detailed Weekly Progress  



<details id="week-1-1st--6th-june">
<summary>📌 Week 1 (1st – 6th June)</summary>

**Summary**  
- Explored `openmf/mifos-mobile` codebase architecture (network, data, model, feature layers).  
- Studied Kotlin Multiplatform + Compose Multiplatform setup.  
- Cross-referenced proposal deliverables with current architecture.  
- Migrated loan feature in `android-client`.  
- Reviewed PRs: [#2399](https://github.com/openMF/android-client/pull/2399), [#2396](https://github.com/openMF/android-client/pull/2396)

**Pull Requests**  
- [#2404](https://github.com/openMF/android-client/pull/2404) – feat(feature:loan): migrate to CMP  

</details>

---

<details id="week-2-7th--13th-june">
<summary>📌 Week 2 (7th – 13th June)</summary>

**Summary**  
- Continued work on loan module migration in `android-client`.  
- Explored Unit/UI testing approaches.  
- Reviewed PRs:  
  [#2402](https://github.com/openMF/android-client/pull/2402),  
  [#2403](https://github.com/openMF/android-client/pull/2403),  
  [#2396](https://github.com/openMF/android-client/pull/2396),  
  [#2394](https://github.com/openMF/android-client/pull/2394),  
  [#2391](https://github.com/openMF/android-client/pull/2391),  
  [#2369](https://github.com/openMF/android-client/pull/2369),  
  [#2382](https://github.com/openMF/android-client/pull/2382)

**Pull Requests**  
- [#2400](https://github.com/openMF/android-client/pull/2400) – refactor(feature:path-tracking): migrate to CMP  
- [#2401](https://github.com/openMF/android-client/pull/2401) – [draft] refactor(feature:client): migrate to CMP  

</details>

---

<details id="week-3-14th--20th-june">
<summary>📌 Week 3 (14th – 20th June)</summary>

**Summary**  
- Completed migration of loan module.  
- Discussed blockers (image rendering in client screen).  
- Synced with mentor & UI/UX team on new designs.  
- Reviewed PRs:  
  [#2402](https://github.com/openMF/android-client/pull/2402),  
  [#2403](https://github.com/openMF/android-client/pull/2403),  
  [#2408](https://github.com/openMF/android-client/pull/2408)

</details>

---

<details id="week-4-21st--27th-june">
<summary>📌 Week 4 (21st – 27th June)</summary>

**Summary**  
- Setup **theme and typography**.  
- Built first UI components.  
- Collaborated with design team on mockups.  
- Reviewed PRs:  
  [#2418](https://github.com/openMF/android-client/pull/2418),  
  [#2419](https://github.com/openMF/android-client/pull/2419),  
  [#2416](https://github.com/openMF/android-client/pull/2416),  
  [#2414](https://github.com/openMF/android-client/pull/2414),  
  [#2413](https://github.com/openMF/android-client/pull/2413),  
  [#2412](https://github.com/openMF/android-client/pull/2412),  
  [#2411](https://github.com/openMF/android-client/pull/2411),  
  [#2410](https://github.com/openMF/android-client/pull/2410)

**Pull Requests**  
- [#2846](https://github.com/openMF/mifos-mobile/pull/2846) – feat: setup theme and typography  
- [#2847](https://github.com/openMF/mifos-mobile/pull/2847) – refactor: radio button component  
- [#2848](https://github.com/openMF/mifos-mobile/pull/2848) – feat: customized card  
- [#2849](https://github.com/openMF/mifos-mobile/pull/2849) – feat: uploaded state component  

</details>

---

<details id="week-5-28th--4th-july">
<summary>📌 Week 5 (28th June – 4th July)</summary>

**Summary**  
- Designed **Onboarding language screen** + logic in ViewModel.  
- Built **Login screen** + logic in ViewModel.  
- Designed **Status component**.  
- Reviewed android-client PRs:  
  [#2427](https://github.com/openMF/android-client/pull/2427),  
  [#2425](https://github.com/openMF/android-client/pull/2425),  
  [#2423](https://github.com/openMF/android-client/pull/2423),  
  [#2422](https://github.com/openMF/android-client/pull/2422),  
  [#2421](https://github.com/openMF/android-client/pull/2421),  
  [#2420](https://github.com/openMF/android-client/pull/2420)

**Pull Requests**  
- [#2850](https://github.com/openMF/mifos-mobile/pull/2850) – feat: onboarding language screen ui & viewModel  
- [#2851](https://github.com/openMF/mifos-mobile/pull/2851) – feat: sign in ui & viewModel  
- [#2852](https://github.com/openMF/mifos-mobile/pull/2852) – feat: status component  

</details>

---

<details id="week-6-5th--11th-july">
<summary>📌 Week 6 (5th – 11th July)</summary>

**Summary**  
- Completed Sprint 1 Figma designs.  
- Cleaned auth module.  
- Reviewed PRs in android-client & mobile-wallet:  
  [#2432](https://github.com/openMF/android-client/pull/2432),  
  [#2429](https://github.com/openMF/android-client/pull/2429),  
  [#2426](https://github.com/openMF/android-client/pull/2426),  
  [#2428](https://github.com/openMF/android-client/pull/2428),  
  [#2433](https://github.com/openMF/android-client/pull/2433),  
  [#1878](https://github.com/openMF/mobile-wallet/pull/1878)

**Pull Requests**  
- [#2853](https://github.com/openMF/mifos-mobile/pull/2853) – feat: sign up ui & viewModel  
- [#2854](https://github.com/openMF/mifos-mobile/pull/2854) – feat: upload id ui & viewModel  
- [#2855](https://github.com/openMF/mifos-mobile/pull/2855) – feat: otp authentication ui & viewModel  
- [#2856](https://github.com/openMF/mifos-mobile/pull/2856) – feat: recover password ui & viewModel  
- [#2857](https://github.com/openMF/mifos-mobile/pull/2857) – feat: set new password ui & viewModel  

</details>

---

<details id="week-7-12th--18th-july">
<summary>📌 Week 7 (12th – 18th July)</summary>

**Summary**  
- Started Sprint 2 mockups.  
- Fixed desktop build issue.  
- Designed Home Dashboard + navigation fixes.  

**Pull Requests**  
- [#2859](https://github.com/openMF/mifos-mobile/pull/2859) – fix: compose plugin version & navigation  
- [#2860](https://github.com/openMF/mifos-mobile/pull/2860) – feat: home ui & viewModel  

</details>

---

<details id="week-8-19th--25th-july">
<summary>📌 Week 8 (19th – 25th July)</summary>

**Summary**  
- Continued Sprint 2 mockups.  

**Pull Requests**  
- [#2861](https://github.com/openMF/mifos-mobile/pull/2861) – feat: passcode ui & viewModel  
- [#2862](https://github.com/openMF/mifos-mobile/pull/2862) – feat: savings account ui & viewModel  
- [#2865](https://github.com/openMF/mifos-mobile/pull/2865) – feat: savings account filters & generic account module  
- [#2868](https://github.com/openMF/mifos-mobile/pull/2868) – refactor: signup flow  

</details>

---

<details id="week-9-26th-jul--1st-aug">
<summary>📌 Week 9 (26th Jul – 1st Aug)</summary>

**Summary**  
- Completed Sprint 2 mockups, started Sprint 3.  

**Pull Requests**  
- [#2870](https://github.com/openMF/mifos-mobile/pull/2870) – feat: account label card  
- [#2872](https://github.com/openMF/mifos-mobile/pull/2872) – feat: account details ui & viewModel  
- [#2875](https://github.com/openMF/mifos-mobile/pull/2875) – feat: update account ui & viewModel  
- [#2879](https://github.com/openMF/mifos-mobile/pull/2879) – feat: loan account ui & viewModel  
- [#2880](https://github.com/openMF/mifos-mobile/pull/2880) – refactor: bound dashboard services with screens  
- [#2883](https://github.com/openMF/mifos-mobile/pull/2883) – refactor: integrate savings transfer & deposit flow  
- [#2888](https://github.com/openMF/mifos-mobile/pull/2888) – feat: loan account summary  
- [#2892](https://github.com/openMF/mifos-mobile/pull/2892) – feat: loan repayment schedule  

</details>

---

<details id="week-10-2nd--8th-aug">
<summary>📌 Week 10 (2nd – 8th Aug)</summary>

**Summary**  
- Completed Sprint 3–4 mockups.  
- Progressed towards core goals (Figma, Transaction categorization, iOS/Desktop pipelines, Scheduled Payments).  

**Pull Requests**  
- [#2897](https://github.com/openMF/mifos-mobile/pull/2897) – feat: complete loan apply flow with validation  
- [#2898](https://github.com/openMF/mifos-mobile/pull/2898) – feat: recent transactions  
- [#2901](https://github.com/openMF/mifos-mobile/pull/2901) – feat: qr code reader screen  
- [#2902](https://github.com/openMF/mifos-mobile/pull/2902) – refactor: beneficiary details for qr code generation  
- [#2903](https://github.com/openMF/mifos-mobile/pull/2903) – refactor: removed redundant card components  
- [#2904](https://github.com/openMF/mifos-mobile/pull/2904) – refactor: apis setup for receiving server messages  
- [#2906](https://github.com/openMF/mifos-mobile/pull/2906) – refactor: account top bar title  
- [#2910](https://github.com/openMF/mifos-mobile/pull/2910) – feat: settings ui  
- [#2914](https://github.com/openMF/mifos-mobile/pull/2914) – feat: logout  

</details>

---

<details id="week-11-9th--15th-aug">
<summary>📌 Week 11 (9th – 15th Aug)</summary>

**Summary**  
- Completed Sprint 5–6 mockups.  

**Pull Requests**  
- [#2918](https://github.com/openMF/mifos-mobile/pull/2918) – feat: language update  
- [#2923](https://github.com/openMF/mifos-mobile/pull/2923) – feat: loan product selection  
- [#2924](https://github.com/openMF/mifos-mobile/pull/2924) – feat: loan product details  
- [#2926](https://github.com/openMF/mifos-mobile/pull/2926) – refactor: connected loan product details & application form  
- [#2929](https://github.com/openMF/mifos-mobile/pull/2929) – feat: upload documents for loan  

</details>

---

<details id="week-12-16th--22nd-aug">
<summary>📌 Week 12 (16th – 22nd Aug)</summary>

**Summary**  
- Completed **Third Party Transfer** & **Share account application flow**.  

**Pull Requests**  
- [#2937](https://github.com/openMF/mifos-mobile/pull/2937) – chore: remove unused modules  
- [#2938](https://github.com/openMF/mifos-mobile/pull/2938) – feat: savings application & enhance home navigation  
- [#2939](https://github.com/openMF/mifos-mobile/pull/2939) – refactor: home dashboard internet handling  
- [#2940](https://github.com/openMF/mifos-mobile/pull/2940) – refactor: logout dialog  
- [#2941](https://github.com/openMF/mifos-mobile/pull/2941) – feat: fill savings application  
- [#2942](https://github.com/openMF/mifos-mobile/pull/2942) – feat: share application details  
- [#2943](https://github.com/openMF/mifos-mobile/pull/2943) – feat: additional details for share account application  
- [#2944](https://github.com/openMF/mifos-mobile/pull/2944) – feat: third party transfer ui & viewModel  

</details>

---

<details id="week-13-23rd--29th-aug">
<summary>📌 Week 13 (23rd – 29th Aug)</summary>

**Summary**  
- Focused on **loan module improvements**, **UI consistency**, and **authentication enhancements**.  
- Fixed multiple Android build issues and updated theme support.  

**Pull Requests**  
- [#2947](https://github.com/openMF/mifos-mobile/pull/2947) – refactor: made remarks field mandatory & enhance state handling  
- [#2948](https://github.com/openMF/mifos-mobile/pull/2948) – refactor: text field  
- [#2949](https://github.com/openMF/mifos-mobile/pull/2949) – refactor: rounding amount to decimals  
- [#2950](https://github.com/openMF/mifos-mobile/pull/2950) – refactor: loan repayment schedule with prepopulated data  
- [#2951](https://github.com/openMF/mifos-mobile/pull/2951) – refactor: use first name instead of username for better readability  
- [#2952](https://github.com/openMF/mifos-mobile/pull/2952) – refactor(loan): show consistent loan actions for all account statuses  
- [#2953](https://github.com/openMF/mifos-mobile/pull/2953) – refactor: make middle name optional  
- [#2954](https://github.com/openMF/mifos-mobile/pull/2954) – refactor: navigation after transfers, update, withdraw  
- [#2955](https://github.com/openMF/mifos-mobile/pull/2955) – refactor: make transfer handling  
- [#2956](https://github.com/openMF/mifos-mobile/pull/2956) – feat: updating theme  
- [#2957](https://github.com/openMF/mifos-mobile/pull/2957) – refactor: auth module with loading animation  
- [#2959](https://github.com/openMF/mifos-mobile/pull/2959) – refactor(loan-application): dialogs  
- [#2960](https://github.com/openMF/mifos-mobile/pull/2960) – fix: android build  
- [#2962](https://github.com/openMF/mifos-mobile/pull/2962) – fix: android build  

</details>

<a id="key-learnings"></a>  
## 📖 Key Learnings  

- Migration to **Kotlin Multiplatform** and **Compose Multiplatform**.  
- Designing modular UI with **Figma → Compose MVI** workflow.  
- Implementing **end-to-end banking features** (loan, savings, share, transfers).  
- Writing cross-platform **auth, onboarding, and navigation flows**.  
- Improving developer experience with **refactors & CI/CD pipelines**.  

---

<p align="center">
  <em>📌 This is a <strong>living blog</strong> – progress updates are continuously added.  
  Click on the ▸ arrow buttons above to view weekly details.</em>  
</p>
