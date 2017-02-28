# The ICAPS 2017 conference website. #
Designed by Kristie Taylor-Muise based on Halcyonic by HTML5 UP.

## Instructions for submitting updates ##
These are rather draft instructions, but they should serve as a loose guide.

### Clone the ICAPS2017 repository and set up your local repository ###
1. Sign up for Github
2. Go to https://github.com/ICAPS2017/icaps2017.github.io and click the 'Fork' button in the upper right.  This should create and bring you to your own copy of the ICAPS website repository.
3. Use git to clone your repository
4. Make your edits (your website is under workshops/SPARK/ )
5. Run 'jekyll serve' in the base directory of the repository, which should build the site and launch a local web server at http://localhost:4000/ so that you can test your changes
6. Use 'git commit ...' and 'git push' to push your changes back to the website
7. Use https://github.com/ICAPS2017/icaps2017.github.io/pulls to create a "Pull request", which will notify us that your changes are ready to apply, and we'll log on to merge them into the main site. I've created an example pull request here:
https://github.com/ICAPS2017/icaps2017.github.io/pull/1
8. Mak and I will be notified and approve the changes to the site, at which point they'll go live.


### Set up a remote tracking branch ###
After you've cloned the ICAPS on GitHub and set it up on your local machine,  you should add a remote repository for tracking changes to the main site:
 ```
$ git remote add icaps git@github.com:ICAPS2017/icaps2017.github.io.git
```
You only need to do this once for your local repository.

### Branch to make your edits ###
Use git-fetch to update the remote repository, and then create a new branch for the pull request you plan to make:
```
$ git fetch icaps
$ git checkout -b <branch-name> icaps/master
```
Edit your files normally.  You can test your changes by running `jekyll serve` from the base directory (icaps2017.github.io), which will start a webserver on http://localhost:4000

If you add a new file, remember to add it with `git add`.  Commit your changes with `git commit`,  and push it back to GitHub with `git push`:
```
$ git add <path-to-new-file>
$ git commit -am <useful but terse change description>
$ git push origin
```
You should repeat this part of the procedure for each new pull request.




