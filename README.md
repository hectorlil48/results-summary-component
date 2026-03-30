# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Working through this project reinforced several important frontend development concepts, especially in building clean, scalable, and responsive UI components.

One of the biggest takeaways was the importance of creating a design system using CSS variables. By defining colors, font sizes, and font weights in the :root, I was able to keep my styles consistent and easy to maintain:

```css
:root {
  --navy-950: hsl(224, 30%, 27%);
  --fs-md: 1.125rem;
  --fw-bold: 700;
}
```

This approach made it much easier to update styles globally without searching the entire file.

I also focused on writing structured and reusable CSS using the BEM naming convention. This helped me organize styles clearly and avoid conflicts:

```css
.card__item {
  display: flex;
  justify-content: space-between;
}
.card__item-score {
  font-weight: var(--fw-bold);
}
```

Using BEM made the relationship between elements obvious and improved readability.

Another key learning was building responsive layouts with Flexbox and media queries. I designed the layout to stack vertically on smaller screens and switch to a side-by-side layout on larger screens:

```css
@media (min-width: 768px) {
  .card {
    display: flex;
  }
}
```

This reinforced how to think about layout changes across different screen sizes and how to structure components for flexibility.

I also learned the importance of keeping spacing consistent rather than strictly following every value from the design file. In cases where tools like Figma provided fractional values (e.g., 56.5px), I rounded them to maintain a cleaner spacing system.

Finally, I added small touches for accessibility and user experience, such as focus states for buttons:

```css
.card__button:focus-visible {
  outline: 3px solid var(--navy-200);
}
```

Overall, this project helped me move beyond just styling components and start thinking more about scalability, consistency, and real-world development practices. It gave me more confidence in structuring CSS for larger projects and preparing for frameworks like React.

### Continued development

1. Advanced Responsive Design Techniques
   I’m comfortable with Flexbox and basic media queries, but I want to get better at complex layouts that adapt smoothly to multiple breakpoints, including handling dynamic content without breaking the design.

2. CSS Architecture & Reusability
   Using BEM and a design system helped a lot, but I want to practice scaling these systems for larger projects. For example, creating reusable components with consistent spacing, typography, and color variants.

3. Animations and Micro-Interactions
   I want to refine my ability to add subtle, polished animations for hover states, button interactions, and loading states, without overdoing them or impacting performance.

4. Accessibility and Semantic HTML
   I added focus states and rounded some alt text practices, but I want to consistently apply accessible design patterns, including proper ARIA attributes and semantic markup for larger, interactive components.

5. Spacing and Layout Consistency
   Rounding fractional spacing values was a good start, but I want to get more comfortable with a full spacing scale and design tokens, so layouts feel intentional and cohesive across projects.

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - It helps to check how padding and margin should be applied.

### AI Collaboration

During this project, I used Claude AI to help guide some of my design and development decisions. Specifically, I used it to:

Think through style choices — for example, deciding on consistent spacing, color usage, and whether to round fractional values from the Figma design.
Check accessibility — asking whether certain elements, like icons or buttons, needed proper alt text or focus states.
Get feedback on my progress — validating that my approach to structuring CSS, using BEM, and building responsive layouts was on the right track.

What worked well:

Claude AI helped me clarify decisions quickly without second-guessing myself.
It was useful for confirming best practices and accessibility considerations.

Overall, using AI as a coaching and advisory tool helped me make more confident, intentional design and development choices while building this project.

## Author

- Website - [Hector Ramirez](https://www.hectorramirez.dev/https://www.your-site.com)
- Frontend Mentor - [@hectorlil48](https://www.frontendmentor.io/profile/hectorlil48)
- Github - [@hectorlil48](https://github.com/hectorlil48)
