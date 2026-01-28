# machinelearning-envsetup

# 1.create a master branch in the repository otherwise main branch created  by default

git clone https://github.com/SaralaSewwandi/machinelearning-envsetup.git

cd machinelearning-envsetup/

git branch

echo "# machinelearning-envsetup" >> README.md

git init

git add README.md

git config user.email "saralasewwandi@gmail.com"

git config  user.name "Sarala"

git commit -m "first commit"

git branch -M master

git remote add origin https://github.com/SaralaSewwandi/machinelearning-envsetup.git

git push -u origin master


# Clear all existing docker objects to set up a cleaned docker environment

sudo docker stop -vf $(sudo docker ps -aq)

sudo docker rm -vf $(sudo docker ps -aq)

sudo docker system prune

sudo docker system prune - - volumes

sudo docker system prune -a --volumes

sudo docker rmi -f $(sudo docker images -aq)

  
