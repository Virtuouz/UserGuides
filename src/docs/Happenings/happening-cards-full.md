---
title: Happening Cards Full
layout: layouts/page.html
eleventyNavigation:
  key: Happening Cards Full
  order: '9'
tags: Happenings
draft: false
_schema: default
---
![](/assets/images/uploads/image-66.png)

This is a powerful component that will show all upcoming or past happenings whether they are dedicated happening pages or blog posts. However, there is a required set up for this component to work

## Set up for upcoming

Upcoming events can work in 2 ways. With pagination and without pagination. Pagination is when there are too many happenings to fit on one page and the option to view the next page appears.

![](/assets/images/uploads/image-72.png)

### Without pagination

Using this component without pagination works like with any other components. Just add it to your page and your are done. It will show up to 22 happenings

### With Pagination

For upcoming happenings with pagination, this component will **ONLY** work on page that is inside a "Happenings" folder and has a page location of "/"

![](/assets/images/uploads/image-74.png)

Notice the folder above

![](/assets/images/uploads/image-75.png)

This is what the page location should look like. A page location of "/" inside of a folder makes it act like the "home" page for that folder.

## Set up for past happenings

Sometimes we want people to be able to find our past events.

For past events, this component will only work on a page that is inside a "Happenings" folder, and has page location of Past

![](/assets/images/uploads/image-76.png)