## Usage

### Basic Usage

After downloading, simply edit the `.astro` and `.md` files included with the template in a code editor to make changes. To preview the changes you make to the code, run `npm run dev`.

### Walkthrough

Follow the steps to [Fork](https://github.com/Developer-Student-Club-UoA/portfolio-website-workshop?tab=readme-ov-file#creating-and-deploying-a-portfolio-on-github-and-netlify) this repository using the instructions found in the parent repository.

Open the repository using IDX, or on your local machine with your favorite text editor.

Run the code using `npm run dev` in the terminal -- you should see the contents of the webpage on `localhost:4321`.

#### Changing Text

First we want to run the code using `npm run dev`, make sure you've got a page that looks like this:

![image](https://github.com/user-attachments/assets/54fb5d00-8164-49cd-b063-46a0a0a83c81)

To customise this, we can start by taking a look under `src/pages`. This folder includes the code for all your pages, routed by filename.

Open the `index.astro` file -- this corresponds to the home page.

![image](https://github.com/user-attachments/assets/624bccbc-92e9-4159-a7ca-443602536509)


Under the `Hero` component, you can edit the text on *lines 32 and 33* to your liking. Save the file and the change should be reflected on the browser.

![image](https://github.com/user-attachments/assets/80a297f9-06d4-49e5-8f41-486ebc7aaa51)

You can change the image by replacing `public/assets/portrait.jpg` with your own image.

![image](https://github.com/user-attachments/assets/dd12f637-de1d-49e4-8412-f677be4535fe)

To edit your skills, you want to open to skills component in `src/components/Skills.astro` and edit the corresponding text. The `/components` folder will hold all the components, which are the building blocks to the website.

Icons are defined using svgs in `IconPaths.ts`.

#### Other pages

In the `about.astro` file, we'll change the About Section. We recommend writing something about your interests, career objectives, skills, and maybe even hobbies.

You can add a new page just by creating a new `.astro` file under the pages folder, using the same template.

For each page, you can change the `title` and `description` prop for the BaseLayout component. These edit the title and description tag for each page.

![image](https://github.com/user-attachments/assets/05cc52d3-1efc-45ea-9b18-6e3075b0b48f)

If you want to change the default title and description tags, you can do so in the `layouts/BaseLayout.astro` Component.

#### Nav and Footer

Now take a look at the `Nav.astro` component under the `/components` folder. You can replace the placeholder `[Your Name]` on *line 21*, and you can also add or remove links from the navbar by editing the `textLinks` array on line 5.

You can also edit the footer with the `Footer.astro` file; you can replace the text with whatever you want, and also edit the links to your socials.

#### Adding Projects

Now let's take a look at the projects page. You will notice a few dummy projects. Click on one of them to see what it looks like.

![image](https://github.com/user-attachments/assets/ee1bd91b-d04f-4f3b-8cd0-7906233b4c1a)

To edit these pages, let's take a look at the files under `src/content/projects`. The pages are dynamically generated based on the content in these files. Try editing the content of one of the files, adding a new file using the same template, or deleting a file to see your changes.

The img property takes in images from `public/assets`. You can replace the placeholder images with more relevant ones.

The text uses markdown syntax, an example better utilising this is in `project4.md`.

#### Contact

Finally, let's update what email people should contact you at.

Open the `components/ContactCTA.astro` file, and replace the `mailto:me@example.com` to your own mailing address.


>Note: Be aware that this constitutes putting your email on the internet. You probably already have it available on other social media platforms but if you are not comfortable with the idea of putting your personal email out there then we recommend deleting the contact section.


#### Styling
Finally, you can open the `src/styles/global.css` file to view the project wide styling.

The main stuff you might want to change is the accent colours on *lines 19 to 22*, and font on *lines 74 to 77*.

#### Styling
Now commit your changes! You can do this by running the following commands:

```
git add .

git commit -m "My First Commit!"
```


### Extras

Of course, you can customise your portfolio and add virtually anything you want. If you want to do this, we recommend looking at the more comprehensive Astro Documentation at https://docs.astro.build/en/basics/astro-components/.

### Deployment
To learn about how to deploy your newly created portfolio on netlify, please return to the parent repo and follow the [Deployment Instructions](https://docs.astro.build/en/basics/astro-components/) there.
