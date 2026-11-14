# From Labs to Bullets: Lite

**Track your labs. Get hired.**

A lab tracker for IT students. Log each hands-on lab as you finish it, then turn your labs into resume bullets, a training summary, and interview stories.

👉 **Open the app:** https://from-labs-to-bullets.github.io/From-Labs-to-Bullets-Lite/

> **Lite vs. the full app.** The full *From Labs to Bullets* app also has class notes, study prompts (Listener, Examiner, Refresh), Friday weekly reviews, and mock interview logs. **Lite keeps only the career side:** lab tracking, lab notes, the three career prompts, the PDF training record, and the GitHub portfolio.

---

## What it does

Over 17 weeks of IT technical training, students complete close to 100 virtual labs. From Labs to Bullets: Lite helps them keep a record of that work and put it to use.

1. **Log each lab right after you finish it (Monday to Thursday),** while the title and details are fresh. Everything saves as you type.
2. **Turn your labs into career material.** Generate prompts for resume bullets, a training summary, and interview stories (STAR) from everything you've logged.
3. **Export your training** as a private PDF training record and a public-ready GitHub portfolio.

## The lab log

The **Today** screen has one required question for the day, plus a section for each lab.

**Course or module:** choose it from the list (or add a new one).

1. How many labs have you completed so far today? Raise the number after each lab, and a new section appears for it. Enter 0 on days without labs.

For each lab:

- **Lab title** (paste it from your lab platform)
- **2.** What did you build, configure, deploy, or automate in the virtual lab, and what specific technologies or tools did you use to accomplish it? *(action-word chips, a description, and technology tags)*
- **3.** How did the environment or solution function after you completed the lab, and what business or technical objective did your setup achieve? What problem were you trying to solve?
- **4.** What was the scope of the lab environment, including the number of systems, devices, accounts, or automation scripts you configured? *(with examples for each area of the program)*
- **Lab notes** *(optional)*: key steps, commands, settings, or a problem you hit and how you fixed it. Troubleshooting notes make strong interview stories.

Click **Save day** when you're done. If a required answer is missing, the app lists it and jumps to it.

**Labs that span two days:** log the lab on the day you finish it.

**Fridays:** there's no class, so Today shows **Week at a glance** to catch up on missed days. It also offers a shortcut to turn the week's labs into bullets, and a backup reminder.

**Week 9 (Pro-Dev Week):** week 9 is always dedicated to professional development, so the app doesn't track it.

## Summaries & bullets

The app writes the prompts and the student pastes them into their own AI tool (Microsoft Copilot, ChatGPT, Claude, Gemini, and others). The app itself never contacts an AI service.

Each prompt can cover all of training, a single week, a course, or a date range, and includes every lab answer and the lab notes.

### Resume bullets

Bullets use this format: **Action + Technology + Purpose**

- **Action:** start with what you did (built, configured, deployed, automated).
- **Technology:** name the specific tools you used.
- **Purpose:** finish with what the setup accomplished.

*Example:* Configured Azure Virtual Networks and Network Security Groups to segment workloads and block unauthorized inbound traffic.

The prompt tells the AI to use only facts from the student's labs, never invent numbers or results, and present the work as hands-on training rather than job experience. Students can save the bullets they like inside the app.

### Training summary and interview stories

- **Training summary:** an overview, skills grouped by area, key labs, and next steps to explore on Microsoft Learn.
- **Interview stories:** 3 to 5 stories in STAR format (Situation, Task, Action, Result), each with two interview questions it answers well.

## Exporting your training

On the **Summaries & bullets** tab, **Export your training** creates two files from whatever is chosen under **What to include**:

- **Training record (PDF):** every lab, including lab notes and saved bullets, in a clean printable layout. Click **Create PDF**, then choose **Save as PDF** in the print window. This file is private. To edit it, open the PDF in Microsoft Word.
- **GitHub portfolio (README.md):** labs, technologies, and saved resume bullets, formatted for GitHub. It leaves out lab notes, because it's meant to be public. Technologies are grouped by what they do (Cloud & Virtualization, Server & Identity, Networking & Security, Automation & Operations, DevOps & Version Control, Endpoint Management, AI), with anything unrecognized under Other tools. Instructors can adjust the groups in `SKILL_RULES` in `index.html`.

## Your data stays on your computer

