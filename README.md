# website-template

This is a template for creating a Quarto web site using RStudio.

To use it effectively you need to know how to push and pull from GitHub to RStudio using the Git panel buttons, which requires a working GitHub personal access token (PAT). If you don't have one setup, following [these instructions](https://happygitwithr.com/https-pat.html#tldr in *Happy Git and GitHub for the useR* to set one up. (In short you will create a token for HTTPS and store it using **gitcreds**.)

## ABSOLUTE ESSENTIALS

*If you have any difficulties or have feedback of any kind, please file an issue or communicate through [Discussions](https://github.com/jtr13/website-template/discussions).*

### Copy this template (GitHub)

- [ ] 1. Click the green "Use this template" button above. (You need to login to GitHub to see this option). Choose the "Create a new repository" option. DO NOT FORK THE REPO. Choose a descriptive name for your repo based on your content. (Unlike when you fork a repo, you get to choose the name. If you change your mind before you do any work, delete your new repo and start over.) Leave the "Public" option checked or else GitHub Pages won't work.

### Set up Pages (GitHub)

- [ ] 1. On the home page of your repo, click Settings. Click the "Pages" section on the left. In the **Build and Deployment** section, set **Source** to "Deploy from a branch" (Classic Pages experience) and **Branch** to **main** with **/docs** folder. Click Save. Above the **Build and Deployment** section, a box will appear with your book's URL. Copy the URL. (Note that sometimes there is a delay until your book actually appears at that URL. You do not need to wait on the page. If it doesn't appear after a few minutes, make a change and commit it to trigger a GitHub Pages build.)	

- [ ] 2. Click the gear button near "About" on the home page of the repo and check the "Use your Github Pages website" box under "Website". 

### Copy the repo link (GitHub)

- [ ] 1. Click the green Code button and copy the link under HTTPS. It should have the format: `https://github.com/[USERNAME]/[REPO NAME].git`

### Clone the repo (RStudio)

- [ ] 1. Clone your new repo with *File, New Project..., Version Control, Git* in RStudio. You will need to paste the link from the previous step in the Repository URL box.

### Edit some key files (RStudio)

- [ ] 1. Edit the all caps info in  `_quarto.yml` to your info.

- [ ] 2. Edit `index.qmd` as appropriate.

- [ ] 3. Edit `projects.qmd` as appropriate.

### Render the web site (RStudio)

- [ ] 1. Install **quarto** following the instructions here: https://quarto.org/docs/get-started/. If you already have it, update to the most recent version. 

- [ ] 2. Render the web site locally by clicking the "Build" tap on the right and then "Render Website"

- [ ] 3. Use `browseURL("docs/index.html")` to view your site locally (or just open `docs/index.html` in a browser).

- [ ] 4. If it looks good, commit and push all changed files to GitHub. 

(You will need to repeat steps 2 and 4 every time you wish to update the book online.)

### Next steps

- Choose a theme from [https://bootswatch.com/](https://bootswatch.com/) and replace "cerulean" in `_quarto.yml` with your prefered theme.

- Add additional tabs/sections by creating new `.qmd` files and listing them in `_quarto.yml` under `projects.qmd`.

### Additional features

Please consult the official guide to **quarto** web sites: [https://quarto.org/docs/websites/](https://quarto.org/docs/websites/)

### Edit README	(GitHub or RStudio)

Once you've completed these steps, delete the content of this **README** and add a short description of your project with a link to the book URL. It would be appreciated if you add the following to the end:	

*This repo was initially generated from a Quarto template available here: https://github.com/jtr13/website-template.*

(And starring the repo would be nice too!)

