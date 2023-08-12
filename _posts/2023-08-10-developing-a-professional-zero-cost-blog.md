---
layout: markdown-page
title: Developing a professional zero cost blog
permalink: /developing_a_professional_zero_cost_blog
published: True
date: 2023-08-10
category: Productivity
categoryurl: ./productivity
categorycolor: warning
tags: Blog
excerpt: "Developing a professional, zero cost blog is now easier than ever thanks to these tools and services. This is the exact roadmap I used to create this blog, and you can do it to."
author: PBTL Team
authorimg: ./assets/images/favicon.ico
readtime: 30 min read
previewimg: ./assets/images/posts/4by3/female-typing-laptop.jpg
backgroundimg: ./assets/images/posts/4by3/female-typing-laptop.jpg
flagship: True
featured: False
---

## Getting started

In order to successfully make it through this guide, a very basic level of coding knowledge is recommended. Alternatively, if you are willing to learn on the go that's also fine! If you have some familarity with excel formulas, visual basic, html or other languages it will be smooth sailing. You can always use AI services like [ChatGPT](https://chat.openai.com/) to assist you.

If you have never seen a line of code in your life and are absolutely not interested, then you might be out of luck for the zero cost blog. In this case, I'd recommend using one of the services below to begin your blogging journey (albiet at a slightly higher price point).

>1. [Ghost](https://ghost.org/)
>2. [WordPress (Hosted)](https://wordpress.com/)
>3. [WordPress (Self-hosted)](https://wordpress.org/)
>4. [Blogger](https://www.blogger.com/)
>5. [Tumblr](https://www.tumblr.com/)
>6. [Medium](https://medium.com/)
>7. [Squarespace](https://www.squarespace.com/)

All up, getting through this guide and setting up a simple blog website should take about 30-60 minutes.

## Workflow tools

#### GitHub

Head over to [GitHub](https://github.com/) and sign up. GitHub is a web-based platform for version control and collaborative software development. It's what we are going to use to manage and deploy our blog website. Also download and install [Github Desktop](https://desktop.github.com/). This will allow us to easily manage version control locally on our computer.

#### Visual Studio Code

[Visual Studio Code](https://code.visualstudio.com/) is a free, highly customizable code editor developed by Microsoft for programming and web development. Download and install this so we can build and test our website.

## Building the most simple website

GitHub Pages is a static site hosting service from GitHub that takes HTML, CSS, and JavaScript files straight from a repository on GitHub, optionally runs the files through a build process, and publishes a website.

#### Create a repository

From GitHub, [create a new public repository](https://github.com/new) named **username.github.io**, where username is your username (or organization name) on GitHub. This is where all your website content will be stored online.

![create a new public repository](https://pages.github.com/images/user-repo@2x.png){:width="600px"}

#### Clone the repository to your computer

This is so we can make changes to our blog in our chosen code editor (Visual Studio Code) and preview changes to the website locally before committing them. To do this click the "Set up in Desktop" button. When the GitHub desktop app opens, save the project. You can use the default locations suggested by GitHub Desktop.

![set up in desktop](https://pages.github.com/images/setup-in-desktop@2x.png){:width="600px"}

#### Create an index file

An "index.html" file is the primary entry point for a web browser to display the content of a website, written in HTML (Hypertext Markup Language). From GitHub Desktop click on **"Open in Visual Studio Code**". From here create a new file in the repository called "index.html" and copy in the follow code as an example. Save the file.

    <!DOCTYPE html>
    <html>
    <body>
    <h1>Hello World</h1>
    <p>I'm hosted with GitHub Pages.</p>
    </body>
    </html>

![visual studio code create index file](./assets/images/posts/screensnips/visual-studio-index-file.png){:width="800px"}

#### Commit and publish
Enter the repository, commit your changes, and press the publish button to send your index.html file back to GitHub …and you're done! Fire up a browser and go to https://username.github.io

![commit and publish](https://pages.github.com/images/desktop-demo@2x.gif){:width="600px"}

And that's the most simple version of our website. So how do we go from something basic looking to a clean professional look? We'll cover this and how to add functionality to your blog below.

## Styling and functionality

#### Templates

To build up our blog with functionality and styling I suggest starting with a template. We could go and start coding all the styling ourself, and it's a good idea to try this sometime to get a basic idea of the HTML syntax. Starting with a template will also help you to ensure you website looks suitable on mobile devices.

You can get a nice clean free blog template from [startbootstrap](https://startbootstrap.com/theme/clean-blog-jekyll). You can find the [source code](https://github.com/startbootstrap/startbootstrap-clean-blog-jekyll) and additional instructions on GitHub. Download this template and copy paste the entire contents into your repository.

![simple-blog-template](https://assets.startbootstrap.com/img/screenshots/themes/clean-blog-jekyll.png){:width="800px"}

If you want something a bit fancier you can browse other websites or purchase a professionally designed HTML template. If you want to go down this path (which can save you a lot of time) I would recommend to look at [Bootstrap Themes](https://themes.getbootstrap.com/).

Reading up a little on the below will help you to best modify your blog.

#### Jekyll
By default GitHub pages uses [Jekyll](https://jekyllrb.com/) to serve your website content. Jekyll is a static site generator, commonly used for creating simple, fast, and secure websites. It takes plain text content and transforms it into static HTML pages, making it easy to manage and host websites without the need for a complex content management system (CMS) or a dynamic server. It's popular among developers and bloggers for its simplicity and efficiency.


#### Bootstrap
[Bootstrap](https://getbootstrap.com/) is a widely used front-end framework for building responsive and visually appealing websites and web applications. It provides a set of pre-designed HTML, CSS, and JavaScript components that help developers create consistent, mobile-friendly user interfaces. Bootstrap simplifies the process of designing and structuring web content, making it a popular choice for developers seeking to streamline the development of modern and responsive websites.

#### Markdown
Markdown is a lightweight markup language that simplifies the formatting of plain text content. It's commonly used for writing documentation, web content, and even simple formatted notes. Markdown uses simple and intuitive syntax (such as using asterisks for emphasis, hashtags for headings, and square brackets for links) to indicate formatting elements like headings, lists, links, and more. It's widely supported on various platforms, making it a popular choice for creating structured yet easy-to-read documents. Read the style guide [here](https://www.markdownguide.org/).

You don't need to be an expert in any of these, but knowing roughly what they do will allow you to edit and tinker with your website as needed to achieve the results you want.

## Installing Jekyll and previewing your website locally
This can sometimes be a bit tricky but if you perservere this will be the final hurdle. Follow the [install instructions](https://jekyllrb.com/docs/) on the Jekyll website depending on your operating system.

Once you have installed Jekyll, from your repository in Visual Studio Code, open a new terminal. "Terminal" -> "New Terminal". Try either one of the following to start the local web server.

    $ jekyll serve

    $ gem exec jekyll serve

If this suceeds then head to **http://127.0.0.1:4000** to preview your website locally.

## Recommendations
A few tips and tricks that I would recommend. Learn how to use the following Jekyll tools (ask ChatGPT to explain each one)

1. includes
2. layouts
3. posts

By using includes and layouts this will let you author your posts in markdown (.md) which you can preview the formatted version in Visual Studio Code as you author your posts.

## Conclusions
That covers the basic framework for your blog. We won't go into all the details on how to edit every component of the blog, please use all the links provided above and AI to assist you with this. Don't feel intimated if this all feels too foreign, the learning curve is pretty past and if you stick at it for a day or two you will be well on your way.