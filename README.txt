Coding Temple
HTML & CSS Project
Event Center Website
by Regan Frese

**Intro** - I decided to build my website for a fictional community center based on a few community centers around the Philadelphia area. I wanted this to be a mixed-use space that both organized its own events and also was available for booking public & private events by the community.

**First Steps** - I started out by creating a low-fidelity prototype in Figma. This allowed me to get a general structure for how I wanted the home page to be laid out. I also figured out my color scheme and font choices. From there I had a template for how the other pages could be structured. See Figma mockup here: https://www.figma.com/design/y1VgdhPGUxH17taYGgHoJk/event-center-website?node-id=0-1&t=5t4kKICLZx69TLoc-1

**Design & Style** - Overall my personal style choices tend to be very neutral, muted, and monochromatic. So I went with an overall black & white color scheme with an accent color. Since this is Philly, I used a pastel version of Eagles green for my accent color. I picked a modern sans serif font called Lexend and went with the Deca style and Zetta style throughout the page.

**CSS** - I built a good chunk of my style sheet first since I had my colors, fonts, and layout pretty locked in.

I started by using CSS variables to establish my color scheme (using :root).

Next I introduced my fonts. Since I wanted to use a custom font, I downloaded the font file and established it with @font-face, which I learned how to do on the Google fonts site. I nicknamed each font family and used the relative path to source the file.

Then I created my navigation bar. I wanted the logo for the community center to stay on the left side of the page while the nav buttons stayed on the right. To accomplish this I created a container for the entire bar, created a logo class and a nav-button class, and then created another container for just the buttons. I used Flexbox justify-content: space-between so that the logo part of the bar would stretch across the entire screen regardless of the screen size but the buttons would stay over on the right. I used hover and transition to make it so that when the mouse hovers over the nav buttons, they changed color and had a slight drop shadow. I also removed the text-decoration for the button links to give the button text a cleaner look.

I then established the fonts and colors for my headings and paragraph text.

I wanted to have a photo banner across each page where the photos would stay the same but the text would change on each page. So I created a container for the images and used absolute positioning to float the text over the images. I also used image filters to be able to make all of the images greyscale without having to individually edit each image. All of the images are stock photos from unsplash.com.

For each chunk of content, I created a class and a container for that class if necessary. For example I used .quote for the description and review on the home page. I used .container-block and .block on most of the pages for each page's main content. And I also created an about section for the home page.

Next, I created the footer. This was a challenge because I wanted to have the email newsletter section centered, the site links justified left with four links in a row, and the socials justified right with four links in a row. So I had a few levels of flexbox to get this layout to work. For the links, social icons, and the subscribe button, I used :hover and transitions to make them stand out. I also added target="_blank" to the social icons so that they would open a new tab upon being clicked. I just used each social media's home page for now, since I don't have real social accounts for this fictional community center.

**HTML** - For the events page, I reused the .container-block and block classes I created for the home page. I reused those on a few other pages as well.

For the catering menu page, I used tables to organize the different items on each menu. I used :hover to make the menu easier to read.

For the location page, I embedded a Google maps location (I just used City Hall's address as the address for this fictional community center). I got the embed link directly from Google Maps.

For the Contact page, I used <form> for the contact form. I used <select> to create a dropdown menu so that the user could choose their inquiry topic. I also formatted the form with CSS so it would match the aesthetic of the page.

**Final steps** - Once I had all the CSS done, layout built, and specific content entered, I worked on Media Queries. Most of my tweaks were just to make my containers use the column flex-direction, but I also had some adjustments to make to the image sizes, text sizes, and to the tables. I tested my media queries using the Google Dev Tools built into Chrome.

**Thanks for reading!**