- **No accounts, no sign-in, no server.** Everything is saved in your web browser, on your own computer.
- **Nobody else can see your entries,** including your instructor and the people who maintain this repository.
- **Turn on auto-save.** The last setup step asks students to choose a file, ideally in their **OneDrive** folder. The app then saves the diary to that file every time they type.
- **Edge asks for permission during the first few visits.** Click **Resume auto-save**, then **Allow**. When Edge offers **Allow on every visit**, choose it.
- **Browser data cleared, or a new computer?** Choose **I already have a diary file** (or **Open my diary file** in **Settings & backup**) and pick the file.
- **Use Microsoft Edge on your computer.** Auto-save works in Edge and Chrome on a computer, not in Firefox, Safari, or on phones. Don't use InPrivate windows.
- **Without auto-save, download a backup every Friday** from **Settings & backup**.

### Using Lite alongside the full app

Lite keeps its data completely separate from the full app, even in the same browser. It uses its own storage, its own auto-save file (`My lab diary (Lite).json`), and its own backup files.

- **Bringing labs over from the full app:** in Lite, use **Restore from a backup file** and choose a full-app backup or diary file. Lite copies the labs and saved bullets. Class notes, study material, weekly reviews, and mock interviews are left out. The original file is never changed.
- **Lite never auto-saves into a full-app diary file.** If a student picks one by mistake, Lite refuses and explains why, so their class notes are never lost.

## Getting started (students)

1. Open the app link above in Microsoft Edge and bookmark it.
2. Enter your training start date.
3. Turn on auto-save and save your diary file in your OneDrive folder.
4. After each lab, open **Today**, raise the number of labs, and fill in the new lab section.
5. Whenever you like (Fridays are a good time), open **Summaries & bullets**, copy a prompt, and paste it into your AI tool.

## For instructors

### Publishing the app

The whole app is a single file, `index.html`.

The app is published from the public repository [From-Labs-to-Bullets/From-Labs-to-Bullets-Lite](https://github.com/From-Labs-to-Bullets/From-Labs-to-Bullets-Lite).

1. Upload `index.html` and this `README.md` to the repository.
2. In the repository, open **Settings**, then **Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
3. After a minute or two, the app is live at https://from-labs-to-bullets.github.io/From-Labs-to-Bullets-Lite/.

To publish an update, click **Add file**, then **Upload files**, drag in the new `index.html`, and click **Commit changes**. Students' saved entries are not affected.

> **Keep the same web address.** Each student's entries are tied to the app's exact URL. If the app moves, students must download a backup from the old address and restore it at the new one.

### Course list

The **Course or module** list is preloaded with:

- AZ-040: Automating Administration with PowerShell
- GH-900: GitHub Foundations
- Windows Server: Installation, Storage and Compute
- Windows Server: Networking
- Windows Server: Identity
- Linux Administration Fundamentals (Ubuntu)
- AZ-900: Azure Fundamentals
- AI-901: Microsoft Azure AI Fundamentals
- AZ-400: DevOps Solutions
- MD-102: Endpoint Administrator
- AZ-104: Azure Administrator
- SC-300: Identity and Access Administrator

Students can add a course with **+ Add a new course…** in the dropdown, or edit the list in **Settings & backup**. To change the default list for a new cohort, edit `DEFAULT_COURSES` near the top of the script in `index.html`.

### Lab lists

No lab list is built in, because labs can change from one cohort to the next. Students paste each lab's title from their lab platform. The app remembers the technologies each student enters and suggests them next time.

## Technical details

- A single, self-contained HTML file (HTML, CSS, and JavaScript). There is no build step, and it uses no external libraries.
- Data is stored in the browser's `localStorage` under `fltb-lite.v1`. Backups and the auto-save file are plain JSON files marked `"app": "fltb-lite"`.
- Auto-save uses the browser's File System Access API (Edge and Chrome on a computer). The file's location is remembered in IndexedDB (`fltb-lite-files`). On startup, the app compares the file with the browser copy and keeps the newer one. Nothing is sent to a server.
- The app asks the browser for persistent storage, so the browser won't remove its data on its own when disk space runs low.
- Designed for Microsoft Edge on Windows. The rest of the app also works in Chrome, Firefox, and Safari, but auto-save is only available in Edge and Chrome.
- Supports light and dark mode automatically.
