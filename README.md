# Mobile Web Specialist Certification Course
---
#### _Three Stage Course Material Project - Restaurant Reviews_

## Project Overview: Stage 1

For the **Restaurant Reviews** projects, you will incrementally convert a static webpage to a mobile-ready web application. In **Stage One**, you will take a static design that lacks accessibility and convert the design to be responsive on different sized displays and accessible for screen reader use. You will also add a service worker to begin the process of creating a seamless offline experience for your users.

### Specification

You have been provided the code for a restaurant reviews website. The code has a lot of issues. It’s barely usable on a desktop browser, much less a mobile device. It also doesn’t include any standard accessibility features, and it doesn’t work offline at all. Your job is to update the code to resolve these issues while still maintaining the included functionality.

### What do I do from here?

1. In this folder, start up a simple HTTP server to serve up the site files on your local computer. Python has some simple tools to do this, and you don't even need to know Python. For most people, it's already installed on your computer.

In a terminal, check the version of Python you have: `python -V`. If you have Python 2.x, spin up the server with `python -m SimpleHTTPServer 8000` (or some other port, if port 8000 is already in use.) For Python 3.x, you can use `python3 -m http.server 8000`. If you don't have Python installed, navigate to Python's [website](https://www.python.org/) to download and install the software.

2. With your server running, visit the site: `http://localhost:8000`, and look around for a bit to see what the current experience looks like.
3. Explore the provided code, and start making a plan to implement the required features in three areas: responsive design, accessibility and offline use.
4. Write code to implement the updates to get this site on its way to being a mobile-ready website.

## Leaflet.js and Mapbox:

This repository uses [leafletjs](https://leafletjs.com/) with [Mapbox](https://www.mapbox.com/). You need to replace `<your MAPBOX API KEY HERE>` with a token from [Mapbox](https://www.mapbox.com/). Mapbox is free to use, and does not require any payment information.

### Note about ES6

Most of the code in this project has been written to the ES6 JavaScript specification for compatibility with modern web browsers and future proofing JavaScript code. As much as possible, try to maintain use of ES6 in any additional JavaScript you write.

### Special Note
I have removed all instances of `tabindex` from all non-interactive elements. The rubric states that tabindex is required, however the MDN states that it is not recommended to use it that way.

link: [MDN tabindex page featuring accessibility concerns](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex#Accessibility_concerns)

> Avoid using the tabindex attribute in conjunction with non-interactive content to make something intended to be interactive focusable by keyboard input. An example of this would be using an <div> element to describe a button, instead of the `<button>` element.

> Interactive components authored using non-interactive elements will not be listed in the accessibility tree. This will prevent assistive technology from being able to navigate to and manipulate it. The content should be semantically described using interactive elements (`<a>`, `<button>`, `<details>`, `<input>`, `<select>`, `<textarea>`, etc.) instead. These elements have built-in roles and states that communicate status to the accessibility that would otherwise have to be managed by ARIA.

### Instructions:

1. Clone this app to your computer.

```
git clone https://github.com/TechSnazzy/restaurant-reviews-app.git
```

2. From a command line, change to this project directory and then run the server using Python.

```
cd restaurant-reviews-app
python -m SimpleHTTPServer 8000
```

3. Launch your web browser and visit this page: [http://localhost:8000](http://localhost:8000)

### Resources

I can't give enough thanks or credit to these valuable resources on the web. These resources helped push me in the right direction to get this app running.

* [Project 1 MWS Webinar with Doug Brown](https://www.youtube.com/watch?v=92dtrNU1GQc)
* [Matthew Cranford: Restaurant Reviews App Walkthrough](https://matthewcranford.com/restaurant-reviews-app-walkthrough-part-1-map-api/)
