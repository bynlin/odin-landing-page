# odin-landing-page

This HTML and CSS project involves building a landing page by referencing an image provided by TOP. My pain points and process:

Part 1: Add structured, page contents in to html:

1. Study image
2. Identify, structure and add into the html:
   • main sections
   • sub-sections into main sections
   • contents into the sub-sections

Part 2: Use 'layout constraints' method to size and position sections:

1. Use 2 layout containers:
   .container {max-width: 64rem; margin-inline: auto; padding-inline: 1rem;}
   .container-narrow {margin-block: 5rem; padding-block:3rem}
2. .container-bubble uses both layout constraints but the narrow version needs to be color blue with padding andborder-radius for:
   .container.bubble {background-color: blue; color:light; max-w}
3. Haven't clean up sizes of margins and paddings yet
4. It only hit home for me at this point that .container.bubble means the element will take in declarations from both .container and .bubble and if i add declarations to .container.bubble, the element will take them in too

Part 3: Sort through the wrapping:

1. A wrapper of background color wraps up the entire section, so that the background color fills viewport instead; aka full-width backgroun
2. Next nested wrapper: layout container (.container) wraps; aka Centered Layout Container
3. Next nested wrapper: section to group the contents, act as a parent; aka Flex Parent Component
4. Next nested wrapper: individual children items; aka Individual children
   These wrappings confuses me to no end... I'm sure there're better ways to do this, but I just don't know what I don't know yet.

Part 4: Deciphering how I should add classes & write selectors to target the elements:

1. There are a lot of times I was writing declarations correctly, e.g. applying styles or flex properties, but it wasn't reflecting. So I thought I was writing them wrong. But then I realise I was targeting wrongly instead, like, img nested deeply in .card should be '.card img' but I tried stuff like, .'card.img' or '.book.img', etc
2. Only when I change the selectors, then the right stylings or flexing would show up

Part 5: Deciphering how I should write so that the landing page flexes:

1. I have the most difficulty with flexing images
   -Problem: telling the img to flex so that it does not overspill its container and so that it fill its container as the container flexes accordingly to viewport changes

- max-width
- min-width
- width
- height
- height-auto

Part 6: Reviewing and refining user experience like making 'go to section' scroll instead of smack
