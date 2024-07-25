---
layout: post
title: "Creating a Site or Blog Using Jekyll on GitHub Pages (Without Local Installation)"
date: 2024-07-26
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
For example, you can set the repository name to "blog".

#### 2. Set Up Jekyll on GitHub

Follow the steps below to set up Jekyll:

1. **Initialize the repository with Jekyll:**
You have to initialize the repository for Jekyll. Jekyll is a static site generator that uses markdown to generate sites so you would be creating a `.md` file for each page.

   - For a personal or organisation site, if you didn't add a README file when creating the repository, you can do so now by clicking "Add a README" on the repository main branch. The `README.md` file serves as your personal site/portfolio. You can skip this part if you are creating project pages like we are doing in this post. Jekyll uses `README.md` or `index.md` file as home page.
   - Create the necessary Jekyll files by clicking "Add file" > "Create new file" and then creating the neccessary files as described below.


2. **Create `_config.yml`:**
   
   `_config.yml` is the configuration file for your Jekyll site. Create this file in the root directory of your repository and add your site configuration.

     ```yml

     # Site title
     title: My GitHub Page

     # Site description
     description: This is my site hosted on GitHub Pages using Jekyll.

     # Theme to use (this uses the default Jekyll theme)
     theme: minima
     
     # Base URL of your site
     baseurl: "/my-blog" # For a personal or organization site, leave this blank - `baseurl: ""`. For a project site, set this to your "/<repository-name>"

     # URL of your site
     url: "https://godzuche.github.io" # Replace godzuche with your GitHub username

     # Permalink settings for blog posts
     permalink: /:year/:month/:day/:title/
     ```

3. **Create `index.md`:**
   
   `index.md` will be the main content file for your site. It is the home page of your site.
    Create this file in the root directory of your repository and add some initial content.

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
   
   1. Click on **Add file**
   2. Click on **Create new file**
   3. For the file name, use `_posts/` (Hurray! So easy! You just created _posts directory). Directories are created by appending `/` to the file name. Inside this directory you would create your first blog post.
   4. Once the directory is created, just enter a file name to create a new file.
   5. The name should be in this format: `YEAR-MONTH-DAY-title.md`. For example, 2024-07-26-my-first-post.md is a valid name for My First Post.
   6. Add the following content to the `2024-07-26-my-first-post.md` file:


```yml
---
layout: post
title: "My First Post"
date: 2024-07-26
---

This is my first blog post on my new Jekyll site! :)
```

#### 3. Commit and Push Your Changes

After adding your site content, commit and push your changes to GitHub. If you're editing directly on GitHub, save the changes.

Well done! 🙌 You have finished creating your beautiful site but one more step left - you need to make it go live by `hosting` it.

#### 4. Enable Github Pages (Hosting)

1. Go to the repository on GitHub.
2. Click on the "Settings" tab.
3. Scroll down to the "GitHub Pages" section.
4. Select the branch you want to use for GitHub Pages (usually main or gh-pages). This should be the branch that we want to host the pages.
5. Save the settings.

Awesome!🥳 Your site should be live at `https://<username>.github.io` or `https://<username>.github.io/<repository-name>` 
depending on the type of Github page you created as described in `step 1`. For our case, we use the `project pages` option so our site should be in this form: `https://<username>.github.io/<repository-name>`.

Now, you can share the `URL` to friends :)

### Customizing Your Site

**Themes:**
GitHub Pages supports various themes. You can change the theme by updating the `_config.yml` file and specifying a different theme. In this post, we used the `minima` theme.

**Custom Domain:**
You can use a custom domain for your GitHub Pages site. Follow the instructions here to set it up.

### Conclusion

Creating a site or blog using Jekyll on GitHub Pages is straightforward and does not require local installation. 
By following these steps, you can have your site up and running quickly. Happy coding! :)



   
