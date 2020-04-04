
<div style="width:100%;height:150px; padding: 30px;
    display: flex;justify-content:center;align-items:center; background-color: #000;">
<image src="assets/images/logo_white.png" style="margin-right:10px; margin-bottom: 25px;" alt="DC logo"/><h1 class="display-4" style="font-size: 6em; font-family:&quot;Monserrat&quot;, sans-serif;color:#fff; "> Personal Training</h1>
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

Here I test the front end in 3 manners. First of all, probably considered the most fundamental test is whether or not the interactive elements of the website actually work as intended. This will include things like navigation links, buttons, forms being submittable with correct validation. Also to check syntax in the code itself.

Secondly is the compatibility of the program. It's easy to assume it works from the computer that the project was written on but what about other devices? Large screen desktops? Mobile devices?  Furthermore one has to consider the different operating systems and even more so the array of browsers that could host the website. 

The final manner of testing is Usability, does the website cater to individuals with learning disabilities? How easy is it to navigate from one section to another? Does the website look good? How consistent is the structure across the pages? 

### Functionality

Link Test:
There are 3 types of links that were used in my project. Namely external  (leave the website), internal (direct to another page of the website) or anchor (directs to a specific region of a page). The default anchor '#' is the top of the same page.

To ensure all the links were working, I had to count the number of opening 'a' and 'button' tags on each page. An easy way of doing this is to use ctrl+f and search tool in my IDE (for this project I used Visual Studio Code) and it would return result 1 out of the total count. Or it could return a 'No Results' message but this would be a problem on a website with multiple html pages.

#### Link Count

index page contains
ext 5, internal 5, anchor 2 (essentially same link but active in 2 different resolutions) - Total 12
results page contains
ext 5, int 5, anchor 1 (button link) - Total 11.
training page contains
ext 5, int 5 , anchor 5 - Total 15 (Note - 5 price button links were set as anchor tags due to there being no destination page)
contact page contains
ext 7, int 5  anchor 0. (Note- 1 ext link is on the googlemaps iframe) - Total 12.                 

 Knowing where all the anchor tags and buttons are located, I would then systematically hover the cursor over every link and button on each page and note the outcome. I used the following check list to ensure each link was working correctly.

#### Link/Button Checklist
<ol>
<li>Upon hovering the cursor over the link. The expected hover effect (as written in the stylesheet) takes place.</li>
<li>The cursor changes from an arrow pointer icon to a hand icon.</li>
<li>Upon clicking the link or button any active effect put in place should be now shown.</li>
<li>The destination page or region is located correctly.</li>
<li>Destination page is located in the appropriate tab.</li>
</ol>

### Expected Outcome

<ol>
<li>I had set my link elements to subtly change colour to a brighter instance of the colour already in place. All links typically went from grey color #c6c0c0 to bright white #fff upon hovering. Buttons had no hover effect.</li>
<li>The cursor should indeed change from an arrow pointer icon to a pointing hand icon on all links and buttons.</li>
<li>I didn't add any active effects.</li>
<li>Should reach the location listed in the 'href' property of the anchor tag or the 'action' property of the form button.</li>
<li>External links should be opened in a new tab. Internal in the same tab.</li>
</ol>

#### Result

All 50 links passed.

Form Test:
There are only 2 forms on my site. They are both formatted under the same CSS rules in my stylesheet. So the consistency is 100% across all forms. Because this is a front end project only the button can't actually do as intended and submit forms as that would require a backend using JavaScript to use some business logic to store it into a database or potentially create email links. 

At the moment, the only current features that should be able to pass tests are the validation of the submitted entries and the default entries being populated.

For validation testing all possible permutations of entry boxes containing at least one character or more must be considered. In this case, one of the forms has 4 entry fields (training page) and the other 3 (contact page). The validation at the front end scope will only determine whether the fields are empty or not. It will not be able to assess whether the format of the entry matches a certain regex pattern for example emails containing no spaces and at least one '@' and '.' character. Further backend code is required in order for this type of testing to be carried out.

The form button typically executes some action upon being clicked but as there is no back end the button will simply serve as an anchor link to the top of the page if all required entries are non-empty. I will call this scenario Successful validation or SV in short. Contrary to this Unsuccessful Validation (UV) will be where at least one field is found to be empty that should be non-empty. In this case, a pop up will appear notifying the user that from the top down the first empty required field it comes across must be non empty. 
 
The contact page form is the simplest test so let's start with that one. All fields are required here therefore Succesful Validation should happen in one scenario only - Three non-empty entry boxes. In order to complete the test play out the following scenarios after each one hit the 'Send' button:

Key: FullName=FN, Email=E, Query=Q, non-empty= ne, empty=e.

FN:e,E:e,Q:e -> UV
FN:ne,E:e,Q:e -> UV
FN:ne,E:ne,Q:e -> UV
FN:ne,E:ne,Q:ne -> SV

#### Result

Contact page form passed.

Training page form has two SV cases with the availability field either empty or non-empty whilst all other required fields are non-empty.

FN:e,E:e,A:e,G:e -> UV
FN:ne,E:e,A:e,G:e -> UV
FN:ne,E:ne,A:e,G:e -> UV
FN:ne,E:ne,A:e,G:ne -> SV
FN:ne,E:ne,A:ne,G:ne -> SV

#### Result

Training page form passed.



-html + css (W3C tools)
    -syntax errors
    -appropriate color schemas/contrast.
    -comply with W3C site.


### Compatibility

    -Across different OS, browsers + resolutions.
    - use NetMechanic

### Usability

    -menus,buttons, links all clearly visible and consistent?
    -All images contain alt text.
    (test via Chalkmark, Clicktale, Clixpy or Feedback Army)

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