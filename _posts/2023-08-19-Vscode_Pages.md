---
toc: True
comments: True
layout: post
title: VSCode, Github Pages Setup
courses: {'csa': {'week': 1}}
type: hacks
---
<html>
<h1 style="padding-left: 70px">Notes</h1>
<h2 style="padding-left: 70px">Commands</h2>
    <ul style="padding-left: 70px">Home directory: cd ~ </ul>
    <ul style="padding-left: 70px">Configure git git config
        <li>git config --global user.email *your email*</li>
        <li>git config --global user.name *your github id*</li>
    </ul>
<h2 style="padding-left: 70px">Set up</h2>
    <ul style="padding-left: 70px"> Forked student repository and copied https link and cloned it in VSCode </ul>

<h2 style="padding-left: 70px">Running pages locally</h2>
    <ul style="padding-left: 70px">Upgrade brew: echo, brew update, brew upgrade, brew install xz</ul>
    <ul style="padding-left: 70px">Ruby: echo, brew install rbenv, rbenv install 3.1.4, rbenv global 3.1.4</ul>
    <ul style="padding-left: 70px">Configure rbenv to initialize in the shell: echo, rbenv versions</ul>
    <ul style="padding-left: 70px">Python & pip: echo, brew install python</ul>
    <ul style="padding-left: 70px">Jupyter notebook: echo, brew install jupyter</ul>

<h2 style="padding-left: 70px">Check versions</h2>
    <ul style="padding-left: 70px">ruby -v, python --version, jupyter --version, jupyter kernelspec list</ul>

<h2 style="padding-left: 70px">Installation</h2>
    <ul style="padding-left: 70px">bundle install, make, make clean when changing the theme, local host and its live, make stop, make convert </ul>

<h1 style="padding-left: 70px">Questions</h1>
<p style="padding-left: 70px"><b>1. In the Development process, developers use Version control. Annotate in notes what you have learned about Version Control while doing this setup process.</b></p>
<ul style="padding-left: 70px; padding-right: 70px">Version control is the practice of tracking/managing changes to code & project files using Git. I've learned that it offers features like branching which allows for parallel development w/out interfering w/main codebase, and merging, which integrates changes from different branches. It also allows me to annotate commits w/meaningful messages, providing purpose & context of each change.</ul>

<p style="padding-left: 70px; padding-right: 70px"><b>(a) Where are the files from GitHub placed on your local machine. How do you navigate to those files.</b></p>
<ul style="padding-left: 70px; padding-right: 70px">terminal: cd ~, ls, cd to directory</ul>
<img style="padding-left: 70px" width="561" alt="Pic" src="https://github.com/e-shen2022/APCSP_Blog/assets/104966589/7ecba803-2aad-42ad-8de5-b2359999d6c2">
<br>
<p style="padding-left: 70px; padding-right: 70px"><b>(b) Where are the files placed in the GitHub Cloud, how do you navigate to those files.</b></p>
<ul style="padding-left: 70px; padding-right: 70px">Navigate to repository you are interested in, click on the "Code" tab, and now you can see the list of files and directories. You can click through folders and their indiivdual files to view their contents</ul>
<p style="padding-left: 70px; padding-right: 70px"><b>(c) How would you update your Fork of student repository if teacher wanted you to pick up an update?</b></p>
<ul style="padding-left: 70px; padding-right: 70px">If it is a new file, just drag it into your repository. If it is updating an existing file, can try these following commands: git remote add upstream *teacher_repo_url*, git fetch upstream, git merge upstream/main, git push origin main. These commands should configure upstream remote, fetch the changes, merge between my local branch and upstream, and push the changes to my fork</ul>
<p style="padding-left: 70px"><b>2. Put into words the difference between viewing GitHub Pages running on localhost machine versus running on a deployed server.</b></p>
<ul style="padding-left: 70px; padding-right: 70px">Viewing GitHub Pages on a localhost machine means you're accessing the website locally on your computer for testing and development purposes. It allows you to preview changes before deploying them, but only you can see the site. Deploying GitHub Pages to a server makes it accessible to anyone on the internet. It's the public version where your changes are permanent, making your website available to a global audience.</ul>
<p style="padding-left: 70px; padding-right: 70px"><b>(a) What is the localhost URL for your distribution? Can anyone else see it?</b></p>
<ul style="padding-left: 70px; padding-right: 70px">Server address: http://0.0.0.0:4200/student/   No one else can see it!</ul>
<p style="padding-left: 70px"><b>(b) What is the GitHub Pages URL for your distribution? Can anyone else see it?</b></p>
<ul style="padding-left: 70px; padding-right: 70px">https://github.com/e-shen2022/student.git. Yes other people can see it.</ul>

<p style="padding-left: 70px"><b>3. DNS is the address manager for the internet. Put into your own words how you changed the address of your student repository.</b></p>
</html>