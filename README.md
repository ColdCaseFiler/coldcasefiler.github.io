# Cold Case Filer

A cold case file web utility.

- [Cold Case Filer](#cold-case-filer)
  * [What is it?](#what-is-it-)
  * [Why did you make it?](#why-did-you-make-it-)
  * [How do you use it?](#how-do-you-use-it-)
    + [_config.yml](#_configyml)
    + [index.md](#indexmd)
    + [Assets](#assets)
    + [People, Places and Objects](#people-places-and-objects)
    + [People](#people)
    + [Places](#places)
    + [Objects, Theories and References](#objects-theories-and-references)
    + [Events and Notes](#events-and-notes)
  * [Credits](#credits)

## What is it?

Cold Case Filer is a Github pages template designed to help organize, link and display information in cold cases.

It is free to use and customize for any case of your choosing.

## Why did you make it?

<a href="https://github.com/qwtel">qwtel</a> did a lot of the heavy lifting, this is based on his <a href="https://github.com/hydecorp/hydejack">Hydejack</a> template, which is designed to be a blog/project showcase, and I have simply modified and extended it. I discussed my intended use for his template, he agreed, and I started customizing.

I made this because, often, when reading about a cold case, I will feel like I need a pen and paper to be able to keep track of every name, relation, detail etc. and combining that cataloguing with a searchable, linkable, web-based database capable of distilling a large amount of data into a modern, readable format seemed like a natural extension.

There seem to be so many cases that have a great deal of information available, but seem to be lacking that key detail or perspective that prevent them from being solved. 

I thought this template might be able to help people catalogue the information that's available to them, and, hopefully, provide a fresh perspective.

## How do you use it?

If you have used Github Pages before, then the setup is likely familiar to you, and you will know which files to edit, and how.

If you have not used Github Pages before, it allows you to host a free webpage, based on this template. (or any other!)

The template does all the hard work of web design for you, leaving you free to just enter your data in plain text, which the template wraps into a nice website for you.

The following steps assume that you have no previous experience with Github Pages, or web development in general.

You'll need a Github account (free).

Once you're setup with that, you can come back to this page and hit the fork button:

![Fork](/assets/img/fork.png)

Then, when it asks you what to name it, call it: __yourusername.github.io__

(where __yourusername__ is whatever Github username you chose. My username is __coldcasefiler__, so my repo is called: __coldcasefiler.github.io__)

Now you've got your own site, and you can begin customizing it!

![Files-Folders](/assets/img/files-folders.png)

### _config.yml

This is where the basic info for your site is located, you will want to change the title, description, tagline, keywords and logo to be that of your case.

### index.md

This is the landing page/main page for the site. It will be the first page people see, and the page that they are taken back to when they click the site logo.

I have used this as a case brief, a summary, an overview of the entirety of the investigation, with clickable links that take you to more detailed pages.

You can ignore all the other files, and start adding data to the main sections of the site, located in the following folders: **_objects, _places, _people, _references, _theories, events/_posts, notes/_posts,** and **assets.**

### Assets

The **assets** folder is where you store any media you upload: pictures, PDFs etc.

The **img** (images) folder is broken down into sub-categories for easier organization: People, Places, Objects and References.

So, if you wanted to use the Unknown Person image, you would find it at: **'/assets/img/people/unknown.jpg'**

### People, Places and Objects

All the data for people, places and objects is stored in plain text files. 

They are all formatted using Markdown, so the naming format should be: **filename.md**

Click on one of the folders and then select "Add file" to add a new entry.

If it is a person, give it a name like: **john-doe.md**

If it's a place, something like: **1-main-street.md**

There are then keywords and details we can add to fill out and style the data.

### People

People have the most detailed data sheet. 

Here you can see the data for our example victim, John Doe (this is __john-doe.md__):
```
---
layout: project
sitemap: true
featured: true

type: person
title: John Doe
caption: Victim
category: 0 Victim
date: 1 Sept 1900
description: >
  37 year old Bricklayer from Louisville.
image: 
  path: /assets/img/people/john-doe.jpg
accent_color: '#56BF56'

age: 20
dateofbirth: 1970-08-11
dateofdeath: 1990-04-15 (est)
sex: Male
race: Caucasian
hair_color: Brown
eye_color: Brown
height: 5'10"
weight: 160lbs

notable_features: 
  - Tattoo on left bicep 
  - Birthmark on right shoulder

home: 
  - place: 1 Joetown St 
    area: Joeville, USA
    
work:
  - place: McDonalds Restaurant
    role: Manager
    
school: 
  - place: Doetown High
    area: Doetown, USA

family: 
  - person: Jim Doe 
    relation: father 
    
  - person: Jane Doe 
    relation: mother 
    
  - person: Steve Doe 
    relation: brother

friends:

neighbours:
  - Mark Lee

coworkers:
  - Shelly Williams

affiliations:

interests: 
  - Fishing

vehicle: 
  - 1988 Chevrolet Cavalier
---
  ```
And, [here you can see](https://coldcasefiler.github.io/people/john-doe/) what it looks like once it gets formatted into a webpage.

So, we have a lot of stuff there, but we can break it down a bit. 

The first two sections are settings that all pages will have in common: __layout, sitemap, featured, type, title, caption, category, date, description, image, accent_color.__

__layout__ - should be set to project

__sitemap__ - set it to true if you want the pages to appear in the search

__featured__ - makes the project card larger, I set it to true for the victim, and false for everyone else

__type__ - person, place or object

__title__ - the name of the person, place or object, which will also be the title of the webpage

__caption__ - the smaller writing that appears below the title on the project card, I use it to describe their relation to the case

__category__ - a method of sorting within the main categories: eg People could be subcategorized into: Victim, Perpetrator, Suspect, Law Enforcement etc. 

I added a number to go out in front that would determine the order of the categories. So, if you wanted your categories to be: Thieves, Victims, and Law Enforcement, in that order, you could call them: 1 Thieves, 2 Victims, 3 Law Enforcement, and that would ensure that they go in the correct order, while a script removes the number for you.

__date__ - the date that will be shown in list view, helpful for when you want to post something today, but have it sorted as happening in the past

__description__ - the text that appears to the right of the image on the project page

__image__ - the main image for the project

__accent_color__ - the color of the project card. I used this to help color code people, places and objects as being associated with the victim, the suspect, law enforcement, etc

The rest of the variables are unique to People. 

Some: __age, dateofbirth, sex, height, weight__ etc. are self-explanatory, and can be entered in any format you choose. Eg. __weight__ can be in pounds or kilograms, __dateofbirth__ can be numerical or words, and it will have no effect on the site.

The rest: __home, work, school, family, friends, neighbours, coworkers, vehicle__, will be linked to their respective pages if you name them correctly.

For instance, if we create a person called __jim-doe.md__, then add: Jim Doe to the list of his family, it will automatically link to the page called __jim-doe.md__, but if we refer to a person called: James Doe, our link won't work, since it will be looking for __james-doe.md__, which doesn't exist!

Another example, if we add: __21-1st-street.md__ to the places folder, we must make sure that when we're referring to it we're calling it: 21 1st Street to make sure the names match. 

It won't work if you refer to it as: 21 First Street, or 21 1st St.

You must ensure that the names follow the same format, if you want links to work.

Any data that you leave out will simply be blank. 

If there is information you don't know, you don't need to add it.

### Places

Places has fewer options than People, but one unique feature it has is that you can embed maps.

Use the embed code from your mapping app, as shown below:
```
---
layout: project
type: place
map: <iframe src="https://www.google.com/maps/d/u/0/embed?mid=1-_L86MZm4qn7-NR5lqFZTYeos2QeiKFL" width="640" height="480"></iframe>
title: 'Murder Site'
caption: Location of Homicide.
description: >
date: '01-01-2016'
image: 
  path: /assets/img/places/murder-site.png
links:
  - title: Link
    url: https://hydejack.com/
sitemap: true
tags: [victim]
accent_color: '#FF7575'
---
```

### Objects, Theories and References

These categories have fewer pre-defined options, but you may add any details, images, links etc. you wish.

Markdown makes tables very easy to create.

### Events and Notes

These two categories are the exceptions. While every other page will show a collection of projects, these two will show a collection of posts, so the layout for these should be set to post, and the title needs to be formatted as YYYY-MM-DD-title.md:

Filename: 2012-02-07-john-doe-leaves-work.md
```
---
layout: post
title: John Doe leaves work
slug: events
description: >
  John uses his keycard to check out at work.
date: 1990-04-15 05:05:00 pm
sitemap: true
hide_last_modified: true
tags: [victim]
---

Last confirmed location
```

This is an event, placed in the events/_posts folder. It has the slug: events, and, though the file itself is named __2012-02-07-john-doe-leaves-work.md__, the __date:__ field will override the date contained in the post title.

In the events folder, posts are ordered chronologically, and will be sorted down to the minute, allowing for a detailed timeline reconstruction.

In the notes folder, posts are ordered newest first, like a traditional blog.

You can use the __date:__ field to organize both posts, and projects. There may be times that you wish to group people together: family, associates etc but they are being broken up by other people in the same category. In that case, you can use __date__ to group them together.

Typically, I will use the date that I am creating the post as the title, and reserve the date field for sorting the post into the order I want.

## Credits

This template is based on <a href="https://github.com/hydecorp/hydejack">Hydejack</a> by <a href="https://github.com/qwtel">qwtel.</a>

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

Unknown Person image provided by: <a href="http://getdrawings.com/unknown-person-silhouette">Unknown Person Silhouette</a>

Fake Human images provided by: https://boredhumans.com/faces.php
