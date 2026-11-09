# kairos schedule bot

A study planner that builds students' study schedules around their classes, work, and life. Everything runs in the student's own browser: plans are saved on their device, and nothing is sent to a server.

## What's in this folder

| File | What it does |
|---|---|
| `index.html` | The planner itself |
| `manifest.webmanifest` | Lets students add the planner to their phone's home screen |
| `sw.js` | Lets the planner open without an internet connection |
| `icons/` | The app icon |
| `README.md` | This guide |

Keep all of these together. The planner works without the extra files, but students can't install it on their phones or use it offline.

---

## Put it online with GitHub Pages (about 15 minutes, free)

### 1. Make a GitHub account

Go to [github.com/signup](https://github.com/signup). Your username becomes part of the planner's web address (for example, `drc-teaches.github.io/kairos`), so pick something you're happy for students to see.

### 2. Create a repository

A repository ("repo") is a folder on GitHub.

1. Click the **+** in the top-right corner, then **New repository**.
2. **Repository name:** `kairos` (this becomes the end of the web address).
3. Choose **Public**. GitHub Pages is free only for public repositories. People can see the planner's code, but never students' plans, which stay on their own devices.
4. Click **Create repository**.

### 3. Upload the files

1. On the new repository's page, click the **uploading an existing file** link.
2. Unzip the folder you downloaded. Select **everything inside it**, including the `icons` folder, and drag it onto the upload area. (Drag the files themselves, not the folder that contains them.)
3. Check that the list shows `index.html`, `manifest.webmanifest`, `sw.js`, `README.md`, and four files starting with `icons/`.
4. Scroll down and click **Commit changes**.

### 4. Turn on GitHub Pages

1. In the repository, click **Settings** (top menu), then **Pages** (left menu).
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to **main** and the folder to **/ (root)**, then click **Save**.
4. Wait a minute or two and refresh the page. A box appears at the top saying **Your site is live at** a web address. That's the link for students.

### 5. Check it

- Open the link in a **private or incognito window**. It should open with the tutorial and work without any sign-in.
- On your phone, open the link and add it to your home screen:
  - **iPhone (Safari):** tap the Share button, then **Add to Home Screen**.
  - **Android (Chrome):** tap the ⋮ menu, then **Add to Home screen** or **Install app**.

---

## Making changes later

**Small text changes** (wording, a link, the campus help lists):

1. In the repository, click `index.html`, then the pencil icon (**Edit this file**).
2. Use Ctrl+F (Cmd+F on a Mac) in your browser to find the text, change it, and click **Commit changes**.
3. The live site updates within a few minutes. Students get the new version the next time they open it online.

**Replacing the whole planner** (for example, a new version from Claude):

1. Click **Add file**, then **Upload files**, and drag in the new `index.html`.
2. Click **Commit changes**. GitHub replaces the old file.

Students' saved plans aren't affected by updates. They live in each student's browser, not in these files.

---

## Good to know

- **Each student's plan is saved only in the browser they use.** To use the planner on another device, they follow **Settings → Use kairos on another device** inside the planner.
- **Clearing browser data erases the plan.** The planner reminds students to make backups.
- **PDF and Word syllabus import** loads small reading tools from the internet the first time it's used, so it needs a connection. Everything else works offline once the planner has been opened once.
- **The Claude syllabus reader isn't in this version.** The planner finds dates with its own pattern matching, so students should check the review screen carefully.
- **The feedback button** opens the Microsoft Form linked in `index.html`. To change it, search the file for `FEEDBACK_URL`.
