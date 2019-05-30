# 2019-05-16_git-workflows

Let's say you want to use the code in this repo. Three use cases: 
1. **Use code as is**  - e.g.:  you just want to rerun a query 
2. **Modify the code for a different purpose**  - e.g.: change the site from LGH to RHS
3. **Suggest improvements to the code**  - e.g: to change the definition of what an "episode" is, to more accurately track patient flow

## Proposed workflow 1: Start with forking 
1. Fork the repository on GitHub.com
2. Clone the repository and save as a folder on your computer. You can save anywhere; it doesn't have to be a shared folder. 
3. Best practice: never do "development" on the master branch. The master branch is supposed to always be functional, production-ready code. Before mkaing changes to the code, create a development branch. For example, if you want to change a query to account for transfers between sites, create a branch named "transfers". 
3. Work on the code files as you normally would. Commit changes with good summaries of what you've changed. When you're sure that your development branch works, you can merge it into your master branch. 
4. Now you want to merge from your master to the "upstream" master. To do that, go to the upstream master on GitHub.com and click on new pull request. 

## Proposed workflow 2: Start with branching 
1. Instead of forking, start by cloning and saving the folder. 
2. *Before making any changes*, create a development branch. 
3. [to be decided] 
reference: https://gist.github.com/seshness/3943237 


## Things to test
1. What happens if the upstream fork renames the repo on the cloud? 
2. What happens if we rename specific files in the upstream repo? 
3. How to pull from upstream repo into a fork? 
    - https://help.github.com/en/articles/merging-an-upstream-repository-into-your-fork
4. How do we resolve merge conflicts? 
5. How frequently should collaborators be merging from upstream into their fork/branch? 
