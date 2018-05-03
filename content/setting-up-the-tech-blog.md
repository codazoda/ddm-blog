+++
date = "2018-05-02T08:16:19-06:00"
title = "The DDM Technology Blog"
author = "Joel Dare"
+++

We created this blog to learn about each other through our writings about technology. We hope it can promote cross team collaboration among developers and foster new friendships within DDM. We want to spark conversations with developers that we don't interact with on a regular basis. The idea was born in one of two Dev Spring Camp meetings setup by the DDM scrum masters Chad, Mary, Katie, and Ben.

My goal is to create a blog that's as simple as possible to contribute to and leverages technologies that most of us already use. My hope is to reduce the complexity enough that it encourages contributions.

## Plain Text

I opted to use plain text files, using the common markdown formatting, for the main content that we'd be writing. I also looked at blogging software that could automatically turn those text files into raw HTML. Most of us have written README.md files for our git repositories and otherwise used Markdown formatted text files. I worked under the assumption that we're not all familiar with the particular blogging software I opted to use.

## Static Site Generator

The blog is a static site that can be hosted nearly anywhere. It can be hosted directly on github or on our local development machines. Having chosen markdown, I looked at several static site generators. I considered the most popular options first and then explored a couple of the less popular ones as well. The most popular options are Jekyl and Hugo. Jekyl is supported by Github directly but I opted to use Hugo for two reasons. First, I found it's syntax to be a little bit cleaner. Second, it's distributed as a single executable file with no external dependencies.

## Including the Binary

I opted to include the Hugo binary directly into the repo itself. This reduced the software requirements to get up and going to almost none. Most of the development staff here uses Mac's. With the hugo executable included in the repo the only software requirements are git and your favorite text editor. It does add a little size; it's currently 19MB. No big deal given the typical internet connections we have.

## Manual Site Generation

I considered implementing git hooks to generate the site automatically but decided against it. Git doesn't checkout the `.git/hooks` directory. It avoids that in order to prevent security problems with automatic code execution. There are tricks we can use to implement the hooks anyway but they introduce other requirement such as npm, composer or a script to create symlinks. Ultimately the hooks only reduce a single publishing command so I abandoned the idea.

## Simple Template

I selected one of the most basic site templates offered by Hugo. I then copied the template files directly into the blog repo. Git doesn't bring in submodules automatically and there is no obvious indication that they're required when you first clone a project. Since simplicity was a major goal I opted to copy the files over.

Because, ideally, there will be a lot of us contributing to this blog, I needed to add author information to the individual posts. I made a few minor changes to the template and then renamed it to make it clear that it's not the original. A trade off is that we won't get template updates. I've found that a lot of the existing templates are poorly maintained. Givin that it further reduces complexity and probably won't see a lot of updates anyway, I thought the trade off was worth it.

## Iterating

I wrote the README.md file for this repo and then worked through it dozens of times trying to reduce writing and publishing to a couple of steps each. I'm pretty happy with the few steps that I got it down to but I know there's more room for improvement and I didn't solicit any feedback. If lots of developers get involved and comfortable then the simplicity may become less necessary over time.