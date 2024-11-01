# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

This challenge asked me to recreate a QR code for Desktop and Mobile.

### Screenshot

![](./FireShot%20Capture%20001%20-%20Frontend%20Mentor%20-%20QR%20code%20component%20-%20.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

First, I noted down all the elements I could see in the design including an image, h1, h2 and section and organised them into HTML tags.
Then, I inserted these into the HTML body content.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid and Flex
- Desktop-first workflow

### What I learned

The main thing I learned had to do with Grid layouts in CSS. For a long time, I couldn't get my alignment right because I had defined the grid with a repeat function that used fr units. This meant that the browser split my grid into the available space, meaning it wasn't a fixed grid and would change based on the viewport, which made aligning items difficult. Once I measured that each track should be 64px in width, the grid was able to be centre aligned both along main and cross axis so that I could then begin optimising for mobile. To centre align, I used align-content and justify-content. I had tried margin: auto but found this not to be helpful due to its consideration of 'available space'. I learnt the importance of using align-content, not align-items and respectively, with justify. I'd like to practice grid layouts a lot more because I find them incredibly useful as a visual person.

At first, I struggled with writing the media queries for responsive design. It had been a while since I had gone over it. I took a desktop-first approach and used max-width values. I used Chrome dev tools to help me visualise. I wanted the QR code to stay in position down to mobile at 375px, but I had to adjust the grid-column values to ensure that the grid sized down proportionally so the .card stayed in the same place as the viewport width reduced. Something that clicked into place was that before, I was applying width values according to the viewport to the grid container, because I wanted it to take up the space rather than shrink. But, I learnt that if I used width: 100% instead, this snapping into place would stop happening when I sized the viewport down. I don't quite understand why this is, but logically, it makes sense that I should be able to just tell the browser that the grid should take up all the viewport space rather than remain stuck at its max width setting. I guess this meant that any value below the max width and the grid would collapse back to its unresponsive design and shrink smaller and smaller, unhelpfully.

I enjoyed getting into a nice flow trialling different solutions and speedily googling questions I had along the way to piece together my understand of what I did and did not need in my code. It was fun.

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<h1>Some HTML code I'm proud of</h1>
```

```css
.proud-of-this-css {
  color: papayawhip;
}
```

```js
const proudOfThisFunc = () => {
  console.log("🎉");
};
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
