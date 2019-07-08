---
layout: post
title: CloudCannon Versus WordPress
date: 2019-07-07 12:00:00
description: >-
  First impressions from spinning up a couple Jekyll sites on CloudCannon.
  Coming from a former software engineer who found himself supporting WordPress
  sites since 2015.
image: /uploads/cloudcannon-versus-wordpress/cloudcannon-wordpress-logos.png
author: mark l chaves
tags:
  - Review
  - CloudCannon
  - WordPress
---

## First Impressions

My very first impression of **CloudCannon** was *oxymoronic* at best. It just didn't make sense at first, e.g., to go *sling* around a lot of code to build things that are already available for WordPress.&nbsp;

I was introduced to CloudCannon by a friend about two months ago. I briefly looked at the CloudCannon site (didn't know anything about *Jekyll* yet) and thought,

> "Oh no. Do I really need to *(re)invent* the wheel yet again? Do I really need to code-up an image carousel when there are hundreds of off-the-shelf WordPress carousels out there?"

At the same time–I was running into a brick wall trying to squeeze every speed optimisation trick in the book out of **WordPress** (bloated themes and WordPress hosting companies included). Dealing with these performance headaches made me reminisce about the good old times. When the web was so young (c. 1995). I pondered, why can't I go back and use a static webpage for my home page? Why does WordPress stuff everything into the database only spit everything out as a static HTML. Surely, not every page needs to be 100% generated from a database (which is just a big series of flat files).

So, there I was. Looking for (maybe) some sort of hybrid solution when a friend told me their site was hosted on something called CloudCannon.

### TL:DNR

1. Looking at CloudCannon for the first time, I dreaded the thought of writing *by hand* an entire website in HTML/CSS/JS. *Reinventing* a photo gallery or slider seemed like a complete waste.
2. With WordPress, I grew *complacent* with not having to write much code. But, I suffered on a daily basis, working long hours **optimising** about a dozen bloated WordPress sites with minimal gains.

**Enough whining. Let's look at the code\!**

![](/uploads/cloudcannon-versus-wordpress/WordPress-logotype-alternative-792.png){: width="792" height="428"}

## What I Like About WordPress

There is a **plethora**. Hold on. There is an **extravaganza** of hosting providers, themes, & plugins. Which is also WordPress' *dark-side*. For example, if I need a homepage hero *slider*, there are many out there to choose from. If I need an image *gallery* or a *modal popup*, they are almost always built into a premium theme. I don't need to go into any code to get these widgets up and running fast.

A lot of the available *widgets* and plugins are **well designed** and *sexy*. They look amazing and they work well. Many are free, *freemium*, or donation-based.

Having these *conveniences* can also be a *curse*. More on that soon.

Having a bunch of **hosting provider** options is a *big* benefit. WordPress is the most popular website/web CMS (content management system) platform in the world\! Therefore, there is no shortage of finding skilled professionals to support a WordPress site.

If you have the time, skills, and budget, you can have a fast WordPress site that Google *PageSpeed* loves. I'll have to say though, achieving this takes near-heroic efforts.

## What I Don't Like About WordPress

#### WordPress Development == Sloooow Page Refreshes

I really dislike (hate) having to refresh slow loading page builder editors and posts/pages. But, I'm too afraid to install a bloated WordPress development environment and all the third-party plugins that come with it on my laptop.

#### Too Many Moving Parts (Plugin-arrhea)

There are way too many moving parts in a typical WordPress site. These moving parts change all the time. E.g. WordPress versions, **PHP** versions, plugin updates, and theme upgrades. Most of my clients install too many plugins. For example, one of my clients has **over 50 plugins**. They don't even know which plugins they really need and most of them are outdated (one hasn't been supported for 6 years--no joke). I'm trying to get it down to high thirties, low forties (still too high for my liking). Auditing and pruning plugins is not easy. And, that's putting it lightly. It's been a work in progress for weeks and we're not done yet. I've only managed to prune about a dozen so far. Every WordPress developer knows having too many plugins is a **security risk** and performance killer.

#### Uncontrollable Page Bloat

Themes provide little control over what gets loaded on your web pages. More optimised themes give you some control. But, mostly **not** at page-level, i.e., site-wide control only. Page-level granularity is where you really need the control--it's vital for optimising a website.

Standard *general* purpose themes generate way too many *round-trips* to the server (135-156 server requests are common). Obviously, 156 server requests are a ridiculous **waste of resources** for every single page on the site. As a reference, **GTmetrix** (a leading site performance test tool) says **88** requests are the average.

#### More Than Enough Rope

Ah, let me count the number of ways to *shoot* ourselves in the foot. For example, I can add custom CSS to the

1. Appearance &gt; Customise &gt; Additional CSS
2. Theme's main style.css file
3. Child theme's style.css file
4. Theme editor
5. Site builder's page-level Additional CSS code snippet editor
6. Inline CSS in the text editor

Have fun managing changes with this. Let alone trying to find a **bug**&nbsp;this *spaghetti* architecture.

#### Glossed-Over Child Themes

