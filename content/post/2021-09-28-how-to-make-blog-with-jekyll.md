---
date: "2021-09-28T00:00:00Z"
image: "https://i1.wp.com/codelatte.org/wp-content/uploads/2018/11/github-jekyll.png"
subtitle: how to make blog with jekyll
tags:
- blog
- jekyll
title: how to make blog with jekyll
---

## Creating a Blog on GitHub Using Jekyll 

Jekyll is a website generator designed to create static blogs to host on GitHub Pages. Tom Preston-Werner created Jekyll to allow people to blog using a simple static HTML site, with all content hosted and version-controlled on GitHub. The goal is to remove the hassle of blogging platforms by creating workflows that enable blogging in a simpler way.

## How Does Jekyll Work?

Quoted from its official website, Jekyll allows us to create blogs easily and without using a database. All pages and posts will be converted to Static HTML so that it speeds up loading because there is no need to call the database.

Jekyll takes our content written in Markdown, delivers it via templates and deploys it as a static website, ready to serve. GitHub Pages easily serves websites directly from our GitHub repository, so you don't have to deal with any hosting.





In this article, we will learn how to create a blog on Github Pages using Jekyll. The process this time will be a little simpler than the others, because we will only do 4 steps, including:

1. Create a blog from Jekyll.

2.Host our Jekyll blog for free on GitHub.

3. Edit/custom blog such as name, avatar and social media links.
Publish our first post!

4. Publish our first post!

## Creating a Blog on GitHub Using Jekyll

note: if you don't have a github account, please create one first.


Visit [Jekyll Now](http://www.github.com/barryclark/jekyll-now), and hit the “Fork” button in the upper right corner of the repository to copy a copy of the blog theme to your GitHub account.

![contoh](https://i0.wp.com/cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/cddcf942-6cc7-4a1f-bf1b-5066b5e553ec/step1.gif)

As GitHub users, we are entitled to a free “user” website, which will be live at ```http://usernamegithub.github.io.``` This space is ideal for hosting a Jekyll blog! Next we need to rename the repository that we forked earlier to ```usernamegithub.github.io.```

![gambar](https://i1.wp.com/codelatte.org/wp-content/uploads/2018/11/Screen-Shot-2018-11-01-at-8.12.45-PM.png)

Your website will be live soon. You can check by going to your ```http://usernamegithub.github.io```

![hasil](https://i0.wp.com/codelatte.org/wp-content/uploads/2018/11/Screen-Shot-2018-11-01-at-8.15.18-PM.png)


## Customize Jekyll Blog

Now you can change the website name, description, avatar and other options by editing the file ```_config.yml.``` This custom variable has been set for convenience when your website is created.

Making changes to ```_config.yml``` (or any file in your repository) will force GitHub Pages to rebuild your website with Jekyll. The rebuilt website will be viewable a few seconds later at ```http://usernamegithub.github.io.``` 


