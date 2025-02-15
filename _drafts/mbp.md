---
layout: post
title: MBP-Tutor Admin Portal Redesign
assets_dir: mbp
summary: "I redesigned the admin portal of the MBP-Tutor site to improve the user experience and enhance productivity."
categories: [portfolio, web, design, programming, JavaScript, PHP, MSU]
permalink: /portfolio/mbp
thumbnail: thumbnail.png
---

{% include post-details.html %}

## Overview

While working as a web developer at Michigan State University's Broad College of Business, I was tasked with redesigning the administration portal for the [Multicultural Business Progam's](https://broad.msu.edu/undergraduate/opportunities/mbp/) tutoring website (MBP-tutor). The site was built using `Laravel` and `jQuery` and uses `LDAP` to connect MSU's single sign-on. No code for this project will be shown because it is a proprietary web application; all sensitive information will be blurred.

## Goals

Prior to the redesign, the admin portal of the MBP-tutor site primarily consisted of a core page which included all the functionality for managing the tutor roster, assigning students to tutors, checking students' grades, and monitoring appointment attendance. While this was functional in a literal sense, but the user experience suffered from the difficulties that came with navigating collapsable sections and obscure input layouts.

As such, we set the following goals when redesigning the portal: 

- Separate functionality into different pages.
- Improve layout and visibility of inputs.
- Maintain familiarity for those accustomed to the workflow pre-redesign.
- Introduce single sign-on so the administrator and tutors can login with their MSU accounts.

This would prove to be a daunting task for me as I was a new employee at the time still familiarizing myself with the university's systems. However, I was able to successfully meet these goals to the satisfaction of my supervisors and the current site administrator.

## Implementation

### Breaking Out Functionality

The most glaring issue with the site was that all the functionality on that core page was buried inside a massive JavaScript bundle created by a web developer who no longer worked for the university. After digging through the bundle and reviewing the sections of the core page, I determined that it would make the most sense to split the functionality of the site up into the following:

#### Tutor Roster Management

The first piece of functionality to get its own page was the ability to manage the current roster of tutors. This includes:

- Reviewing new tutor applications.
- Assigning current tutors to time slots and rooms.
- Updating a tutor's employment status and pay.

All the aforementioned features are found in a `table` element that contains information on all the tutors for the current semester. There is also a `fieldset` near the top of that contains all the filters for tutoring status.

<a href="/assets/mbp/roster.png" target="_blank">![](/assets/mbp/roster.png)</a>

#### Tutor Assignment

#### Student Grades

#### Tutoring Courses

### Reinventing the Wheel

### Single Sign-on

## Reflections