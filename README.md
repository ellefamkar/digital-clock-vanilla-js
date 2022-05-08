# Digital Clock application

## Welcome to my project guys! 👋

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

Thanks for checking out this front-end project. This is a really simple digital clock so as to learn how to write and work with date and setInterval or even setTimeout.

Remember that "Every day is a learning day", so let's checkout the requirements to start such project

### The challenge

In his project you should be able to:

- Provide dynamic digitl clock

### Links

- Live Site URL: [Digital Clock](https://ellefamkar.github.io/digital-clock-vanilla-jss)

## My process

### Built with

- Semantic HTML5 markup
- CSS
- js

You can use any tools you like to help you complete the project. So if you got something you'd like to practice, feel free to give it a try. However, i wrote this design with simple html5 and css, since my users should be able to: View the optimal layout

### What I learned

This projects helped me being more familiar with the details of js and DOM concept, and use my js knowledge as well to create a responsive project with small details and proficient.

To see parts of my codes and see how you can add code snippets, see below:

```html
     <div class="clock"></div>
```
```css
 .clock {
            border: 1px solid #ffffff;
            padding: 1rem;
            border-radius: 25px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translateX(-50%) translateY(-50%);
            color: #17d4fe;
            font-size: 60px;
            font-family: Orbitron;
            letter-spacing: 7px;
         }

```
```js
// add new to do
function showTime(){
    let date = new Date();
    let h = date.getHours();
    let m = date.getMinutes();
    let s = date.getSeconds();
    let session = "AM";

    if(h === 0){
        h =12;
    }
    if(h > 12){
        h = h-12;
        session = "PM";
    }

    h = (h < 10) ? `0${h}` : h;
    m = (m < 10) ? `0${m}` : m;
    s = (s < 10) ? `0${s}` : s;

    
    let time = `${h} : ${m} : ${s} ${session}`;
    document.querySelector(".clock").innerText = time;

}
setInterval(showTime,1000);
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.


### Continued development

In my future projects, not only i am going to focus on improving my basic knowledge of front end developmentso as to create cooler projects. I will also try to be much more familiar with UI design so as to better understand my clients needs and requirements.

## Author

- Website - My website is under construction but you can find my works here : [Elle Famkar](https://github.com/ellefamkar)
- Twitter - [@Ellefamkar](https://www.twitter.com/ellefamkar)

Feel free to ask any questions come to your mind on my github account!

## Acknowledgments

I want to thanks my mentos who have been infuelntial and helpfull with great projects, tips and lessons. 


**Have fun using this project!** 🚀