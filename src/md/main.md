---

# Home

## Introduction

Hey! Welcome to Neotutor, a website that will teach you the basics on how to make your very own personal website! This guide will have everything you will need, from nothing to a beautiful creation of your own. As social media continues to get worse and worse, I felt like this would be a good thing to write up.

## Why should I have a website?

Here are some reasons on why you might want to have your own webpage:

* Put it in your social media profile so people can get to know you better
* Write about your life
* Show off photos you've taken
* Show off art you've made
* Sell commissions
* Show off music you've made

If any of these apply to you, then consider reading more of this.

## But isn't making a website so hard hacker coding?

Not really, as long as you can understand the basics of logic and design, you should be fine. Anyone can make a website with a bit of effort and help from a guide or the broader internet!

## Guide

Now that you've determined you have reasoning and the time to make a website, let's get started!

1. [How do Websites work?](#how-do-websites-work)
2. [Setup](#setup)
3. [HTML](#html)

---

# How do websites work?

I'm not going to get too specific, but basically there is a server with all the information to your website somewhere in the world. This could be your home computer, a datacenter in Silicon Valley, or even a [Raspberry Pi](https://en.wikipedia.org/wiki/Raspberry_Pi)! When the server gets a request to send you a website, it will determine all the info it needs to send to you and then give your computer all the needed files to show a website. This all works over a protocol called **H**yper**t**ext **T**ransfer **P**rotocol (HTTP) which you can find the technical details about [here.](https://en.wikipedia.org/wiki/HTTP)

![Request Example](assets/images/request.png)

1. Client (You) asking for the website files
2. The server gives you the website file(s) if it can find them

### What files are used for programming websites?

The main files you'll find for the structure of a website are:

1. Hypertext Markup Language (HTML) (.html, .htm)
2. Cascasding Style Sheet (CSS) (.css)
3. JavaScript (JS) (.js)

HTML is like the foundation of your website, it determines where things on your website will be placed, such as text, images, and tables.

CSS is like the paint job it's used to style all the different parts of your website that were made with HTML. You can use CSS to make your website look like almost anything you want.

JavaScript is used to make your website more interactive by adding code. Some examples would be making a sound play when you click a button or making a simple game on your website.

---

# Setup

Let's setup our workspace for making a website. In this guide we will be using a free website hosting service called [Neocities](https://neocities.org). They make setting up a website a lot easier while still allowing you to program in regular web development languages (HTML, CSS, and JS)

First, you will need to sign up for a Neocities account, which you can do on their [homepage](https://neocities.org).

![Signup Page](assets/images/signup.png)

Once you have signed up for Neocities, you can navegate to the [dashboard](https://neocities.org/dashboard) by clicking on your name in the topbar and then clicking edit. You should now be in your dashboard, it should look something like this:

![Dashboard](assets/images/dashboard.png)

Your website will have different files because by default it will only have a HTML and CSS file. From there, you can upload files or click on files to edit them, which will be needed for the next section on HTML.

## Limitations of Neocities

Neocities won't let you:

* Post illegal content (Piracy, Drug dealing, etc.)
* Upload audio or video files (Use YouTube or [Catbox](https://catbox.moe))
* Upload executable files (.exe, .dmg, .sh, etc.)
* Upload compressed files (.zip, .rar, .7z, .tar.gz, etc.)
* Hotlink files

Learn more at https://neocities.org/site_files/allowed_types.

---

# HTML

Now that you have setup your neocities account, you can now start programming in HTML!

First, you're going to need to go to your Neocities [dashboard](https://neocities.org/dashboard) by clicking on your name in the topbar and then clicking edit. Then you should see an `index.html`, that HTML file is your homepage of sorts, hover or it and press edit.

![Click on HTML](assets/images/html.png)

Then from there you should be on a screen with some HTML code, let me explain all of it real quick before you start changing things.

## How does HTML work?

HTML uses these things called tags, a piece of information has a opening tag and a closing tag. Here is an example:

``` html
<h1>My awesome title!</h1>
```

The major difference between a closing tag and an opening tag is a closign tag has a slash at the start like this:

``` html
</tag-here>
```

You can also define information such as where a link will go by putting the following in a tag:

``` html
<a href="https://www.wikipedia.org/">Link to Wikipedia</a>
```

* `href="URL-HERE"` is where an `<a>` tag will take you.
* `src="FILE-HERE"` is where you can use a separate file to define information, such as an image file.

## Let's start coding!

To start, Neocities will provide you with some basic HTML code to start, for this tutorial I don't really want to work off that since I want to show what every tag does. Here is a basic HTML document with no code, I will explain what everything in it does.

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    CONTENT HERE
</body>
</html>
```

1. `<!DOCTYPE>` determines what markup language we're using, in this case we're using HTML
2. `<html lang="en">` shows the start of the HTML content and defines what spoken language is used, English is chosen if nothing is there.
3. `<head>` is where extra content needed content is put where it can't be seen by the user directly on the webpage
4. `<title>` defines the title shown on a browser tab
5. `<body>` is where all the main content seen by user will be defined

Now in the body of the page, let's a header so people know what this website is about:

``` html
<h1>Welcome to Neotutor!</h1>
```

Below that, maybe explain what your website will be about with the paragraph tag:

``` html
<p>Hey! Welcome to my awesome website where I talk about things.</p>
```

## HTML Tag List

| Tag | Use | Example |
|-|-|-|
| <pre><code class="language-html">&lt;h1></code></pre> | Big header | <pre><code class="language-html">&lt;h1>Welcome to Neotutor!&lt;/h1></code></pre> |
| <pre><code class="language-html">&lt;h2></code></pre> | Smaller header | <pre><code class="language-html">&lt;h2>What will I cover here?&lt;/h2></code></pre> |
| <pre><code class="language-html">&lt;h2></code></pre> | Even smaller header | <pre><code class="language-html">&lt;h3>Table of Contents!&lt;/h3></code></pre> |
| <pre><code class="language-html">&lt;p></code></pre> | Paragraph/Text | <pre><code class="language-html">&lt;p>Today we'r going to talk about the state of the internet.&lt;/p></code></pre> |
| <pre><code class="language-html">&lt;a></code></pre> | Paragraph/Text | <pre><code class="language-html">&lt;a href="URL-HERE">My Blusky page.&lt;/a></code></pre> |
| <pre><code class="language-html">&lt;img></code></pre> | Image | <pre><code class="language-html">&lt;img src="images/elgato.png"></code></pre> |

Please know this is not a full list of tags.

---

Blinkie to use on your website:

<img src="assets/images/blinkie.png" class="icon">

*Made with <3 by Stormy, source code [here](https://github.com/0hStormy/neotutor).*
