# 🛠️ GitHub Profile Kit - Developer Instructions

Welcome to your premium, recruiter-quality GitHub Profile Kit, Sumit! This guide will walk you through the quick process of deploying this profile to your GitHub and customizing it as your projects evolve.

---

## 📂 Kit Structure
This kit contains the following production-ready assets:
*   📂 `assets/`
    *   🎨 `header_banner.svg`: A responsive, self-contained SVG header with built-in CSS typing animations, glowing mesh points, and active recruiter status.
    *   🎨 `divider.svg`: A sleek gradient horizontal rule with a centering pulse pulse animation to structure your profile.
*   📄 `README.md`: The primary markdown profile containing a 2-column resume layout, customized single-theme skill badges, structured project cards, and unified Git analytics.

---

## 🚀 Step 1: Create Your Profile Repository
To activate a profile README on your GitHub:
1.  Go to [GitHub New Repository](https://github.com/new).
2.  In the **Repository name** field, type your exact GitHub username: `sumitprajapatismr`.
3.  GitHub will display a special notice: *"You found a secret! sumitprajapatismr/sumitprajapatismr is a special repository..."*
4.  Set the repository visibility to **Public** (required for the profile to appear).
5.  Check **Initialize this repository with a README** (you will replace its content in the next step).
6.  Click **Create repository**.

---

## 📤 Step 2: Upload Your Profile Kit
You can upload these files using the GitHub Web UI or your command-line terminal:

### Option A: Using the Command Line (Recommended)
Open your terminal in this directory (`github-profile-kit`) and execute these commands:
```bash
# Initialize a local git repository if not already done
git init

# Add the files in this kit
git add README.md assets/

# Commit the additions
git commit -m "feat: deploy premium profile kit"

# Rename branch to main
git branch -M main

# Add your GitHub repository as the remote origin
git remote add origin https://github.com/sumitprajapatismr/sumitprajapatismr.git

# Push changes (force-pushing will overwrite any existing boilerplate README)
git push -u origin main --force
```

### Option B: Using the GitHub Website
1.  Navigate to your repository at `https://github.com/sumitprajapatismr/sumitprajapatismr`.
2.  Click on the **Add file** dropdown button and select **Upload files**.
3.  Drag and drop the `README.md` and the `assets` folder into the upload zone.
4.  Enter a commit message (e.g. `Deploy portfolio theme`) and click **Commit changes**.

---

## ⚙️ Step 3: Verify & Optimize Stats
The analytics dashboard uses open-source rendering widgets. Ensure you have made some public contributions for the metrics to populate accurately:
1.  **GitHub Stats & Language Card:** Rendered via `github-readme-stats`. They are pre-themed with background `#0a0f1d`, title `#00f0ff` (neon blue), and text `#a0aec0` to match your banner.
2.  **GitHub Streak Stats:** Rendered via `github-readme-streak-stats` to showcase consecutive days of commits.

If any widget does not render, wait a few seconds and refresh. The services compile caches upon initial requests.

---

## 🎨 Customizing Content In the Future
*   **Modifying Project Details:** Edit the HTML `<table>` section in the `README.md`. Each project is encapsulated in a `<td width="50%">` cell. You can swap descriptions, add screenshots, or update repository hyperlinks.
*   **Updating Badge Colors:** All tech stack badges are generated using Shields.io with custom parameters. You can change their appearance by modifying the query string. For instance, `logoColor=00f0ff` forces the icons to glow cyan.
*   **Editing the Header Subtitle:** The typing animation in `assets/header_banner.svg` is self-contained. To change the typed subtitle, edit the `<text>` element in the SVG file and adjust the `<animate>` tag width accordingly (monospace font characters are roughly 10px wide).
