---
layout: post
title: "Creating a Site or Blog Using Jekyll on GitHub Pages (Without Local Installation)"
date: 2024-07-22
---

## Creating a Site or Blog Using Jekyll on GitHub Pages (Without Local Installation)

### Introduction

GitHub Pages allows you to host websites directly from your GitHub repositories, and Jekyll is a static site generator that's integrated with GitHub Pages. This guide will show you how to create a site or blog using Jekyll on GitHub Pages without needing to install Jekyll locally.

### Prerequisites

- A GitHub account. If you don't have one, you can sign up [here](https://github.com/join).
- Basic knowledge of GitHub and Markdown.

### Steps to Create a Site or Blog

#### 1. Create a Repository

Go to GitHub and create a new repository. The repository name will determine your site's URL.
  - If you name the repository `<username>.github.io`, it will be your personal website, and the URL will be `https://<username>.github.io`.
  - For project pages, you can name the repository anything you like, and the URL will be `https://<username>.github.io/<repository-name>`. We will be using this option for this post.

#### 2. Set Up Jekyll on GitHub

1. **Initialize the repository with Jekyll:**
   - If you didn't add a README file when creating the repository, you can do so now by clicking "Add a README" on the repository main page.
   - Create the necessary Jekyll files by clicking "Add file" > "Create new file" and then creating the following files:

2. **Create `_config.yml`:**
   - `_config.yml` is the configuration file for your Jekyll site. Create this file in the root directory of your repository and add your site configuration.

```yml
title: My GitHub Page
description: This is my site hosted on GitHub Pages using Jekyll.
theme: minima
```
3. **Create `index.md`:**
   - `index.md` will be the main content file for your site. Create this file in the root directory of your repository and add some initial content.

```yml
---
layout: default
title: Home
---

# Welcome to My GitHub Page

This is my site hosted on GitHub Pages using Jekyll.
```

4. **Create `_posts` directory and your first blog post:**
   Create a `_posts` directory in the root of your repository. This directory is akin to a path or folder in your File Explorer. It is where you would be creating your blog posts.
   - Click on **Add file**
   - Click on **Create new file**
   - For the file name, use `_posts/` (Hurray! So easy! You just created _posts directory). Directories are created by appending `/` to the file name.
   Inside this directory you would create your first blog post.
   - Once the directory is created, just enter a file name to create a new file.
   - The name should be in this format: `YEAR-MONTH-DAY-title.md`. For example, 2024-07-22-my-first-post.md is a valid name for My First Post.
   Add the following content to the `2024-07-22-my-first-post.md` file:
```yml
---
layout: post
title: "My First Post"
date: 2024-07-22
---

This is my first blog post on my new Jekyll site! :)
```

#### 3. Commit and Push Your Changes

After adding your site content, commit and push your changes to GitHub. If you're editing directly on GitHub, save the changes.

#### 4. Enable Github Pages

1. Go to the repository on GitHub.
2. Click on the "Settings" tab.
3. Scroll down to the "GitHub Pages" section.
4. Select the branch you want to use for GitHub Pages (usually main or gh-pages). This should be the branch that we want to host the pages.
5. Save the settings.

Your site should be live at `https://<username>.github.io` or `https://<username>.github.io/<repository-name>`.

### Customizing Your Site

**Themes:**
GitHub Pages supports various themes. You can change the theme by updating the `_config.yml` file and specifying a different theme. In this post, we used the `minima` theme.

**Custom Domain:**
You can use a custom domain for your GitHub Pages site. Follow the instructions here to set it up.

### Conclusion

Creating a site or blog using Jekyll on GitHub Pages is straightforward and does not require local installation. By following these steps, you can have your site up and running quickly. Happy coding! :)



   
