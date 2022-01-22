---
sidebar_position: 3
---

# Edit the handbook locally

## Introduction

This is a guide on what you'll need to install and run a local development environment on your machine so you can make
edits locally. This allows you a better overview and preview when making complex changes.

Once you're set up, you will find the source files for the SEF
Handbook [in the sef-handbook repo](https://github.com/sef-global/sef-handbook)

:::tip

When you only need to make small or quick changes, the Web IDE may be easier or faster than the local development
environment.

:::

### Help is available for team members

If you work for SEF, we don't expect you to figure this out by yourself. If you have questions, ask anyone for help or
post in the `#handbook` Slack channel. You're more likely to have success with:

- People that have been here longer than 3 months.
- People that have 'engineer' in their title.

### 1. Start using GitHub

Here's where you can find step-by-step guides on
the [basics of working with Git and GitHub](https://docs.github.com/en/get-started/quickstart). You'll need those later.

### 2. Install Git

1. Open a terminal.
1. Check your Git version by executing: `git --version`.
1. If Git is not installed, you should be prompted to install it. Follow
   this [guide](https://docs.github.com/en/get-started/quickstart/set-up-git) to installing Git and linking your account
   to Git.

### 3. Installing Node.js

1. Download the installer from [Node.js WebSite](https://nodejs.org/en/download/). (The version should be >= 14 or
   above)
2. Run the installer.
3. Follow the installer steps, agree the license agreement and click the next button.

### 4. Clone the source of the website

There are two ways to clone this repository: ssh or https. You only need to choose one.

#### Clone via SSH

The GitHub documentation covers how to setup SSH keys. If you haven't already done this - or aren't sure - read through
the [GitHub SSH docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh). When you have your SSH
keys [added to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account):

1. In a terminal, execute: `git clone git@github.com:sef-global/sef-handbook.git` to clone the website.

#### Clone via HTTPS

If you prefer using https, then:

1. In a terminal, execute: `git clone https://github.com/sef-global/sef-handbook.git`

#### 5. Preview website changes locally

1. In a terminal, execute:
    1. Change to the directory for your site, for example: `cd sites/sef-handbook`
    1. `npm start`
1. Visit http://localhost:3000 in your browser.

#### 6. Start contributing

The pages are located in the `docs` directory. Most pages that you might want to edit are written
in [markdown](https://www.markdownguide.org/basic-syntax/). Read through the [Docusaurus' Markdown features guide](https://docusaurus.io/docs/markdown-features) to understand its syntax and
create new content. Follow [Docusaurus' Docs guide](https://docusaurus.io/docs/docs-introduction) for
more information on creating new pages.

#### 7. Test if all URL links in a page are valid

Run `npm run build` command on your terminal.

It will tell you how many links, if any, are invalid. Fix any invalid links and ideally any warnings.

All internal links (links leading to other parts of the website) should be relative.

