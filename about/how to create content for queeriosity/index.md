---
title: "Contributing to Queeriosity"
weight: 1
draft: false
description: "This guide covers everything from forking the repository to submitting pull requests for contributing to Queeriosity."
tags: ["contributing", "content"]
authors:
  - "amanrathore"
---
<!-- Author: Aman Rathore
Contact: amanr.me | amanrathore9753 <at> gmail <dot> com
Created on: Monday, May 26, 2025 at 22:47 -->

> Drafted by [Aman Rathore](https://amanr.me) and then formatted by LLM and then checked by [Aman Rathore](https://amanr.me).

## Introduction

This guide walks you through contributing content to the [Queeriosity Website](https://queeriosity.github.io/) using Git, GitHub, and [Hugo](https://gohugo.io/).  
No prior experience is assumed—every step is explained.

## Methods to Contribute

### Email Submission
1. Send your blog or art files to [queeriosity01@gmail.com](mailto:queeriosity01@gmail.com).  
2. Include a brief description of your content.  
3. **Optional (but recommended):** Provide a few extra details to help us introduce you:
   - **Name:** Your full name (e.g. Aman Rathore)  
   - **Profile Image:** A link or path to your avatar like [this](https://amanr.me/images/me,%2020250313_162430_hu_8194b8e2508e8b74.jpeg). Direct JPEG or PNG also accepted.  
   - **Bio:** A short tagline or bio (e.g. Website Creator & Maintainer)  
   - **Social Links:**  
     - 🌐 Website: https://amanr.me  
     - ✉️ Email: amanrathore9753@gmail.com  
     - 💼 LinkedIn: https://linkedin.com/in/amanrathorep  
     - 🐙 GitHub: https://github.com/AmanRathoreP  
     - 📸 Instagram: https://instagram.com/aman__0864  
     - 📲 Telegram: https://t.me/aman0864  
      > If you have any other social media or platforms you want to share, feel free to include them!
     

### GitHub Web Interface

  1. Navigate to the `content/` folder in your fork, [reference](#2-clone-your-fork-locally).
  2. Click **Add file → Create new file** or edit existing files.
  3. Commit changes and open a PR as above.

### Git CLI (Command Line Interface)
> This is the recommended method for advanced users who prefer command-line tools and who plan to regularly contribute to [Queeriosity](https://queeriosity.github.io/).

#### Prerequisites

1. **Git** installed on your machine.  
   - Windows: [Git for Windows](https://gitforwindows.org/)  
   - macOS: `brew install git`  
   - Linux: `sudo apt install git` (Debian/Ubuntu)  
2. **Hugo** installed globally.  
   - See [Hugo Quickstart](https://gohugo.io/getting-started/installing/)  
3. A **GitHub account**.  

---

#### 1. Fork the Repository

1. Go to the [original repo](https://github.com/AmanRathoreP/Queeriosity-Website-Content)
2. Click **Fork** (top-right).  
3. Don't rename your fork if you are strictly following this guide.

---

#### 2. Clone Your Fork Locally

Open your terminal and run:

```bash
# Replace <your-username> with your GitHub handle
git clone "https://github.com/<your-username>/Queeriosity-Website-Content"
```
```bash
git clone -b deployment "https://github.com/Queeriosity/queeriosity.github.io"
cd queeriosity.github.io/
```

---

#### 3. Initialize Hugo & Submodules

If the project uses submodules, initialize them:

```bash
git submodule update --init --recursive
```

---

#### 4. Run Hugo Server

Launch Hugo’s live-reload server:

```bash
hugo server
```

* Open your browser at `http://localhost:1313/`
* Any edits under the `content/` folder auto-refresh.

---

#### 5. Add or Edit Content (First Time)

1. Navigate to `content/` directory.
2. Create or edit markdown files (`.md`) for your pages.
3. Preview locally via Hugo server to verify formatting.

---

#### 6. Add remote to your local repository

Navigate to your local repository folder of Queeriosity-Website-Content abd run the below command to add the remote repository:

```git
git remote add origin "https://github.com/<your-username>/Queeriosity-Website-Content"
```
---

#### 7. Place content in the main content repo folder

Once you are done with the changes, copy the content from `content/` folder in `queeriosity.github.io/` to `Queeriosity-Website-Content` 

> only for linux `cp -r -f content/* ../Queeriosity-Website-Content/`

then commit the changes in `Queeriosity-Website-Content` and push it to the remote repository

```git
git commit -a -m "Update content"
```
> - instead of just writing **Update content** please write something more descriptive about the changes you made.
> - Length of commit messages should less than 50 characters.

---

#### 8. Update Content (Subsequent Times)

When you return to add more content later just follow the [step 7](#7-place-content-in-the-main-content-repo-folder).

--- 

#### 9. Open a Pull Request

1. Go to your fork on GitHub.
2. You’ll see a banner: “Compare & pull request.” Click it.
3. Fill in:

   * **Title**: e.g. `Add new blog/art on X`
   * **Description**: Explain *why* and *what* you changed.
4. Submit the PR against the **original** `Queeriosity/queeriosity.github.io` repo, targeting the `deployment` branch.

Once the maintainers review and merge, your content will go live at [https://queeriosity.github.io/](https://queeriosity.github.io/).

---

## Best Practices & Tips

* **Branch per feature**: Isolate work for easier review.
* **Descriptive commit messages**: e.g. `Fix: typo in about-page.md`.
* **Preview often**: Use `hugo server` to catch formatting issues early.
* **Proofread your markdown**: Check headings, links, and images.

---

## Troubleshooting

| Issue                                  | Solution                                                        |
| -------------------------------------- | --------------------------------------------------------------- |
| Hugo server not starting               | Ensure Hugo is installed: `hugo version`                        |
| Merge conflicts when pulling upstream  | Resolve conflicts in your editor, then `git add` & `git commit` |
| Changes not showing in browser         | Clear cache or restart Hugo server                              |


## About Author
- Website: [amanr.me](https://amanr.me/)
- GitHub: [@AmanRathoreP](https://www.github.com/AmanRathoreP) | [@AmanRathoreM](https://www.github.com/AmanRathoreM)
- Telegram: [@aman0864](https://t.me/aman0864)
- Email: [aman.proj.rel@gmail.com](mailto:aman.proj.rel@gmail.com)
- LinkedIn: [@amanrathorep](https://www.linkedin.com/in/amanrathorep/)
- Instagram: [@aman__0864](https://www.instagram.com/aman__0864/)


### Credits
<a href="https://www.freepik.com/free-vector/abstract-background-with-colorful-geometric-shapes_1106978.htm#fromView=keyword&page=4&position=7&uuid=7a5d6f7f-3b53-40a3-8cc5-eb7165f32a43&query=Abstract+Svg">Image by kjpargeter on Freepik</a>