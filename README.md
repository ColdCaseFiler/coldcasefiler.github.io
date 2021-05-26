# Cold Case Filer

A cold case file web utility.

## What is it?

Cold Case Filer is a Github pages template designed to help organize, link and display information in cold cases.

It is free to use and customize for any case of your choosing.

## Why did you make this?

Well, <a href="https://github.com/qwtel">qwtel</a> did a lot of the heavy lifting, this is based on his <a href="https://github.com/hydecorp/hydejack">Hydejack</a> template, which is designed to be a blog/project showcase, which I have simply extended.

I discussed my intended use for his template, he agreed, and I started customizing.

I made this because, often, when reading about a cold case it will make me feel like getting out pen and paper to be able to keep track of every name, relation, detail etc. There seem to be so many cases that have a great deal of information available, but seem to be lacking that key detail or perspective that prevent them from being solved. I thought this template might be able to help people catalogue the information that's available to them, and, hopefully, provide a fresh perspective.

## How do you use this?

You'll need a Github account (free).

Once you're setup with that, you can come back to this page and hit the fork button:

Then, when it asks you what to name it, call it: yourusername.github.io 

(where yourusername is whatever Github username you chose. My username is coldcasefiler, so my repo is called: coldcasefiler.github.io)

Now you've got your own site, and you can begin customizing it!

### config.yml

This is where the basic info for your site is located, you will want to change the title, description, tagline, keywords and logo to be that of your case.

### index.md

This is the landing page/main page for the site. It will be the first page people see, and the page that they are taken back to when they click the site logo.

I have used this as a case brief, a summary, an overview of the entirety of the investigation, with clickable links that take you to more detailed pages.

You can ignore all the other files, and start adding data to the main sections of the site, located in the following folders: _objects, _places, _people, _references, _theories, events/_posts, notes/_posts, and assets.

### Assets

The assets folder is where you store any media you upload: pictures, PDFs etc.

The img (images) folder is broken down into sub-categories for easier organization: People, Places, Objects and References.

So, if you wanted to use the Unknown Person image, you would find it at: '/assets/img/people/unknown.jpg'

### People, Places and Objects

All the data for people, places and objects is stored in plain text files. They are all formatted using Markdown, so they should all be filename.md 

Click on one of the folders and then select "Add file" to add a new entry.

If it is a person, give it a name like: john-doe.md

If it's a place, something like: 1-main-street.md

There are then keywords and details we can add to fill out and style the data.

### People

People have the most detailed data sheet. Here you can see a sample of the data for our example victim, John Doe:
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
  ```
So, we have a lot of stuff there, but we can break it down a bit. The first two sections are settings that all pages will have in common: layout, sitemap, featured, type, title, caption, category, date, description, image, accent_color.

__layout__ - should be set to project

__sitemap__ - set it to true if you want the pages to appear in the search

__featured__ - makes the project card larger, I set it to true for the victim, and false for everyone else

__type__ - person, place or object

__title__ - the name of the person, place or object, and the title of the webpage

__caption__ - the smaller writing that appears below the title on the project card

__category__ - a method of sorting within the main categories: eg People could be subcategorized into: Victim, Perpetrator, Suspect, Law Enforcement etc.

__date__ - the date that will be shown in list view, helpful for when you want to post something today, but have it sorted as happening in the past

__description__ - the text that appears to the right of the image on the project page

__image__ - the main image for the project

__accent_color__ - the color of the project card. I used this to help color code people, places and objects as being associated with the victim, the suspect, law enforcement, etc


## Credits

This template is based on <a href="https://github.com/hydecorp/hydejack">Hydejack</a> by <a href="https://github.com/qwtel">qwtel.</a>

Unknown Person image provided by: <a href="http://getdrawings.com/unknown-person-silhouette">Unknown Person Silhouette</a>

Fake Human images provided by: https://boredhumans.com/faces.php
