# GIFTastic
A project that makes use of an API call to make a dynamic web page

### Overview

In this assignment, I used the GIPHY API to make a dynamic web page that populates with gifs of whatever the user chooses. It calls the GIPHY API and uses JavaScript and jQuery to change the HTML of the site.

### Deployed Site Link
https://doybrian.github.io/GIFTastic/

### Design Concept

1. An array of strings have been initially declared, each one related to a topic that interests me personally. This has been saved to a variable called `topics`. This may not be a necessary step but it helps pre-fill the buttons on the page.
* User can make a list to their own liking.

2. As the page loads, the topics in this array are loaded and create buttons in the HTML.
* Used a loop that appends a button for each string in the array.

3. When the user clicks on a button, the page will grab 10 static, non-animated gif images from the GIPHY API and place them on the page. Each image has a class attached to it and attributes set such that the images are "still" when it loads initially.

4. When the user clicks one of the still GIPHY images, the gif will animate. If the user clicks the gif again, it should stop playing. This was set using the attributes before it was appended to the html.

5. Under every gif, its rating (PG, G, so on) is displayed.
* This data is provided by the GIPHY API.

6. Forms are added to the page that take the value from a user input box especially for adding topics into the `topics` array. A function is then called that takes each topic in the array and remakes the buttons on the page.

### Bonus Goals

1. To ensure the app is fully mobile responsive, Bootstrap was used.

2. The app is developed to allow users to request additional gifs to be added to the page after clicking on other buttons.
* Each request ADDs 10 gifs to the page, NOT overwrite the existing gifs.

3. Included a 1-click button for each gif to its original URL. GIPHY has disabled download on the GIFs. The button instead opens the gif on the GHIPY web site and can saved or possibly downloaded from there.

4. The app allows users to add their favorite gifs to a `favorites` section.
* This will persist even when they select or add a new topic.

5. The app allows users to delete any of existing topics. Also option is given to clear the GIF collection already posted.

6. Sound effects have been added as well.

