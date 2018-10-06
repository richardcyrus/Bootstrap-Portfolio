# Bootstrap-Portfolio

Use Bootstrap to recreate your portfolio with the following items:

* A `.navbar`
* A responsive layout (remeber the grid, rows and columns are your friends)
    * On `xs` and `sm` screens, content should take up the entire screen.
    * On `md` and larger screens, you should have some margins on the left and right side of the screen.
        - Check out various sites on your mobile device versus your computer to see this in action!
* Responsive images.

## Bonus

Using Bootstrap, make a sticky footer and use sub-rows and sub-columns on your portfolio page.

* Your Bootstrap solution should minimize the use of media queries.

## Deploy

Deploy the Bootstrap-Portfolio as a GitHub Project Pages site and link to your main GitHub Pages site.

## Project Files and Folders

* Create a project folder named `Bootstrap-Portfolio`.
* In the `Bootstrap-Portfolio` project folder create the following directories:
    - `assets/images`
    - `assets/css`
* In the `Bootstrap-Portfolio` project folder create the following files:
    - `index.html`
    - `contact.html`
    - `portfolio.html`
    - `assets/css/style.css`.

# Project Setup Script

>**Note:**
>To execute the following, you will need to have the `hub` commanline utility installed.
>On macOS with Homebrew run `brew install hub`.

```bash
#! /usr/bin/env bash

# Define the Project Name and Folder Name.
PROJECT_NAME='Bootstrap-Portfolio'

# Define the parent location for the project files.
BASE_DIR="${HOME}/Projects/Homework"

# Define the complete project location.
PROJECT_DIR="${BASE_DIR}/${PROJECT_NAME}"

# Make sure the parent project directory exists
mkdir -p "${BASE_DIR}"

# Change to the parent project path.
cd "${BASE_DIR}"

# Create the local Git repository for the project.
hub init -g "${PROJECT_NAME}"

# Change into the project folder.
cd "${PROJECT_DIR}"

# Create the project repository on GitHub.
hub create "${PROJECT_NAME}"

# Add the project README
echo "# Bootstrap-Portfolio" >> README.md

# Create the project folder structure.
mkdir -p assets/{images,css}

# Create the files needed in this project.
touch {index,contact,portfolio}.html assets/css/style.css

# Add the project files to version control and push them to the GitHub
# remote repository.
git add . && git commit -m "Initial Project Setup"
git push -u origin master
```

# References

- The JavaScript snippet used to update the Copyright in the footer came from [Update Your Footer](http://updateyourfooter.com/ "Update Your Footer")

# Credits

- The profile photo was taken by my friend and fellow photographer Jeff Acker.

- Images on the Portfolio page were provided courtesy of [Lorem Picsum](https://picsum.photos "Lorem Picsum") and [Unsplash](https://unsplash.com "Unsplash").
- The following images from Lorem Picsum were used on the Portfolio page.
    - _Project_: Wire Frame
        - _Picsum Image_: [618](https://unsplash.com/photos/ypVM8PnygUo), _Author_: [Mika Ruusunen](https://unsplash.com/@mikaruusunen)
    - _Project_: Giftastic
        - _Picsum Image_: [373](https://unsplash.com/photos/i8CYGnoerR0), _Author_: [Jay Wennington](https://unsplash.com/@jaywennington)
    - _Project_: Rock, Paper, Scissors
        - _Picsum Image_: [817](https://unsplash.com/photos/ssrbaKvxaos), _Author_: [Alex wong](https://unsplash.com/@killerfvith)
    - _Project_: Train Scheduler
        - _Picsum Image_: [821](https://unsplash.com/photos/2TlAsvhqiL0), _Author_: [Eutah Mizushima](https://unsplash.com/@eutahm "Eutah Mizushima")
    - _Project_: Liri Bot
        - _Picsum Image_: [688](https://unsplash.com/photos/a_xa7RUKzdc), _Author_: [Benjamin Sloth Lindgreen](https://unsplash.com/@benjaminslothlindgreen "Benjamin Sloth Lindgreen")
    - _Project_: Word Guess
        - _Picsum Image_: [345](https://unsplash.com/photos/S_mEIfXRzIk), _Author_: [Mario Calvo](https://unsplash.com/@mariocalvo "Mario Calvo")
    - _Project_: Friend Finder
        - _Picsum Image_: [662](https://unsplash.com/photos/ILz31HBGEak), _Author_: [Caleb Ekeroth](https://unsplash.com/@calebekeroth "Caleb Ekeroth")
    - _Project_: Burger 2: The Sequel
        - _Picsum Image_: [1074](https://unsplash.com/photos/sseiVD2XsOk), _Author_: [Samuel Scrimshaw](https://unsplash.com/@samscrim "Samuel Scrimshaw")
    - _Project_: Clicky Game
        - _Picsum Image_: [366](https://unsplash.com/photos/6PF6DaiWz48), _Author_: [Rayi Christian Wicaksono](https://unsplash.com/@mumolabs "Rayi Christian Wicaksono")
    - _Project_: News Searcher
        - _Picsum Image_: [342](https://unsplash.com/photos/r4He4Btlsro), _Author_: [Steven Lewis](https://unsplash.com/@stevenlewis "Steven Lewis")
    - _Project_: News Fit to Scrape
        - _Picsum Image_: [1073](https://unsplash.com/photos/Oaqk7qqNh_c), _Author_: [Patrick Tomasso](https://unsplash.com/@impatrickt "Patrick Tomasso")

- The background image is from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns").
    - The image used on this site is [White Sand](https://www.toptal.com/designers/subtlepatterns/?s=white_sand), by [Atle Mo](http://www.atlemo.com "Atle Mo").
    - The images from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns") use the following [license](https://creativecommons.org/licenses/by-sa/3.0/ "Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)")

## The Unsplash License

All photos published on Unsplash can be used for free. You can use them for commercial and noncommercial purposes. You do not need to ask permission from or provide credit to the photographer or Unsplash, although it is appreciated when possible.

More precisely, Unsplash grants you an irrevocable, nonexclusive, worldwide copyright license to download, copy, modify, distribute, perform, and use photos from Unsplash for free, including for commercial purposes, without permission from or attributing the photographer or Unsplash. This license does not include the right to compile photos from Unsplash to replicate a similar or competing service.
