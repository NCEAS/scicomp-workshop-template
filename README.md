# NCEAS Scientific Computing Workshop - Template

## Repository Explanation

This repository is the template for workshops offered by NCEAS Scientific Computing Support (SciComp) Team. This repository (and by extension, future workshops' repositories) creates a website with [Quarto](https://quarto.org/) meaning that web pages can be written with Markdown syntax. Following the steps below when creating a new workshop repository guarantees a consistent structure and aesthetic across all workshops (i.e., a consistent "brand").

## To Make a New Workshop Repository:

1.  **Fork** this repository to your GitHub profile

2.  **Rename** the repository by replacing "template" with 1-2 words about the workshop content

    -   E.g., "scicomp-workshop-github", "scicomp-workshop-tidyverse", etc.

3.  **Transfer ownership** of the repository to **someone who can make public repositories** on the [NCEAS GitHub Organization](https://github.com/NCEAS)

    -   Likely Julien Brun [brunj7](https://github.com/brunj7)

4.  **Create content** for the workshop in separate .qmd files

    -   Note that you'll need to add the names of each file to the "\_quarto.yml" file for the pages to be included in the Quarto website

5.  **Render content** by running `quarto render` in the *Terminal*

6.  **Deploy** the website with GitHub Pages

    -   A\) On the repository's GitHub page, click "Settings"
    -   B\) In the left sidebar, scroll down to "Pages" (under the "Code and Automation" subheading)
    -   C\) In the dropdown that says "None" select "main"
    -   D\) In the dropdown that says "/ (root)" select "/docs"
    -   E\) Click "Save"
    -   F\) Copy the link that produces
    -   G\) Paste the link into the "About" section of the repository to make it easier to find later

------------------------------------------------------------------------

### Background on Creating a Website with Quarto

**Note that this *is not* related to the above instructions on how to create a new workshop from this template**. This is included just "for your information" in case you are curious.

There are several paths to [creating a website with Quarto](https://quarto.org/docs/websites/#:~:text=Quarto%20Websites%20are%20a%20convenient,rendering%20options%2C%20and%20visual%20style.) but this one was created by doing the following:

I. Create a GitHub repository with a README and .gitignore

II\. Run `quarto create-project myproject --type website` in the *Terminal* - Note that "myproject" should be the same as your repo name or you'll need to drag some files around

III\. Create a file called ".nojekyll" by running `touch .nojekyll` in the *Terminal*

IV\. That's it!
