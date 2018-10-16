---
layout: post
section-type: post
title: How I Built this Website
category: Tutorial
tags: [ 'Jekyll', 'WebStuff','Git']
---

# Intro

This post details how I built this website using Jekyll, and hosted it on Github Pages. It's a great tutorial for someone who has no knowlegde of how this process works, and explains everything you need to know to create and host a website on github pages from a pre-exsisting jekyll template. If you already have knowledge of some of the tools used here, feel free to skip sraight to the sections that apply to you. For those of you who want to know how to modify the layout and style of a templated site, I'll include that information in a separate tutorial.

<hr>

# Choosing Your Tools

When it comes to creating and hosting your own website, there are a lot of options out there. As a busy student or professional, you may not the have time to spend hours upon hours working on and maintaining a website from scratch. But you still want to make your website look like a proffesional piece of work. You could use website builders like Wix and Squarespace, but I find those are either too expensive, or place limits on what you can do with your website.

Jekyll was the happy medium for me. It's a framework that manages many of the details of creating and updating your website, while allowing you to configure the site up to the point of including your own HTML, CSS and JavaScript. You don't have to go that fa into things to get a good looking site running, but having the freedom for originality is always a great option.  

Using Jeykll is simple, You just install jekyll, fork an exsisting template from github, add in your own images and text, and you're done! Hosting your website on github pages is even easier, and I'll be showing you how to do all that in this post.

# Using the command line

For this tutorial, we'll be using the Unix Command Line. If you are not familliar with Unix, or the command line in general, Here's a general summary of [The Unix Shell](https://swcarpentry.github.io/shell-novice/reference/). 

For MacOS and Linux, the default terminals are unix shells, but if you're on windowws, I recomend installing [Git Bash](https://gitforwindows.org/) as your unix shell. This will give you unix command line sytax, and it comes with git installed by default, so it saves you the trouble of installing separately.

# Installing Jekyll

I used Bundler to install and manage jekyll. If you have Ruby installed, then installing Bundler should be pretty easy. Just enter the following into the command line:

<pre><code class='bash'>
$ gem install bundler
</code></pre>

If you dont have Ruby installed, you can find details on the [ruby website](https://www.ruby-lang.org/en/downloads/), or you can install using the package manager of your choice.

# Using Git for version Control

Version Control is important for anyone working on a large project, or in large teams. Github is one of the most common version control platforms today. We'll be using github as the host for this website. If you don't have a github account, sign up for one at [github.com](https://github.com/). 

Here are some basic git commands:

<table style="width:100%" class = 'table'>
    <tr>
        <th>Command</th>
        <th>Purpose</th>
    </tr>
    <tr>
        <td>git init {directory_name} </td>
        <td>creates a new git versioned repository</td>
    </tr>
    <tr>
        <td>git status</td>
        <td>prints out the current status of the working branch.</td>
    </tr>
    <tr>
        <td>git add {filename} </td>
        <td>stages a file to be commited</td>
    </tr>
    <tr>
        <td>git rm {filename}</td>
        <td>removes a file from the list of tracked files</td>
    </tr>
    <tr>
        <td>git reset</td>
        <td>reverts the current branch to the last commit</td>
    </tr>
    <tr>
        <td>git commit</td>
        <td>makes a commit to the working branch of your repository</td>
    </tr>
</table> 

These commands should be enough to setup, and manage a basic git repository. But what if we want to start from a pre-made code base? Thats when we fork a repository.

# Forking a Repo

The first step is to find a jekyll template that you want to fork. There are plenty of great options, so you should be able to find a good starting point for whatever you want your site to be.

Once you have a template, it's time to fork the repository and create a local clone on your machine. To fork a repository, navigate to that repository's page and click  the fork button.

![fork-repo-button]({!baseurl}//img//posts//fork-repo-img.png)

now that you've created a fork, navigate to your fork of the jekyll template, click clone or download, and copy the url that pops up.

In the command line on your machine enter the following:

<pre><code class='bash'>
$ git clone {https://my-repository-url}
</code></pre>

for the URL, you should use the address you copied from github. This wil create a local clone of the repository that you can make changes to, and use to update your main site.

# Cusomizing Your Site

Most of the built in customizations for your template will be found in the _config.yml file in you repository. open this file, and change the options to cusomize your template. 

You can do more in depth customizations than this, but those will be covered in a later tutorial. Once you've added the cusomization you want, use the commands:

<pre><code class='bash'>
git add {filename}
</code></pre>

and once you've added all your changed files, run:
<pre><code class='bash'>
git commit -m "some message about the changes you made"
</code></pre>

To finalize and commit your changes. once you've commitied you changes locally, you can push them up to your origin branch on github, by using git push.

That's it, you've created a jekyll site from a template! Now that you have something basic set up, you can start hosting your website, or cutomize it further.