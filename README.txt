This is a meta-repo for all KDE Frameworks. KDE Frameworks 5 has split into multiple repositories.
This adds all of them as git submodules so they can all be cloned and build as one, just like when it was in kdelibs.

I used the cmake files

How to download:
git clone https://github.com/n3rdopolis/kf5.git
cd kf5
git submodule sync --recursive
git submodule init
git submodule update --recursive --force --remote
git pull

and then run 
git pull
git submodule update --recursive --force --remote

to update to the latest KDE modules if you ever need to. This works on Git 1.8.2 and later, where submodule branches are supported


If you have an older version of git than 1.8.2, to update all the submodules you will need to run 
git submodule foreach git checkout master

if you need to rebuild
