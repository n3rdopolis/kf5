This is a meta-repo for all KDE Frameworks. KDE Frameworks 5 has split into multiple repositories.
This adds all of them as git submodules so they can all be cloned and build as one, just like when it was in kdelibs.

I used the cmake files

How to download:
git clone https://github.com/n3rdopolis/kf5.git
cd kf5
git submodule sync --recursive
git submodule init
git submodule update --recursive --force
git pull
