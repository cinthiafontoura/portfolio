# Portfolio

Cinthia Fontoura Portfolio is a site for those who are looking to hire me as a front-end software developer to joy their team and bring a project to life. Users of this site will be able to see some of my projects live and check the code, know more about me, which technologies I'm using or studying, contact me and follow me on social media and hopefully hire me!

The live website can be found at [Portfolio](https://cinthiafontoura.com).

PS - This website was created as the first assessment at Code Institute and received the MERIT grade. You can check all the [previus commits on the original code repository](https://github.com/cinthiafontoura/cinthia-fontoura-portfolio).

![responsive](https://user-images.githubusercontent.com/80278757/157774385-20d15644-0823-494f-ae1d-6276a7cf8513.png)



## Features

* **Navigation**
  - Fixed navigation bar includes links to the Projects, About and Contact sections to allow easy navigation through the page. 
  - The logo make it easy back to homepage without scrolling up.  
  
![navigation](https://user-images.githubusercontent.com/80278757/157774697-d9a78bc0-c8ea-4f33-9146-2790d12b46f7.png)



* **The Header**
  - A quick introduction tells who I'm and what I do with a button that goes to the contact section to facilitate communication and a gif representing me. 
  - A Resume button that opens the link to my CV on a new tab showing to the user my professional path and education. 
  
![intro](https://user-images.githubusercontent.com/80278757/157774716-ebc1b4b8-5ef6-4a84-91fd-7a1a9bdedee5.png)


* **Projects Section**
  - A brief description of each website project, the technologies used, buttons linking to the live project and code on GitHub, and an image showing what the responsive website looks like.
  - The icons are just illustrative, all technologies are in the description.
  
![projects](https://user-images.githubusercontent.com/80278757/157774772-1af914cc-979f-4c3b-9460-a8ac84333c9f.png)




* **About Section**
  - A photo of my head, a description of me and what I know and a button to download my CV.
  - In this section, the user will know where I came from, what I did to live until now and how I decide to move to the tech sector, some technologies that I have studied and they can download my CV for future consultation.
  - All icons have a title attribute to make accessible to screen readers as described in the [Font Awesome documentation](https://fontawesome.com/docs/web/dig-deeper/accessibility#auto-accessibility-with-kits).

![about](https://user-images.githubusercontent.com/80278757/155027291-86677484-2db4-4d77-b331-e7f397e63e75.png)


* **Contact Section**
  - A simple form that collects  Name, Email and Message for users that wants to get in touch with me.
  - The form is working using Netlify forms. The steps to use are as follow:
    - Add **name** and **data-netlify="true"** attributes to the element **form**. 
    - You can read the documentation here [Forms setup](https://docs.netlify.com/forms/setup/)
  
![contact](https://user-images.githubusercontent.com/80278757/155027300-62d70c6d-1949-474f-af2c-808cfcbe34dd.png)


* **The Footer**
  - The footer section includes links to social media and email to encourage users to keep connected.
  - All links open in a new tab.
  
![footer](https://user-images.githubusercontent.com/80278757/155013571-a4a81c91-8f39-4689-8d46-5a8e2b891d63.png)


* **Form feedback page**
  - A response page saying thank you to those that sent a message in the form with a link back to the portfolio website.
  - This page it's essential to give the user feedback about what happens when they click on the "Send" button.

![thank-you](https://user-images.githubusercontent.com/80278757/155611575-ac14306c-7c4e-4d9a-aa5f-a02f6879c24e.png)



## Testing

* I've tested that this page works in Chrome and Firefox (mobile and desktop versions).
* I've confirmed that this project is responsive on all screen sizes using dev tools.
* I confirmed by testing with users that the text of all sections is readable and easy to understand.
* I've confirmed that the form works, requires entries in every field and the submit button works.

### Validator Testing

  * **HTML** 
    - No errors were found when passing throught official W3C Validator.

  * **CSS**
    - No errors were returned when passing through the Jigsaw.
  
  * **Accessibility**
    - I confirmed that the colours have enough contrast and fonts chosen are easy to read, and all links, icons and images have descriptive text for screen readers running it through Lighthouse in Chrome DevTools.

    - **Desktop**

       ![lighthouse-desktop](https://user-images.githubusercontent.com/80278757/155611377-5fc53857-4da7-474d-887e-9ff30803ec9e.png)

    - **Mobile**

       ![lighthouse-mobile](https://user-images.githubusercontent.com/80278757/155611357-38f4ae37-b919-4fff-825d-3aa920aaa42f.png)


### User Experience 
  * Users got confused when the link to the live site in the Portfolio project opened the same webpage in another tab. To fix this, I removed the button of this project that gives them access only to the code on GitHub. I also change the colour of the Live Site button to provide more emphasis to the code of each project.
  * Mobile users found it difficult to read justified text. To solve, I aligned the text to the left.
  * I fixed the navigation bar on top of the desktop version and on the bottom for mobile to guarantee that the navigations links are easier to access by small hands. 

     
### Bugs and Errors

  * **Solved**
    - Because this site was built just using HTML and CSS and I used the action="mailto:email" attribute the form show a security error. I solved this issue by deploying in Netlify and using their built-in form handling.
    - When I first passed through the W3C Validator all anchors elements were inside the buttons tags resulting in errors. So I removed and the errors are gone. 
    - All colours were changed to be more accessible for those who have a visual deficiency.
    - The images in the Portfolio section was background images using two divs and positioning, resulting in a broken style on medium and smaller screens and impossible to detect by screen readers. I've solved using Adobe Photoshop to create the image and add them to the HTML using img element and alt attribute.
    - After implementing an arrow up button to help users goes to the top of the page I realize that the buttons don't work because I've added the id attribute in the fixed navigation. I changed the location of the id to the body element to fix the issue.

  * **Unfixed**    
    - No unfixed bugs.
 
### Improvements to the code
  * **Implemented**
    * Change the classes names and start using the BEM Methodology to make the code easier to follow.
    * Reorganise all CSS elements in alphabetical order to make the maintenance faster and more logical.

  * **To implement**
    * Using a gif in the hero animation is causing damage to the performance for desktop and mobile versions, the better way to prevent this is using a video instead.
    * For the mobile performance increase is necessary to reduce the size of the images. 

 
     
## Deployment

The site was deployed to Netlify pages. The steps to deploy are as follows:
   - In the Netlify overview click on **Add new site**
   - Choose **Import an existing project** on the dropdown menu
   - Click on the GitHub button to connect to the Git provider
   - Chose the repository of the project that you want to deploy
   - Click on **Deploy site** and after a few seconds, you will have access to the URL of the deployed site.
   - Go to **Domain settings** > **Options** > **Edit site name** to change the site name and personalize the URL.
 
 The live website can be found at [Cinthia Fontoura Portfolio](https://cinthiafontoura.com).
  
 
## Credits

* Support of documentation in [W3schools](https://www.w3schools.com/).
* BEM methodology in [GetBEM](http://getbem.com/introduction/).
* Wireframe made using Figma [check here](https://www.figma.com/proto/3AfX32lUP6UvdqDZnaKQ6o/Cinthia-Fontoura-Portfolio?page-id=0%3A1&node-id=0%3A1&starting-point-node-id=1%3A2&scaling=min-zoom)
* Icons from [Font Awesome](https://fontawesome.com/)
* Code for the fixed navigation found on [stackoverflow](https://stackoverflow.com/questions/2861247/center-aligning-a-fixed-position-div).
* Colour palette create on [Addobe Color](https://color.adobe.com/create/color-wheel).
* Images created and resized using Adobe Photoshop.
* The images in the navigation, header and thank-you page was created using [picrew website](https://picrew.me/image_maker/338224).
* Favicon generated on [Favicon](https://favicon.io/)
