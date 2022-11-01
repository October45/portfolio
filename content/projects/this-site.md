---
title: "This Site"
date: 2022-10-31T23:45:04+02:00
description: "How I built this site, the site you are currently watching."
image: "https://d33wubrfki0l68.cloudfront.net/c38c7334cc3f23585738e40334284fddcaf03d5e/2e17c/images/hugo-logo-wide.svg"
type: "post"
tags: ["projects", "hugo", "webdev"]
showTableOfContents: true
draft: false
---

# Building this site

The story of how I built this site is a short story spread out over a long time.
I've wanted a portfolio site to display me and my work ever since I started learning web development for real. The hardest challange was always how and where to start.

## Backstory

### Why Hugo?

[![Hugo Logo](https://d33wubrfki0l68.cloudfront.net/c38c7334cc3f23585738e40334284fddcaf03d5e/2e17c/images/hugo-logo-wide.svg)](https://www.gohugo.io/)

First of all, let's look at why I chose Hugo as my way of developing this site, the main reason was really as simple as: I wanted to try something new.
After some research I found out that it was a static site generator, built in Go which I'm currently learning at grit:lab, which seemed to fit perfectly.

### Previous experiences

I knew that I liked writing my content in Markdown, and that if I ever wanted to add something new to it, it would be much easier in a "blog" type of way.
I've previously written websites in raw HTML+CSS, some including JS and others using PHP and MySQL for some database labbing.
But doing that for a portfolio/blog site seemed boring and tedious.

Then I had the idea of using Django in Python, which is what we used in school when learning Python, but I did not really like it as I didn't really understand it.
Then we used React for our final project in school, and it was easy to develop in, and I liked it.
But I didn't really want to use it for a portfolio site, as it would be both overkill and too hard to add new content to.

### How I found Hugo

After thinking about my portfolio site for a long while on and off I suddenly found a Youtuber ([ChrisTitusTech](https://www.youtube.com/christitustech)) that I started to like really much.
He had a blog which he posted articles on for every video that he made, which I found interesting how he found the time and energy to do it.
But then he published a video on how he did it, and suddenly I had found what seemed like the perfect way to build my site.

[![ChrisTitusTech](https://christitus.com/images/2022-thumbs/stop-using-apt.jpg)](https://www.christitus.com)

## Building the site

### The first steps

I started by watching the video that [ChrisTitusTech](https://www.youtube.com/christitustech) made on how he built his site, and then I started using the [article](https://christitus.com/how-i-setup-my-website/) he wrote for that video.
He used a theme that I did't find fitting for my purposes, so I started looking for a new one.
I went through several different themes, before I found one that I liked: [Gokarna](https://themes.gohugo.io/gokarna/). After using it to build the basic structure of the site, I found it lacking in some areas, so I started looking into Hugo themes, how they were built, where the links between the different parts were, and how to customize them even further than the ways given in the base theme.

### Customizing the theme

First of I had to fork the original repository, as working in the original clone does not belong to the best practices.
Then I started by removing a HTML tag that really annoyed me, then I looked into how the built in "Posts" function worked, and how I could use that to make the Projects page.

Of course there are other miscellanious things that I changed, and surely there will be more in the future.

### The Projects page

The Projects page was mainly added to distinguish between the blog posts and the projects, as I wanted to have a page for each of them.
The projects is meant to show what I have done in an article type of way where I also tell the steps I took and there may be some code snippets included.

## Conclusion

I'm really happy with how this site turned out, and I'm looking forward to adding more content to it in the future.
I'm also looking forward to learning more about Hugo and how to use it to it's full potential.
Creating a website with Hugo and a theme was so easy that I might even use it instead of a raw HTML+CSS site in the future, even for small things, as it was so easy to throw up the quickest prototype and then it was ready to be deployed.

### Steps to build a basic Hugo site

1. Install Hugo
2. Create a new site with `hugo new site <sitename>`
3. Add a theme with `git submodule add <theme-repo> themes/<theme-name>`
4. Add the theme to the config.toml file
5. Follow theme instructions for configuration
6. Add content with `hugo new <content-type>/<content-name>.md`
7. Build the site with `hugo`
