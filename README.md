# About this repo
This repo serves as a catalogue of all Nuumi.ai-related projects. Other projects are added as sub-modules to this repo. And necessary documentations are also added here.
Submodules in this repo include the following listed ones. Some of them may need special access. If you think it's related to your work, please contact Cheng Shen (shenchg126@gmail.com) for access.

# Development guides
For each project, you are suggested to follow the same steps to set up dev environment and make commits to keep our code base clean and ordered:
1. Fork the repo to your own personal Github repo. For example if I'd like to work on Perseus, I would fork it from `nuumi-ai` to `SCandium`.
2. Set up local repo by cloning the personal github repo:
```
git clone git@github.com:SCAuFish/Perseus.git
```
3. Now the remote `origin` branch is set to `git@github.com:SCAuFish/Perseus.git`, but we also need to keep track of the repo under `nuumi-ai` and make sure we are in sync with other people's changes, therefore we do:
```
git remote add upstream git@github.com:nuumi-ai/Perseus.git
git remote
# You should see two remote pointers `origin` and `upstream`
```
4. Sync local master branch with upstream
```shell
git checkout master
git pull upstream master
```
5. Now if I want to do some developments, I check out from master branch
```shell
git checkout -b add-new-feature
# Developments, testing, etc.

git pull upstream master # Before creating PR for the new changes, make sure other people's changes are synced

git push origin add-new-feature # push changes to forked repo
```
6. Create PR in `nuumi-ai/Perseus` repo, https://github.com/nuumi-ai/Perseus/pulls, to merge the changes from `SCandium/Perseus:add-new-feature` branch.

# Projects
## Perseus
* Repo link: https://github.com/nuumi-ai/Perseus

## Recommender System Competition 2022 
* Repo link: https://github.com/nuumi-ai/Recommender-System-Competition-2022