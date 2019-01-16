# Build A Portfolio Website

With all of the projects you will be working on here at Lambda School, you will need somewhere to house them!  There is no better opportunity to learn and show off your skills than a beautiful portfolio website.  

You have the ability to write HTML, CSS, and responsive media queries.  You also know how to identify and write responsive units.  It's time to put that knowledge into action by reading someone else's code and adding your own flavor.  You will be building a portfolio website from a template found on [https://html5up.net/](https://html5up.net/).

## Project Set Up

### Follow these steps to set up and work on your project:

- [X] Create a forked copy of this project.
- [X] Add PM as collaborator on Github.
- [X] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [X] Create a new branch on the clone: `git checkout -b <firstName-lastName>`.
- [ ] Implement the project on the `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: `git push origin <firstName-lastName>`.

### Follow these steps to download your template and start the project:

- [X] Navigate here: [https://html5up.net/](https://html5up.net/)
- [X] Pick a template that represents you and download it to your local machine
- [ ] Unzip the code and copy the site to your git repository that you just set up
  * Note that we won't be utilizing the pre processed CSS structure, you can just ignore any folder with LESS or SASS (SCSS) in it.
- [ ] Work on the MVP requirements listed below

### Follow these steps for completing your project after your MVP is completed:

- [ ] Submit a Pull-Request to merge `<firstName-lastName>` Branch into master (student's Repo). **Please don't merge your own pull request**
- [ ] Add your Project Manager as a Reviewer on the Pull-request
- [ ] PM then will count the HW as done by merging the branch back into master.

## MVP Requirements

- [X] Study the code base and identify both responsive units and where media queries were used.  Take notes on anything that confuses you or interesting things you find.  Share this information in your standup meeting with your group

The template that I picked was overflow. This template
uses media queries to traslate CSS from desktop -> tablet -> tablet(portrait) -> and mobile. 

First, the code starts by setting the entire class .container to a width of 1140px. The .container class is applied to 5 article tags (feature 1, feature 2, portfolio, contact) so this means they will all have a fixed width of 1140px if on a very large screen.

The first two media queries deal simply with the width of our container.
1. max width 1680px, (desktop) set the width to 960px
2. max width 1080px (tablet), set the width to 95%
Why does he do px for desktop and % for tablet? Tablet is starting to introduce responsiveness. Once we get to screens 1080px and below, the container starts resizing smaller to 95% of 1080 (at 1080, would be 1026px but it depends on the viewport of your screen)

After about 300 lines of CSS, additional media queries that update the CSS for the .row class, which define two rows of images and my input area for the contact part.

Originally, there are 2 rows of images, 4 columns but the media queries size those rows so eventually its only 1 column of images
1. max width 1680px
2. max width 1080px
3. max width 840px
4. max width 736px

Finally, the media queries deal with:
1. max width 1680px- basic, header
2. max width 1080px- banner, header
3. max width 840px- basic, box, header, banner
4. max width 736 px (mobile)- basic, list, icons, menu, actions, button, box, header, banner, footer, poptrox

- [ ] Customize the template to you 
	- [X] Update the title tag match your name
	- [X] Update the place holder content throughout the template to your information
		* Some templates are much larger than others, you don't need to fill in every little div with information, just try to get the site representing you and your work 
		* You can use sites like [https://www.pexels.com/](https://www.pexels.com/) for free images to fill in place holders
		* Showcase projects you have worked on by providing some information and links to your git hub projects
- [X] Implement proper attribution: Attribution is required under the [creative commons license](https://html5up.net/license) that came with the website files you downloaded.  Be sure to provide attribution somewhere in the site.  The templates should already come with attribution found in most footers but double check to be sure.
- [ ] Host your website for the world to see. Follow the instructions found here [https://pages.github.com/](https://pages.github.com/).  Once you have hosted your web page, share it for your peers to see.  This is not a small feat!

## Stretch

- [ ] Study the JavaScript used in your template and see if you can tweak any of the behavior to see how it works
- [ ] Download another template and see if you can get the CSS preprocessor working on the project