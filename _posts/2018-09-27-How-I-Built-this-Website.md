---
layout: post
section-type: post
title: How I Built this Website
category: Tutorial
tags: [ 'Jekyll', 'WebStuff','Git']
---

# Intro

This post details how I built this website using Jekkyl, and hosted it on Github Pages. This is a great tutorial for someone who has no knowlegde of how this works, and explains everything you need to know to create and host a website on github pages from a pre-exsisting jekyll template. If you already have knowledge of some of the tools used here, feel free to skip to the sections that apply to you. For those of you who want to know how to modify the layout and style of a templated site, I'll include that in a separate tutorial.

====================================================================================


# Choosing Your Tools

When it comes to creating and hosting your own website, there are a lot of options out there. As a busy Engineering student, I don't have time to spend hours upon hours working on and maintaining a website from scratch. But I want to make my website look like a proffesional piece of work. Website builders like Wix and Squarespace are either too expensive, or place limits on what you can do with your site.

Jekyll was the happy medium for me. It's a framework that manages many of the details of creating and updating your website, while allowing you to configure the site up to the point of including your own HTML, CSS and JavaScript. You don't have to go that far to get a good looking site running, but having the freedom for originality is always a great option.  

Using Jeykll is simple, You just install jekyll, fork an exsisting template from github, add in your own images and text, and you're done! Hosting your website on github pages is even easier, and I'll be showing you how to do that as well.

# Using the command line

For this tutorial, we'll be using the Unix Command Line. If you are not familliar with Unix, or the command line in general, Here's a general summary of [The Unix Shell](https://swcarpentry.github.io/shell-novice/reference/). 

For Mac and Linux, the default terminals are unix shells, but if you're on windowws, I recomend installing [Git Bash](https://gitforwindows.org/) as your unix shell.

# Installing Jekyll

I used Bundler to install and manage jekyll. If you have Ruby installed, then installing Bundler should be pretty easy. Just enter the following into the command line:

<pre><code class='bash'>
$ gem install bundler
</code></pre>

If you dont have Ruby installed, you can find details on the [ruby website](https://www.ruby-lang.org/en/downloads/), or you can install using the package manager of your choice.

# Using Git for version Control

Version Control is important for anyone working on a large project, or in large teams. Github is one of the most common version control platforms today. We'll be using github as the host for this website. If you don't have a github account, sign up for one at [https://github.com/]. 

using markdown

| command                      | purpose                                |
|------------------------------|----------------------------------------|
|git init \<directory name\>   | creates a new git versioned repository |
|git status                    | prints out the current status of the working branch. includes information on files that have been staged for commit, files that have been removed from you repo, or have been edited and are not staged.|
| git add \<filename\>         | stages a file to be commited |
| git rm \<filename\>          | removes a file from the list of tracked files |
| git reset                    | reverts the current branch to the last commit |
| git commit                   | makes a commit to the working branch of your repository |

using html

<table style="width:100%" class = 'table'>
    <tr>
        <th>Command</th>
        <th>Purpose</th>
    </tr>
    <tr>
        <td>git init [directory_name] </td>
        <td>creates a new git versioned repository</td>
    </tr>
    <tr>
        <td>git status</td>
        <td>prints out the current status of the working branch. includes information on files that have been staged for commit, files that have been removed from you repo, or have been edited and are not staged.</td>
    </tr>
    <tr>
        <td>git add [filename] </td>
        <td>stages a file to be commited</td>
    </tr>
    <tr>
        <td>git rm [\<]filename[\>]</td>
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


# Forking a Repo


# Cusomizing Your Site