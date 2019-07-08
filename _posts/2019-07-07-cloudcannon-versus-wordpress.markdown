---
layout: post
title: CloudCannon Versus WordPress
date: 2019-07-07 12:00:00
description: >-
  First impressions from spinning up a couple Jekyll sites on CloudCannon.
  Coming from a former software engineer who found himself supporting WordPress
  sites since 2015.
image: /uploads/cloudcannon-wordpress-logos.png
author: mark l chaves
tags:
  - Review
  - CloudCannon
  - WordPress
---

## First Impressions

My very first impression of **CloudCannon** was oxymoronic at best. I was introduced to CloudCannon by a friend just about two months ago. I briefly looked at the CloudCannon site (didn't know anything about *Jekyll* yet) and thought,

> "Oh no, do I really need to *(re)invent* the wheel yet again?"

At the same time–I was running into a brick wall trying to squeeze every speed optimisation trick in the book out of **WordPress** (bloated themes and WordPress hosting company's included). Dealing with these performance headaches made me reminisce about the good old times when the web was so young (c. 1995). I pondered, why can't I go back and use a static webpage for my home page? Why does WordPress stuff everything into the database only to be spit out again as a static HTML file in the end. Surely, not every page needs to be 100% generated from a database (which is just a big series of flat files as well).

So, there I was. Looking for maybe some sort of hybrid solution when a friend told me their site was hosted on something called CloudCannon.

### TLDR

1. I dreaded the thought of writing *by hand* an entire website in HTML/CSS/JS. *Reinventing* a photo gallery or slider was not appealing to me at all.
2. I grew *complacent* with not having to write much code. But, I suffered on a daily basis working long hours **optimising** about a dozen bloated WordPress sites with minimal gains.

Enough whining. Let's look at the code\!

## What I Like About WordPress

There are a **plethora** of hosting providers, themes, & plugins. Which is also WordPress' dark-side. For example, if I need a homepage hero *slider*, there are many to choose from. If I need an image *gallery* or a *modal popup*, they are almost always built into a premium theme. Easy. I don't need to go into any code to get these widgets up and running fast.

A lot of the widgets and plugins are well designed and sexy. Many are free, *freemium*, or donation-based.

Having these *conveniences* can also be a *curse*. See below.

Having a bunch of hosting provider options is a *big* benefit. WordPress is a popular website/web CMS platform. Therefore, there is no shortage of finding skilled professional to support a WordPress site.

## What I Don't Like About WordPress

#### WordPress Development == Slow Page Refreshes

I really dislike (hate) having to refresh slow loading page builder editors and posts/pages. But, I'm too afraid to install a bloated WordPress development environment and all the third-party plugins that come with it on my laptop.

#### Too Many Moving Parts

Way too many moving parts. And, these moving parts change all the time. E.g. WordPress versions, PHP versions, plugin updates, and theme upgrades. Most of my clients have way too many plugins. One of my clients has over 50 plugins. She doesn't even know which ones she really needs. I'm trying to get it down to high thirties low forties (still too high for my liking). Auditing and pruning plugins is not easy–putting it lightly. It's been a work in progress for weeks and we're not done yet.

#### Uncontrollable Page Bloat

Themes provide little control over what gets loaded on your web pages. Some more optimised themes give you some control. But, mostly not at page-level i.e. site-wide control only. And, page-level granularity is what is vital for optimising a website.

Standard general purpose themes generate way too many *round-trips* to the server (135-156 server requests is common). Obviously, 156 server requests is a ridiculous **waste of resources** for every single page on the site.

Too many ways to shoot yourself in the foot. Multiple ways to add custom code (scary). Child themes should absolutely be necessary, but support for child themes is not well advertised. It's an extra step. It adds more complexity and overhead. And to make things worse, most WordPress site owners have no clue they need to use one.

Inconsistent support for dev environments. Mixing up original intention of staging environments. This is getting into the weeds, but I need to mention this.

My personal WordPress site is pretty simple. Yet, half of my plugins are devoted to performance tuning. I'll most likely need a couple more optimisation plugins before the end of this year. Crazy.

## What I Like About CloudCannon

#### Transparency

I can see all the source HTML I need to see. I can do stuff that WordPress rejects in it's editor or stuff that I need to install yet another bloated plugin just to inject a couple lines of code.

#### Local Development Environment

I'm back using a version control system\! Yay\! Something I haven't been able to use in the WordPress universe. And, GitHub rocks\! My live CloudCannon sites, GitHub code repositories, development repositories, and development site are always in sync. Love it. I don't this I could ever do this with WordPress. I wouldn't even know where to start. With CloudCannon, GitHub is a natural part of the process.

I can build/test/publish customisations quickly. The dev cycle is light speed compared to WordPress.

\#2 GitHub. Portable. Fast local dev env. Want to move the code to another server or another laptop. Easy\!\!

\#3 Lean. Don't need to know phpMyAdmin. Don't need to know SQL. Almost a anti-plugins environment.

Minimal editor. Similar to Medium's editor, which I like.

## What I Don't Like About CloudCannon

CMS editor is slow. Takes a few seconds to save a post with no images. Seems to hog my CPU. Very similar to how slow Divi is and how it chokes my computer resources.

I don't see a preview button in the editor.

I don't see an obvious market or store for themes. I (luckily) stumbled upon the two themes that I'm using now.

I don't see a way to create a draft version of a published post.