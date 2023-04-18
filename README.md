# Make It Real - 404 NOT FOUND
This is a solution to the '404 NOT FOUND' project of the Make It Real course.
## Overview
### The challenge
The user will see a 404 page with a scarecrow that will have a responsive design. Making the page both for mobile and desktop.
### Screenshots
Screen of 375px by 800px:
![SS of the challenge in a screen of 375px by 800px.]ss\ss-375.png

Screen of 1440px by 800px:
![SS of the challenge in a screen of 1440px by 800px]ss\ss-1440.png
 
## My process
### Built with
- HTML5
- CSS
- Flexbox 
### What I learned
It was my first time using flexbox and I think it went pretty good. Actually at first I thought it was completely mandatory to use a media querie to make a responsive design, however as I was working with the flexbox the design become responsive by itself.

I joined the scarecrow and the main texts on a .container, and then used the `flex-wrap: wrap;` so when the screen width was reduced the items could reorganize one below the other.
Next, I used `justify-content: center;` and `align-items: center;` so the items inside .container where centered in the page.

Something a little hard and strange forme that I'm still understanding is how in the .attribution div I needed to use `display: flex`, and `postion: absolute` at the same time:
```
.attribution {
    color: #7b7b7b;
    font-size: 12px;
    display: flex;
    justify-content: center;
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    margin-bottom: 10px;
}
```
The `display: flex` allowed me to center the items that were: the text of the div and the `<a>` element with my name.

The `postion: absolute` allowed me to set the position in the bottom part and center with `left: 50%` and ` transform: translateX(-50%);`, so that the `left` property moves the elemetn left edge to the middle of the page (50%), and then the `transform` property is used with the function `translateX(-50%)` to move 50% of the element in the X axis to the leftb(because of the negative value).


### Continued development

I found `flexbox` really helpful, however I think I'm just starting to understand it, actually I think I'll need to study more CSS, because I'm finding harder to understand this than coding in JavaScript. 

### Useful resources
Where I searched everything about flexbox:
- https://css-tricks.com/snippets/css/a-guide-to-flexbox/#aa-flex-basis

Where I found the centering piece of code with `transform: translateX(-50%)`:
- http://web.simmons.edu/~grovesd/comm244/notes/week8/centering-elements#:~:text=To%20horizontally%20center%20a%20block,combination%20with%20the%20transform%20property.&text=The%20left%20property%20shifts%20the,used%20with%20the%20translate%20function.
It is not a secure place but has some really good info.

## Author
- Name - Federico Cordoba 
- Twitter - @mercuryeater

