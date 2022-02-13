# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62).  

## Table of contents

- [The Challenge](#the-challenge)
- [My Screenshot](#my-screenshot)
- [Links](#links)
- [My process](#my-process)
- [Built with](#built-with)
- [What I Lerned](#what-i-learned)
- [Author](#author)

## The Challenge

The challenge is to build out this card component and get it looking as close to the design as possible. Users should be able to view the optimal layout depending on their device's screen size.

## My Screenshot

My solution
| Mobile                                                                                 | Desktop                                                                                 |
| -------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| <img src="./screenshot_mobile.png" width="150" height="" alt="Screenshot of solution"> | <img src="./screenshot_desktop.png" width="500" height="" alt="Screenshot of solution"> |

## Links

- Live Site URL: [https://rauf-dev.github.io/fm_qr-code-component/](https://rauf-dev.github.io/fm_qr-code-component/)

## My process

Mobile first. Then used flexbox and row-reverse to get the desktop layout. Additionally, media queries to finely align content in larger resolutions.

## Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Getting feet wet with BEM methodology

## What I learned

### Perfect is the enemy of finished :clock3::clock4::clock5:

Perharps the most important learning is "Perfect is the enemy of finished". There will always be tweaks and refinements to be done whereby the learning process is stagnant.

### Flex trumps over Grid for responsive layout. Maybe

Flexbox just seems to have more magic than grid in terms of responsiveness.
Need more practice with grid.

### HTML picture element vs media queries

Althought I ended up not using it, the html Picture element can be used to display different images instead of media queries, e.g.

```html
<picture>
    <source srcset="/media/cc0-images/surfer-240-200.jpg"
            media="(min-width: 800px)">
    <img src="/media/cc0-images/painted-hand-298-332.jpg" alt="" />
</picture>
```

### CSS Background property saves lines of code 

Also learnt about the CSS background property that can be used to set all background properties in one line! Albeit it has accessibility concerns as screen readers will not announce an image set using background (url).

```css
 background: url(./images/image-header-desktop.jpg) no-repeat center/cover;
```

### Overlaying a color onto jpg image '🎉'

Creating a color overlay on a jpg image

```html
 <div class="header-image">
    <div class="header-overlay"></div>
  </div>
```

```css
.header-image {
  background: url(./images/image-header-mobile.jpg) no-repeat center/cover;
  height: 350px;
  width: 100%;
  border-radius: 10px 10px 0 0;
}
.header-overlay{
  border-radius: 10px 10px 0 0;
  background: rgba(170, 92, 219, 0.5);
  height: 100%;
  width: 100%;
}
```

## Author

- Website - [raUF!](https://www.heyrauf.com)
- Frontend Mentor - [@raUF!](https://www.frontendmentor.io/profile/yourusername)
