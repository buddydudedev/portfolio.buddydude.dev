---
layout: post
title: Cashflow Classic
assets_dir: cashflow-classic
summary: "A free online game for learning how to invest."
categories: [portfolio, game, programming, web, JavaScript, YETi CGI]
permalink: /portfolio/cashflow-classic
thumbnail: thumbnail.png
---

# Cashflow Classic

<p class="post-summary"><strong>A free online game for learning how to invest.</strong></p>

<div class="categories">
    {% for category in page.categories %}
    <small category="{{ category }}">{{ category }}</small>
    {% endfor %}
</div>

<small class="post-date">2018-03-14</small>

<a  href="/assets/cashflow-classic/cashflow-splash.png" target="_blank">![](/assets/cashflow-classic/cashflow-splash.png)</a>

# Background

As a junior developer at YETi CGI, I worked with a small team of developers to port Cashflow Classic, a Flash game for the web, to native web technologies. To accomplish this, we used CreateJS for the graphics and Firebase for the multiplayer functionality.

# Process

## Handling Lobbies and Multiplayer

Creating lobbies and connect to others in the new Cashflow Classic was done using Google Firebase. Players are able to set up games with up to 6 other players or join others' lobbies.

<a  href="/assets/cashflow-classic/cashflow-lobbies.png" target="_blank">![](/assets/cashflow-classic//cashflow-lobbies.png)</a>

Our Firebase implementation utilized its event-driven functionality to listen to when players join lobbies or when player positions were updated in the game itself.

<a  href="/assets/cashflow-classic/cashflow-lobby.png" target="_blank">![](/assets/cashflow-classic//cashflow-lobby.png)</a>

## The Game Itself

Cashflow Classic starts with each player selecting their dream. On the same card, they are informed as to the job and salary they were randomly assigned. The goal of the game is for players to leave the center of the board, known as the Rat Race, and achieve their dream on the outer board.

The graphics throughout the game were managed by wrapper classes for the CreateJS API. Since we had access to the original graphics of the game and the game was originally made in Flash, using a graphics API that behaved very similarly made the most sense. EaselJS was used to display the graphics and TweenJS was used to move the pieces around the board.

<a  href="/assets/cashflow-classic/cashflow-classic.png" target="_blank">![](/assets/cashflow-classic//cashflow-classic.png)</a>

In addition to using EaselJS for displaying bitmap-based graphics, we also used HTML for some of the graphical user interface elements including the financial statement. While we could have manually placed text using EaselJS, leveraging HTML element also allowed us to use CSS to create the grid layout much more easily. Additionally, it allowed us to more easily implement scrollable areas since we would have had to implement that manually if we were to use exclusively EaselJS.

<a  href="/assets/cashflow-classic/cashflow-folder.png" target="_blank">![](/assets/cashflow-classic//cashflow-folder.png)</a>