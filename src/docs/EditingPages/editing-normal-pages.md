---
_schema: default
title: Normal Pages
layout: layouts/page.html
eleventyNavigation:
  key: Normal Pages
  order: '1'
tags: Editing Pages
draft: false
---
When you first create a an image or edit and existing page you'll presented with many options. Lets break each of the options down

![](/assets/images/uploads/image-18.png)

## Page options

### Draft

This should be self explanatory. If this is checked it your page will be considered in draft mode and will not show up in your live site.

Unfortunately, draft pages do not have access to the live editor. A page must be non draft and saved for the live editor to show up for that page. If you want to live edit your page, but don't want people to find it, you can use the "Remove from navigation" option (more on this later.

All newly created pages will have draft mode check. Don't forget to uncheck the box before saving once you are ready to publish your page.

### Page Title

Every single page on any website requires a page title, this is where you set yours. A page title is what you see in the top tab of your browser

![](/assets/images/uploads/image-21.png)

💡 **Note:**<br>"My Business Name" can be updated in your "site" data file found in your site data section

### Remove from navigation

If this option is turned on it will remove the page from all navigation. What this means is that the page won't show up in the top navigation, footer navigation, or even your sitemap (hidden from google).

This is an useful option for when you need for a page to exist that you don't want anyone to find accidentally. A good example of this is a form submission confirmation page. This option can also be turned on when you want to work on a page with the live editor, but don't want people to see that its not ready yet. Doing it this way is most useful with brand new pages.

### Navigation

This lets you set up how your page will show up in your navigation. This is also where you can create submenus of pages in your navigation.

![](/assets/images/uploads/image-22.png)

#### Standard Use (easy)

When you first create a page you'll need to remember to update the navigation settings of the page. Lets break down each navigation setting how to use it the simple way

##### Key

What you type into the key box is how the page will be identified within the navigation. You can think of the Key as the ID of the page as far as the navigation goes. For simple use, this should be something that quickly explains the pages purpose.

Examples: Home, Services, Contact, Blog

##### Order

In what position this page should show up in the navigation. A page with an order of 1 will be shown first in the navigation compared to pages with order of 1,2,3.... If two pages have the same "Order" one will randomly chosen to actually take that "Order" position and the other page will be placed right after it.

For example, lets say we have pages  Services(2), Blog(3), Contact(2), and Home(1) where the number the number inside the parentheses is that pages order. In the navigation the pages will be shown in this order:<br>Home, Services, Contact, Blog.

Whichever goes second between Services or Contact will be random since they have matching order.

#### Creating Submenus (advanced)

You should start considering creating submenus for your pages once you start reaching 7 or more normal pages, if not your top navigation will start to look ugly very soon. Below is an example of many pages and no submenus being used. While it's not bad, it's very messy looking.

![](/assets/images/uploads/image-23.png)

##### Key

When creating submenus the key has a new role. It becomes the main page (parent) that all the other pages are to be listed under (children).

##### Order

Order will still work the same way as before, except it will be the order within the submenu

##### Display Title

This is where display title might be used more. you might have a parent Key that is easy to type out (like team) but you want to show up as something different in the navigation (like Team Members).

##### Parent

You will place the key of the parent page here for every child page that should be part of the submenu. Continuing with the Team Members example, all the children page would have a parent Key of "team"

##### Putting it all together

Lets use the example of having a Team Members page, but each team member gets their own dedicated page to express themselves with. Your main Team Members page would have a Key of Team Members

![](/assets/images/uploads/image-29.png)

&nbsp;

Every individual team member page would then have their own Keys, like their names for example. What each team member page would share in common would be that they would all share the same Parent key. An example of what the navigation could look like:

![](/assets/images/uploads/image-30.png)

#### External Link

Sometimes you want to link out to a file or another page directly from your website navigation so that it is easier for your customers to get to. An example of this might be a payment page that is powered by the software that you use to keep track of billing.

To link out to other websites or files easily from your navigation you would use this option. You would still need to fil out all previous information navigation (Key, Order, Display Title\[optional\], and Parent\[optional\])

❗**IMPORTANT**:<br>This will prevent the page from building and will not show up on your website if a link is placed here.

### Page Location

This is the location of your page on your website. Another way to think of it is where should this page be linked.

However, if you leave the page location blank it will just use your Page Title as the location.

#### Blog - Special Location

The page location/link of "blog" is special. A page with a page location of blog will only show up in the navigation if you have at least 1 blog post. If you have none, this page will not show up even if you have added content to it.

The reasoning for this is that this page will be used in combination with the Content Section of "Blog Cards Full"

### Meta Description

This is short summary description of the page. This short description is what will be shown in search results. Example below:

![](/assets/images/uploads/image-31.png)

This meta description should usually target a keyword your customers are likely to use when searching for your kind of business.

There are plenty of guides online explaining how to write good meta descriptions, but here are some important pieces:

1. Meta descriptions summarize page content for search users.
2. They influence click-through rates and SEO indirectly.
3. Characteristics of a good meta description:
   * Up to 155 characters in length.
   * Uses active voice and includes a call-to-action.
   * Relevant to page content and unique.
   * Utilizes focus keywords and specifications when applicable.
4. Tips for managing meta descriptions across multiple pages:
   * Prioritize critical URLs.
   * No meta description is better than a bad one
5. Meta descriptions for social sharing enhance visibility on platforms.
6. Despite Google's discretion in displaying them, well-crafted descriptions improve user experience and engagement.

### Hero Content

Every single page requires a hero section. If not hero section is given, the "Simple Hero" will be used and it'll use your pages "Page Title" for the heading.

Refer to the Hero content guide for more information.

### Content Blocks

These are your website sections that you use to build out your website visually.

Refer to the Content Blocks guide for details on each one.