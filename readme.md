# DComEX Software and Workflow Catalogue

This repository is a "living document", for recording the software tools and workflows developed in the DComEX project.

## Adding a new software tool or workflow
Each software tool and workflow is recorded in a markdown document in the respective `software` and `workflows` directories.

1. for the repository
2. copy the template in the appropriate directory to a file
3. edit the copy
4. make a pull request with your proposed changes, or ask @bcumming @ to merge your tool for you.

an example workflow to add a new software tool called "Frobulator"

First, fork the repository so that you have your own fork under your github account (called `your-github-handle` below).

Then clone your fork, and add the template. The workflow for doing this from the command line on Linux or MacOS is:

```
git clone git@github.com:${your-github-handle}/software-catalogue.git
cd software-catalogue
# create a branch for your changes
git checkout -b add-frobulator
cp template.md frobulator.md
... edit frobulator.md with your preferred text editor ...
git add frobulator.md
git commit -m 'add Frobulator software to the catalogue'
git push origin add-frobulator
```

Then go to the github page https://github.com/DComEX/software-catalogue and make a pull request via the web interface.
