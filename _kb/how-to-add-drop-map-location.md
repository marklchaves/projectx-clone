---
layout: kb
collection: kb
type: how-to
title: "Adding a Drop Map Location"
date: 2019-11-12
description: "How-to guide for accessing CloudCannon's visual editor to add a Google Maps location to the Drop Map page (standalone page)."
author: marklchaves
---
## Steps

### Find the Drop Locations Name and URL Fields

1. [Log into CloudCannon.](https://app.cloudcannon.com/users/sign_in)
2. Navigate to the **ProjectX** website from the _Projects_ or _Sites_ dashboard from the left menu bar.
3. From **Projects > ProjectX Live > Sites > ProjectX on master**
4. From **Sites > ProjectX on master**
5. Click on **Explore**. You'll land on **Pages > Standalone** by default.
6. Click on **Drop Map** in the thumbnail grid (should be near the top row). Type **Drop Map** in the search bar if you don't see it right away. The visual editor will open.
7. The page properties are on right hand side. We only need to change the **Locations Name** and **URL**. Please try **not** to edit the **Layout** or **Title**.
8. Enter a name for the location in the **Name** field.

### Add the New URL

1. Go to the new location using **Google Maps**.
2. Click on **Share**.
3. Click on **Embed a map**. Keep the default **Medium** size.
4. Click **COPY HTML**. Then, `cmd C` for Mac or `ctrl C` for Windows.
5. Paste the embed code into a new text editor page.
6. Copy only the link in the `src` attribute. For example, everthing after `src="` and before the closing `"` below. ![Embed Code Screen Capture](/assets/images/help/google-maps-embed-code-1280w.jpg "Google Maps Embed Code Screen Capture")
7. Paste the link into the **URL** field in the **Visual Editor**.
8. Click the _floppy disk_ icon on the upper right to save. Once saved the site will rebuild and your changes will take affect in a few seconds.

---

### Watch the Video

**Note:** Support for multiple map locations was added after this video was recorded. The concept is exactly the same. But, now more than one location can be entered.

<iframe width="560" height="315" src="https://www.youtube.com/embed/NkI6kBczZM0" frameborder="0" allowfullscreen></iframe>

[Watch on YouTube](https://youtu.be/NkI6kBczZM0 "Adding a New Drop Map Location Screencast")