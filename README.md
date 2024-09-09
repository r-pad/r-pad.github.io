# Making changes to the website 
1. ALL changes must be done through github via creating a new branch, making modifications, and then requesting a pull request. Admin will then verify locally and then merge the request. 
1. There are 2 ways to make modifcations. One way is directly through the github page online, or the second way is to locally make changes on your local machine by installing Jekyll on Linux. Minor addition such as adding members photo or publications can be done online through github site without having to locally setup Jekyll.
2. Make changes!


## (Online) Adding or updating the members page
1. Create a new branch with a short description of the change when starting out your work. You can do so by clicking on `master` tab down button, click `view all branches`, and then click `new branch`.
1. Upload a SQUARE 1:1 ratio headshot photo under img/members directory directly through github website. It has to be a square photo or the circle headshot will become an awkward oval. Commit changes to upload.
2. Add an entry to `members.md` directly through the github website -- navigate to the file and click edit file.
   1. Copy paste an existing members item and update.
   2. Commit changes.
3. If you want to make changes to the slideshow of lab photos, update the bottom section of `members.md` and upload image under img/lab directory.
3. Double check syntax and correct file directory, and then create a pull request to the `master` branch of `iamlab.github.io` and NOT `r-pad.github.io`.
4. Notify Mark Lee (MoonRobotics@cmu.edu) about the pull request.

## (Online) Adding a publication
1. If you haven't done so already, create a new branch with a short description of the change when starting out your work. You can do so by clicking on `master` tab down button, click `view all branches`, and then click `new branch`.
2. Upload the cover photo or gif of your research under `pics`. Commite changes to upload.
3. The publications page is updated by updating `_data/pubs.yaml file`. `The publication.md` reads the data from the yaml file and displays it.
4. Add an entry to `_data/pubs.yaml file`.
   1. Indentation matter in yml format, so pay careful attention to match the existing style EXACTLY. Especially when copying over Bibtex, make sure tab indentation is correctly aligned like existing items.
   3. Get the Bibtex from Google Scholar. 
   4. Embed the video link from youtube right click video, and paste the entire embedding info.
   5. You can ignore the tags. It existed for previous lab website to tag key research areas and publications together.
5. Notify Mark Lee (MoonRobotics@cmu.edu) about the pull request.

# (Locally) Setup Jekyll to make bigger changes to the website

## Setup and develop on Linux (Recommended)

1. Clone the GitHub repo by `git clone git@github.com:r-pad/r-pad.github.io.git`. 
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`. 
1. Change the working directory to the `r-pad.github.io` folder. 
1. Run `bundle clean` to clean up the directory (no need to run `--force`). 
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll serve -P 4000 -l --livereload-port 8080` to generate the HTML and serve it from `localhost:4000`. 

More documentations can be found [here](https://jekyllrb.com/docs/). 

### If encountering installation issues of Ruby:
1. Ubuntu and Ruby versions needs to match correctly. In my experience, Ubuntu 20.04 did not work with apt package installation because it installed Ruby 2.7 and Ubuntu 20.04 required Ruby 3.x. In such cases, install Ruby using Rbenv as shown in the 2nd method [here](https://phoenixnap.com/kb/install-ruby-ubuntu).

## Setup on Windows

If the following command does not Network in Windows PowerShell
```
docker run -d -p 4000:4000 -p 25003:25003 --name beautiful-jekyll -v "$PWD:/srv/jekyll" beautiful-jekyll
```
Try the following
```
docker run -d -p 4000:4000 -p 25003:25003 --name beautiful-jekyll -v "$(PWD):/srv/jekyll" beautiful-jekyll
```

# (Locally) Adding or updating the members page
1. First set up local development for Jekyll listed above.
2. Add an entry to `members.md`.
   1. Copy paste an existing members item and update.
   2. Upload a SQUARE 1:1 ratio headshot photo under img/members directory. It has to be a square photo or the circle headshot will become an awkward oval.
3. Check your changes running the server on your local machine and viewing the site at localhost:4000 .
4. Commit and push your changes.
5. If you want to make changes to the slideshow of lab photos, update the bottom section of `members.md` and upload image under img/lab directory.

# (Locally) Adding a publication
1. The publications page is updated by updating `_data/pubs.yaml file`. `The publication.md` reads the data from the yaml file and displays it.
2. Add an entry to `_data/pubs.yaml file`.
   1. Indentation matter in yml format, so pay careful attention to match the existing style EXACTLY. 
   2. Upload the cover photo or gif of your research under `pics`.
   3. Get the Bibtex from Google Scholar. 
   4. Embed the video link from youtube right click video, and paste the entire embedding info.
   5. You can ignore the tags. It existed for previous lab website to tag key research areas and publications together.


# For lab website maintainers
1. The members page is updated by directly modifying members.md .
1. The publications page is updated by updating `_data/pubs.yaml file`. `The publication.md` reads the data from the yaml file and displays it. There are instructions at the top on how to enter a new publication. 
1. Most of the work of being the website admin is approving member's pull requests to update the publications or members. We haven't opened up master branch access to all members as a way to check any updates before they are pushed. To make a new lab maintainer, add them as a member to the iamlab-cmu.github.io repository and set their role as Admin.

# Credit to CMU r-pad lab
Thank you for providing the template and helping us out!

# Credit to the template: Beautiful Jekyll

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/daattali/20)
[![Gem Version](https://badge.fury.io/rb/beautiful-jekyll-theme.svg)](https://badge.fury.io/rb/beautiful-jekyll-theme)

> *Copyright 2019 [Dean Attali](https://deanattali.com)*

**Beautiful Jekyll** is a ready-to-use template to help you create an awesome website quickly. Perfect for personal sites, blogs, or simple project websites.  [Check out a demo](https://deanattali.com/beautiful-jekyll) of what you'll get after just two minutes.  You can also look at [my personal website](https://deanattali.com) to see it in use, or see examples of websites other people created using this theme [here](#showcased-users-success-stories).

**If you enjoy this theme, please consider [supporting me](https://www.paypal.me/daattali/20) for developing and maintaining this template.**

<p align="center">
  <a href="https://www.paypal.me/daattali">
    <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" />
  </a>
</p>
