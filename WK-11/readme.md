# Week 11 Summary
### by Scott LaForest

### Homework Cycle:

I tried to create a true parallax scrolling site by following the [True parallax in CSS](http://keithclark.co.uk/articles/pure-css-parallax-websites/) tutorial that was provided in
this week's content. It was difficult to get right and there are a few problems that I still do not know how to fix.

### Steps for completing this week:
1. Choose images
2. Develop parallax scrolling
3. Research ways to add responsiveness
4. Test code and fix as needed (1000X)

### Trials and Triumph
The first problem was getting it to work on mobile. The scrolling works well on >1000px screens
but anything smaller and some spaces started to show up. I am assuming this is due to the images but the scrolling still looks good. The main thing was turning off the parallax when the screen width is less than 1000px. I used a media query and reset the layers to 0 in `translateZ`. I also
had to change the main `parallax` class to have `perspective:none` and `overflow-y:scroll`.

Secondly getting the images to fit in without any spacing was tough as well. I ended up making sure that all the images had the exact same size 1024X768 and this helped. But again on smaller screens the scrolling left large spaces between the images and content so I turned off parallax
for screens less than 1000px.

### Goals with this page
My main goal was to try a true parallax scrolling implementation and for the most part I think it
works well. However the responsiveness was a challenge and I had to make a very large media query at `max-width:1000px` to make the margins disappear.

### Going Forward
Parallax is really cool and I think looks great when done correctly. In the future I might try a more basic type of parallax that might be easier to make responsive.
