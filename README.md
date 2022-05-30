# Drink Up client
Unsure of what to drink tonight? Use this site to decide! You can search by name or the primary ingredient. Have no idea what you want? There's a random option as well!

I was inspired to make this project when I stumbled upon this colorful photo by [Amy Shamblen](https://unsplash.com/photos/3G8k9IhI6FE) 

The color palette for this site pays homage to the photo as well.

**Link to project:** (https://clara-ra.github.io/drinkup-client/)

![alt text](https://github.com/Clara-ra/drinkup-client/blob/main/assets/screenshot.png)

## How It's Made:

**Tech used:** HTML, CSS, and JavaScript

This site works in conjunction with the API provided by https://www.thecocktaildb.com .
It has three main features - dynamic search, search by drink category, and random select. 
Dynamic search has an event listener that checks to see if the user has stopped typing into the search bar (via keyup). If the user has stopped typing, then that search will be sent to the API. Once the API has successfully responded back, the list is appended to the DOM via JavaScript. 
Search by drink category will fetch all drinks from the API under the specified category. 
Random drink selection will fetch a randomly selected drink via a feature provided by the API.
When a card is clicked, a modal appears with more infomation on the selected drink. Similiar to when a list is generated, this works by appending new HTML via JavaScript. z-index was utilized to ensure the proper stack order when a modal appears or a list is generated.

## Optimizations

Although this site works across various device screen sizes, there are still some wonky elements depending on the screensize. Sizing should be able to take into account wrapping text such as the drinks selection bar and card containers.
Additionally, cacheing may help speed up search runtimes. The less calls that need to be made to the API, the better.
The icons on the site are comprised of seperate images - a sprite holding all the icons would be better.


## Lessons Learned:

APIs are not infallible - clients should be able to gracefully handle cases when an API takes too long to reply, or never does. I also learned what a modal is and how it can be useful in web design. The z-index property can be invaluable for stylizing your site to look the way you want.

