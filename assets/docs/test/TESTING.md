# Hand Embroidery Testing

![Site Mockup](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/mockup/site-mockup2.jpg)


---

## Site Functionality Testing
- __Automated Testing: HTML & CSS Validation__

    HTML and CSS code have been tested and validated by using: [W3C HTML](https://validator.w3.org/) and
    [W3C CSS](https://jigsaw.w3.org/css-validator/). 

    <details>
    <summary>Click here to see validation results below</summary>
    <br>

    ![HTML Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-HTML-Validator.jpg)

    ![CSS Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-CSS-Validator.jpg)

    </details>


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
    | 1. Click all navbar links   | Redirect to corresponding section     | Pass    |
    | 2. Click navbar Contact icon  | Redirect to Contact section     | Pass    |
    | 3. Click logo image   | Redirects to Home page     | Pass    |
    | 4. Click welcome section button  | Redirect to About section     | Pass    |
    | 5. Check all site images   | Images are properly displayed    | Pass    |    
    | 6. Click footer social media icons   | Redirect to corresponding social media site     | Pass    |
    | 7. Click footer About Us links   | Redirect to corresponding section     | Pass    |
    | 8. Click footer Follow Us links    | Redirect to corresponding social media web     | Pass    |
    | 9. Click content typos  | No typing mistakes     | Pass    |
    | 10. Submit form with valid fields  | User redirect to CI form page     | Pass    |
    | 11. Submit form with invalid fields  | Required field message pops up     | Fail -- form is sent without fields been validated    |
    | 12. Click on bars icon  | Displays dropdown menu, Hides bars icon     | Pass    |
    | 13. Click on xmarks icon  | Hides dropdown menu, shows navbar     | Pass    |
    | 14. Re-click on bars icon after clicking on xmark icon  | Displays dropdown menu again, Hides bars icon     | Fail -- dropdown menu is not displayed    |
    <br>

    > The initial tests 11.'Submit form with invalid fields' and  14.'Re-click on bars icon' failed. Check [Bugs](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/TESTING.md#bugs-troubleshooting) section for further information.


- __Peer-code-review Testing | Slack Community__

    After a peer-code-review request, the following issues were spotted by code peers feedback:

    1. Contact form was not fully responsive on small screens.
    2. Footer contact column content had not enough contrast.
    3. Xmark icon on small screens stopeed working after initial use of the bars icon.
    4. Dropdown menu extra right side space.
    5. Too many contact buttons so might be redundant for users.
    <br>

    > All the above issues were addressed and sorted out. Further information on: [Bugs](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/TESTING.md#bugs-troubleshooting) section.


## Responsiveness Testing

The site responsiveness was tested by using [Ui.dev](https://ui.dev/amiresponsive) as well as Chrome Google Developer Tools checking how the site react to different screen sizes.  

<details>
<summary>Click here to see the result below</summary>
<br>

![Site Responsiveness](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/mockup/site-mockup.jpg)

</details>

 
## Accessibility Test Testing

The following tools have been used to ensure this site meets the required accessibility standars: [Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.) and 
[Wave.org](https://wave.webaim.org/)

<details>
<summary>Click here to see testing results below</summary>
<br>

![Wave Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/wave-testing.jpg)
![Lighthouse Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/lighthouse-testing.jpg)

</details>


## Browsers Testing

Manually testing has been performed on the following web browsers: Google Chrome, Safari, and Microsoft Edge.

Additionally, testing has been carried out on the following phone devices: Xiaomi 12 Lite, Huawei P Smart and samsung s14.

Testing has taken into account a range of viewport sizes, including desktop, phone, and tablet dimensions.


## Bugs Troubleshooting
- __CSS Issues: Dropdown Menu, Footer Content, Responsiveness Issue__

    The extra bottom space of the dropdown menu was fixed by applying the flex property 'justify-content: space-evenly' so menu link items will be distributed evenly.
    
    On the Footer the columns headings were highlighted by increasing the font-weight property.

    The Contact button on the Gallery section was removed as redundant for users.

    On small screens, the Contact form fields were overflowing the screen as they were too big to fit into the screen. That issue was fixed by changing the width and padding of the field elements and their container.

- __Accessibility Improvement__

    Low Contrast: The contrast between h5 headings and the background colours was very low. To improve accessibility the initial chosen colour, font size and font weight were edited ensuring that users with visual impairments can now read them easily.

    Images Weight: Images were converted to WebP format, as suggested by my mentor and the Lighthouse Testing report, to achieve quicker loading times.

    Empty Navbar Link: The Contact icon link on the navbar had no text, so a describing text that presents the functionality of the link was added to avoid confusion for screen reader users.

    <details>
    <summary>Click here to see testing results improvement below</summary>
    <br>

    ![Wave Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/wave-testing2.jpg)
    ![Lighthouse Testing](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/lighthouse-testing2.jpg)

    </details>

- __Fail Test 11: 'Submit form with invalid fields'__

    When the 'onclick' JavaScript event was applied to the button element of the contact form, the validation of the form fields using the 'required' HTML attribute was not functioning.
    
    To streamline the project and for testing purposes, the 'onclick' event was eliminated, and the test was reattempted, check result bellow:

    | Action | Expected Behaviour | Result |
    | :---         |     :---:      |          ---: |
    | 11. Submit form with invalid fields  | Required field message pops up     | Pass  |

- __Fail Test 14: 'Re-click on bars icon'__

    When the fa-bars icon in the navbar was clicked after opening the dropdown menu, an unexpected issue arose where the bars stopped to function.

    <details>
    <summary>Click here to see old JavaScript code below</summary>
    <br>

    ![JS code](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/script-dropdown-menu.jpg)


    </details>


    The issue was fixed by removing the JavaScript code and using pure CSS to create the hamburger menu. Code inspiration and reference: [Codepen.io | Erik Terwan](https://codepen.io/erikterwan/pen/EVzeRP). Then the test was performanced again, check result bellow:

    | Action | Expected Behaviour | Result |
    | :---         |     :---:      |          ---: |
    | 14. Re-click on bars icon after clicking on xmark icon  | Displays dropdown menu again, Hides bars icon     | Pass  |

- __Git Issue: Push failed__

    When trying to push a commits from the local repository to the remote one, this error appeared.

    After some research, as I understand, my remote repository was ahead of the local one so pulling changes is needed before pushing again. So this issue can be fixed by merging the changes made on the remote branch with the changes made locally. 

    Git commands used to troubleshooting:

    ```
    git push --help
    git pull origin main

    ```

    Reference: [FreeCodeCamp | Ihechikara Vincent Abba](https://www.freecodecamp.org/news/error-failed-to-push-some-refs-to-how-to-fix-in-git/)

    <details>
    <summary>Click here to see Git error below</summary>
    <br>

    ![Git Error](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/git-error.jpg)


    </details>

## Testing Tools

- [W3C HTML](https://validator.w3.org/)
- [W3C CSS](https://jigsaw.w3.org/css-validator/)
- [Ui.dev](https://ui.dev/amiresponsive)
- [Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.)
- [Wave.org](https://wave.webaim.org/)
