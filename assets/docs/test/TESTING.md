# Hand Embroidery Testing

![Site Mockup](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/mockup/site-mockup2.jpg)


---

## Site Functionality Testing
- __Automated Testing: HTML & CSS Validation__

    HTML and CSS code have been tested and validated by using: [W3C HTML](https://validator.w3.org/) and
[W3C CSS](https://jigsaw.w3.org/css-validator/). Result screenshoots following these links: [HTML Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-HTML-Validator.jpg), [CSS Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-CSS-Validator.jpg)

- __Manual Testing__

    In order to ensure the proper functionality of this single-page site, the following aspects have been tested manually: 

    1. Buttons: work and have same format.
    2. Contact Form & Success Message: work and are correctly displayed.
    3. Images: are properly displayed.
    4. Icons: open correct site in a different tab.
    5. Links: redirect to corresponding site/section.
    6. Paths: set properly, no broken paths.
    7. Typos: absence of any typing error.
    8. Toggle menu: dropdown menu for small screens displays properly.
   
    
    The bellow table shows manual tests performanced:

    | Action | Expected Behaviour | Result |
    | :---         |     :---:      |          ---: |
    | Click all navbar links   | Redirect to corresponding section     | Pass    |
    | Click navbar Contact icon  | Redirect to Contact section     | Pass    |
    | Click logo image   | Redirects to Home page     | Pass    |
    | Click welcome section button  | Redirect to About section     | Pass    |
    | Check all site images   | Images are properly displayed    | Pass    |    
    | Click footer social media icons   | Redirect to corresponding social media site     | Pass    |
    | Click footer About Us links   | Redirect to corresponding section     | Pass    |
    | Click footer Follow Us links    | Redirect to corresponding social media web     | Pass    |
    | Click content typos  | No typing mistakes     | Pass    |
    | Submit form with valid fields  | User redirect to CI form page     | Pass    |
    | Submit form with invalid fields  | Required field message pops up     | Pass    |
    | Click on bars icon  | Displays dropdown menu, Hides bars icon     | Pass    |
    | Click on xmarks icon  | Hides dropdown menu, shows navbar     | Pass    |
    | Re-click on bars icon after clicking on xmark icon  | Displays dropdown menu again, Hides bars icon     | Fail -- dropdown menu is not displayed    |
   


> [!NOTE]
> The initial test of the "Re-click on bars icon" failed. Check [Bugs](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/TESTING.md#bugs-troubleshooting) section to see issues fixed.



- __Peer-code-review Testing | Slack Community__

    After a peer-code-review request, the following issues were spotted by code peers feedback:

    1. Contact form was not fully responsive on small screens.
    2. Footer contact column content had not enough contrast.
    3. Xmark icon on small screens stopeed working after initial use of the bars icon.
    4. Dropdown menu extra right side space.



> [!NOTE]
> Check [Bugs](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/TESTING.md#bugs-troubleshooting) section to see issues fixed.



## Responsiveness Testing

The site responsiveness was tested by using [Ui.dev](https://ui.dev/amiresponsive) as well as Chrome Google Developer Tools checking how the site react to different screen sizes. Check the result here: [Site Responsiveness](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/mockup/site-mockup.jpg)
 
## Accessibility Test Testing

The following tools have been used to ensure this site meets the required accessibility standars: [Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.) and 
[Wave.org](https://wave.webaim.org/)

Testing results can be found here: [Wave Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/wave-testing.jpg) , [Lighthouse Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/lighthouse-testing.jpg)

## Browsers Testing

Manually testing has been performed on the following web browsers: Google Chrome, Safari, and Microsoft Edge.

Additionally, testing has been carried out on the following phone devices: Xiaomi lite 12 and samsung s14.

Testing has taken into account a range of viewport sizes, including desktop, phone, and tablet dimensions.

## Bugs Troubleshooting
- __CSS Issues: Dropdown Menu Style and Footer content__

    The extra bottom space of the dropdown menu was fixed by applying the flex property 'justify-content: space-evenly' so menu link items will be distributed evenly.
    
    On the footer the columns headings were highlighted by increasing the font-weight property.

- __Responsiveness Issue: Contact Form__

    The Contact form fields were overflowing the screen as they were too big to fit into the screen. That issue was fixed by changing the width and padding of the field elements and their container.

- __Fail Test: "Submit form with invalid fields"__
- __Fail Test: "Re-click on bars icon"__
- __Git Issue:__
- __Accessibility Improvement__


## Testing Tools

- [W3C HTML](https://validator.w3.org/)
- [W3C CSS](https://jigsaw.w3.org/css-validator/)
- [Ui.dev](https://ui.dev/amiresponsive)
- [Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.)
- [Wave.org](https://wave.webaim.org/)