Any experience WordPress developer knows to always create a child theme for the main theme. Child themes are where theme customisations go. Why aren't they just built-in?? Why does a developer or a site owner even have to know that child themes exist? Why WordPress theme companies **deliberately build themes that they know will absolutely break** unless the site owner creates a child theme? That would make too much sense–I mean, that would be the responsible thing to do.

![](/uploads/cloudcannon-versus-wordpress/avada-child-theme-warning-792.png){: width="792" height="323"}

So, we're forced to supply our own child themes. But, support for child themes isn't obvious. Creating a child theme is another extra step. It adds more complexity and overhead. And to make things worse, most WordPress site owners have no clue they need to use one.

#### Optimisation Slavery

My personal WordPress site is pretty simple. Yet, half of my plugins are devoted to performance tuning. I'll most likely need a couple more optimisation plugins before the end of this year. And, Google keeps yelling at to put my site on a CDN, if I want a good PageSpeed score. Really? All this for a personal website. Insane\!

## ![](/uploads/cloudcannon-versus-wordpress/cloudcannon-opengraph-792.jpg){: width="792" height="416"}

## What I Like About CloudCannon

#### Transparency

I can see all the source HTML I need to see. Yay\! I can do stuff that WordPress rejects in its editor. E.g.

itemscope itemtype="http://schema.org/Blog"

This tiny piece of code is small, but it packs a punch in the **SEO** world. WordPress strips out this code every time I've tried to add it to my site. Arghhh. With CloudCannon–no worries, mate\! In fact the theme this blog is using has this code already in these pages. Now that's responsible coding\! Happy Days :-)

In the WordPress realm, there's probably a bloated 500 file plugin that will do this tiny little thing for you.

#### Local Development Environment

I'm back using a version control system\! Something I haven't been able to use in the WordPress universe. And, GitHub rocks\! My live CloudCannon sites, GitHub code repositories, development repositories, and development site are always in sync. Love it. I don't think I could ever do this with WordPress (smoothly). I wouldn't even know where to start. With CloudCannon, GitHub is a natural part of the process.

I can build/test/publish customisations quickly. The dev cycle is light-speed fast compared to WordPress.

So, with GitHub and using GitHub Desktop, my two CloudCannon sites are completely portable. I.e., they are already in the cloud, on the web, and on my desktop. I can take them anywhere that runs Jekyll.

Developing websites using local dev env is fast–it's the way to go. What if I want to move the code to another server or another laptop. Easy. Setup Jekyll and Github Desktop and away you go.

The Jekyll ecosystem is lean. I don't need to know PHP or phpMyAdmin (MySQL database manager). I don't need to know SQL. And, the Jekyll culture is an anti-plugin/establishment culture.

#### Editing Content

The CloudCannon content editor is minimalist (and, a bit primitive compared to WordPress). This can be good/bad. I love a minimal editor. CloudCannon's editor works fine for me in terms of functionality. But, it might not work for someone used to WordPress because lack of bells & whistles.

Here's one thing I discovered by accident–CMD-L brings up a link modal right in context. How cool is that\! I wish WordPress could do this.

![](/uploads/cloudcannon-versus-wordpress/cloudcannon-editor-blog-post-link-modal-792.png){: width="792" height="585"}

I think the content editor is the weakest link (so far). Read on below to find out why. Before we toss out the baby with the bathwater–we need to give credit to Jekyll's native document format for blog posts. That's **markdown**. Markdown is incredibly powerful and extremely fast. It's about as minimal as you can get when it comes to publishing content. I love it. I'm happy to see it and use it again.

[Read-up on markdown here](https://guides.github.com/features/mastering-markdown/){: target="_blank"}. By the way, if you use **WhatsApp** or **Slack**, Try using markdown in your next message. You'll look like a pro\!

The downside is that markdown will take some getting used to if all you know are visual editors. The good news is, I bet you will soon be addicted to how much more productive/faster you become (in a short time).

## What I Don't Like About CloudCannon

Here's a short laundry list of what I don't like about CloudCannon

#### Content Editor

1. The content editor is slow. It takes a few seconds to save a post with no images. The editor seems to hog my CPU. Very similar to how slow Divi is and how Divi chokes my computer resources. I ran some performance tests and discovered that the Divi page builder editor actually takes up less CPU than CloudCannon's content editor. I didn't this that was possible\!
2. I don't see a preview button in the editor. I had to publish my draft to see what it would look like.
3. I don't see a way to create a draft version of a published post. In WordPress, you can make draft from a published post in one-click.
4. Ironically enough, I don't see a way to edit HTML/CSS in the CloudCannon editor. You have to get out of the content editor and go into the files directory. Find the blog post markdown file and bring it up in the code editor.

#### Where Are The Jekyll Theme Marketplaces?

Lastly, I don't see an obvious *market* or *store* for Jekyll themes. I (luckily) stumbled upon the two themes that I'm using now.

#### CSS Sprites

I would have loved to use a CSS sprite for this blog post. Using CSS sprites reduce server round trips. Unfortunately, that means I needed to write this post in HTML. Therein lies the trade-off. Simple/minimal/markdown versus HTML/CSS/JS. Maybe that's my next homework assignment?

If you found this useful, please share it. [Or even buy me a cuppa joe](https://ko-fi.com/marklchaves#){: target="_blank"}. Hint hint ;-)