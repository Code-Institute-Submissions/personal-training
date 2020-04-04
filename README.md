
<div style="width:100%;height:150px; padding: 30px;
    display: flex;justify-content:center;align-items:center; background-color: #000;">
<img src="assets/images/logo_white.png" style="margin-right:10px; margin-bottom: 25px;" alt="DC logo"/><h1 class="display-4" style="font-size: 6em; font-family:&quot;Monserrat&quot;, sans-serif;color:#fff; "> Personal Training</h1>
</div>

# Personal Training Webpage

## Description

The front end of a personal training service web page. This project is mainly intended to showcase my skills as a User Interface Designer (UID). My intentions were to appropriately style a web page whilst making it easy to navigate and still be fit for purpose.

The intended users of this readme document would be prospective employers or other students of web development/UI looking to gain inspiration of some sort. Emphasis should be placed on the fact that this is purely for educational purposes and I have no aspiration of using this as a commercial site. With that being stated, the pictures used are stock images suitable for non-commercial content. The people in the images are not actually clients of mine. Numbers and addresses aren't real. They were used to give a realistic impression for the aesthetic of the layout.

I hope you enjoy my work and any feedback you may have would be greatly appreciated. 

[![Run on Repl.it](https://repl.it/badge/github/Domchap90/personal-training)](https://repl.it/github/Domchap90/personal-training)

Please visit via github pages:
 https://domchap90.github.io/personal-training/

## Contents

<ul>

<li>User Experience</li>
<li>WireFrames</li>
<li>Testing</li>
<li>Code to Website</li>
<li>Resources</li>
<li>Credits</li>
<li>Acknowledgements</li>
<ul>

## User Experience

### Website Goals:

This would be a business to customer (B2C) website. The appropriate considerations were made into marketing and accessibility to the general public.

<ol>
<li>To create Brand awareness.
Having an online presence in the personal training world is everything. Especially for increasing residual income revenue streams further in the future. These could be things such as an online membership where people would potentially pay to gain access to articles/ ebooks that the trainer writes about. </li>
<li>Sell Personal Training sessions</li>
<li>Increase client engagement by encouraging them to use our site for extra information thereby increasing the likelihood of  retention</li>
</ol>




## Wireframes

### Index page:

<img src="wireframes/index_page.png" alt="markups of index page">

### Results page:

<img src="wireframes/results_page.png" alt="markups of results page">

### Training page:

<img src="wireframes/training_page.png" alt="markups of training page">

### Contact page:

<img src="wireframes/contact_page.png" alt="markups of contact page">

## Testing

Description, Expected outcome, Result: pass/fail.

### Functionality

Link Test:
There are 3 types of links that were used in my project. Namely external  (leave the website), internal (direct to another page) or anchor which directs to another region of the same page.
<ol>
<li></li>
<li></li>
<li></li>
</ol>
|           | Index      | Results    | Training   | Contact    |<br>
| --------- |:----------:|:----------:|:----------:|<br>
| External  |   
| Internal  |    | right-aligned | $1600 |<br>
| Anchor    |  | centered      |   $12 |<br>
| Total     | are neat      |    $1 |<br>

To ensure all the links were working, I had to count the number of opening 'a' and 'button' tags on each page. An easy way of doing this is to use ctrl+f and search tool in my IDE (for this project I used Visual Studio Code) and it would return result 1 out of the total count. Or it could return a 'No Results' message but this would be a problem on a website with multiple html pages.
Index Link count:
 allowing me to skip straightsystematically  start from the top of each page and hover the cursor over each and every item/element scanning from left to right top to bottom. Waiting for some visual clue that the item was infact a link typically the cursor changes from a pointer to a hand image. Also i had set my <a> elements to in most cases change shade to a brighter instance of the color already in place. I would then proceed to click on the link and see what happened. 

If an external link passed the test it would successfully direct me to another website and the page that was listed in the href attribute. 
If an internal link 
    -internal
    -anchor 
-test forms
    -scripting (empty mandatory fields caught)
    -defaults are populated
    -Optimal formatting
-html + css (W3C tools)
    -syntax errors
    -appropriate color schemas/contrast.
    -comply with W3C site.

### Usability

    -menus,buttons, links all clearly visible and consistent?
    -All images contain alt text.
    (test via Chalkmark, Clicktale, Clixpy or Feedback Army)

### Compatibility

    -Across different OS, browsers + resolutions.
    - use NetMechanic

## Code to Website

    Set up to github pages link.

## Contributors

I, Dominic Chaple am the sole contributor of this project.

## Resources

The logo was created using a company called Free Logo Design:

<a href="https://www.freelogodesign.org/">https://www.freelogodesign.org/</a>

I used Jesse Couch's pen for the hamburger icon animation:
<a href="https://codepen.io/designcouch/pen/Atyop">https://codepen.io/designcouch/pen/Atyop</a>

From this pen i was able to figure out how to do a similar type of animation. This time used for the toggle icon
on the expandable accordian feature for the FAQs.

I am a big fan of rgb to hexadecimal converters online. 
<a href="https://www.rgbtohex.net/">https://www.rgbtohex.net</a>

This was used when I originally used hexadecimal coloring for the shaded overlays ontop of the wide fluid containers labelled as 'headline's. I tried to make the overlays reveal the image underneath by initially changing the 'opacity' property. However the downside to this is that it also alters the text opacity which made it very difficult to read. As a result I chose to use the 'rgba' for the 'background' property instead yielding much better results.
    .headline-overlay { background: rgba(36,34,45,0.5); }

Another website that became of great utility when I had to check the visual aspects over was the contrast checker.<br> 
<a href="https://webaim.org/resources/contrastchecker/">https://webaim.org/resources/contrastchecker/</a>

This was used in conjunction with the Google chrome developer tools extension which helped me endlessly with regards to troubleshooting my code. To the extent where I'm not sure how I would cope without it! Developer tools is tremendously useful in peeling back the layers of styling code that are applied to different resolutions.

## Credits

 Here are links to the free stock images used throughout my project.

### contact page:

<a href="https://www.pexels.com/photo/photo-of-man-running-during-daytime-2803158/">https://www.pexels.com/photo/photo-of-man-running-during-daytime-2803158/</a><br>

### training page:

<a href="https://pxhere.com/en/photo/1364544">https://pxhere.com/en/photo/1364544</a><br>
<a href="https://pixabay.com/images/search/squatting/">https://pixabay.com/images/search/squatting/</a><br>
<a href="https://pxhere.com/en/photo/1330495">https://pxhere.com/en/photo/1330495</a><br>
results page:
<a href="https://pxhere.com/en/photo/903193">https://pxhere.com/en/photo/903193</a><br>


## Acknowledgements

I would like to thank my mentor Brian for helping me out with some much needed advice especially when it came to the general look and design of the website. I'm not naturally the most creative person and i often find it hard to gauge what looks good on my own. Brian made this process a lot easier for me.