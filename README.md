__If you see this message on Master branch, it means the Jenkins builds were successful(test#2)__

# Sparta NodeJs Sample APP DevEnv and CI
This repo will be a dev env you can copy and setup by running vagrant up

# Pre-Requisites 
- [Vagrant](https://www.vagrantup.com/downloads.html) 
- [Virtual Box](https://www.virtualbox.org/wiki/Downloads)
- [Ruby (language not IDE)](https://www.jetbrains.com/ruby/promo/?gclid=CjwKCAiA8Jf-BRB-EiwAWDtEGrHnzaQQ8c12NPrRbN8zrPI-TaFz5HEtSIrcOni-ZEbqJad6B0Bn-RoCajYQAvD_BwE)
- a lightweight IDE, such as [Visual Studio Code](https://code.visualstudio.com/download)

# Instructions and step by step
1. Clone this repo
2. Run `vagrant up` in your terminal in that location
3. go to `192.168.10.100` in your browser to see the homepage for the jsnode app
4. this should also work on `192.168.10.100`
5. if you go to `192.168.10.100:3000` this should also be available there
6. if you go to `192.168.10.100/fibonacci/{}` where {} is any number you should see the fibonacci page is also working. 
8. finally, if you go to `192.168.10.100/posts` you should see a posts page if the DB is working properly. 

# Jenkins how to read from a different branch 

## How to create and push to a new branch using GitBash
To create a branch type the following in bash, in a tracked directory 
```bash
git checkout -b <branch>
```

changing to an existing branch
```bash
git checkout <branch>
```

commit to branch as normal 
```bash
git add . 
git commit -m "comment"
```

once committed you can push specific branches to origin 
```bash
git push origin <branch>
```