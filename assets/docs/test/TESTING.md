# Hand Embroidery Testing

![Site Mockup](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/mockup/site-mockup2.jpg)


---

## Site Functionality Testing
- __HTML & CSS Validation__

    HTML and CSS code have been tested and validated by using: [W3C HTML](https://validator.w3.org/) and
[W3C CSS](https://jigsaw.w3.org/css-validator/). Result screenshoots following these links: [HTML Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-HTML-Validator.jpg), [CSS Validation](https://github.com/anav-dev/hand-embroidery/blob/main/assets/docs/test/W3C-CSS-Validator.jpg)

- __Links, Buttons, Form, Images, Content__

    In order to ensure the proper functionality of this single-page site, the following aspects have been tested manually: 

    1. Buttons: Work and have same format.
    2. Contact Form & Success Message: Work correctly.
    3. Images: properly displayed.
    4. Icons: Open correct site in a different tab.
    5. Links: Redirect to corresponding site/section.
    6. Paths: Set properly, no broken paths.
    7. Typos: absence of any typing error.
   
    
    The bellow table shows manual tests performanced:

    | Action | Expected Behaviour | Result |
    | :---         |     :---:      |          ---: |
    | Click Home, About, Materials, Gallery navbar links   | Redirect to corresponding section     | Pass    |
    | Click navbar Contact icon  | Redirect to Contact section     | Pass    |
    | Click logo image   | Redirects to Home page     | Pass    |
    | Click welcome section button  | Redirect to About section     | Pass    |
    | Check all site images   | Images are properly displayed    | Pass    |    
    | Click footer social media icons   | Redirect to corresponding social media site     | Pass    |
    | Click footer About Us links   | Redirect to corresponding section     | Pass    |
    | Click footer Follow Us links    | Redirect to corresponding social media web     | Pass    |
    | Click content typos  | No typos found     | Pass    |
    | Submit form with invalid fields  | Required field message pops up     | Fail    |
    | Submit form with valid fields  | Success message is displayed, User redirect to CI form page     | Pass    |
   
   
  



> [!NOTE]
> Note about Contact form fixed required issue.

## Responsiveness Testing
- __Devices__

[Ui.dev](https://ui.dev/amiresponsive)
 
## Accessibility Test Testing

[Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.)
[Wave.org](https://wave.webaim.org/)

## Browsers Testing

## Testing Tools

- [W3C HTML](https://validator.w3.org/)
- [W3C CSS](https://jigsaw.w3.org/css-validator/)
- [Ui.dev](https://ui.dev/amiresponsive)
- [Lighthouse](https://developer.chrome.com/docs/lighthouse#:~:text=Lighthouse%20has%20audits%20for%20performance,or%20as%20a%20Node%20module.)
- [Wave.org](https://wave.webaim.org/)