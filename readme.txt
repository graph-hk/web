git/# hongkongelectionstudy.github.io/home is built with Jekyll + Github Pages
# All the files are in ~/Google\ Drive/HKES/home/docs
#

### Show the page locally
# To render the file locally, in Terminal:

cd ~/Google\ Drive/HKES/home/docs

bundle add webrick 

bundle exec jekyll serve

# Then the site can be shown in localhost:4000 of any web browser

### Update Email
# When pushing to GitHub, make sure to remove the stored email. To do so, type the following line in terminal:

git config --global user.email "YOUR_NEW_EMAIL"

# To check if the email change is successful, type the following line:

git config --global user.email


### Update files on GitHub
# To update the GitHub page, in Terminal:

cd ~/Google\ Drive/HKES/home/docs
git add .
git commit -m '[update messages]'
git push -u https://[personal token from GitHub]@github.com/hongkongelectionstudy/home.git gh-pages

git push -u https://[personal token from GitHub]@github.com/graph-hk/web.git gh-pages

