# Configure Git pulgin on Jenkins
Git is one of the most popular tools for version control system. you can pull code from git repositories using jenkins if you use github plugin. 


#### Prerequisites
1. Jenkins server 

#### Install Git on Jenkins server
1. Install git packages on jenkins server
   ```sh
   yum install git -y
   ```

#### Setup Git on jenkins console
- Install git plugin without restart  
  - `Manage Jenkins` > `Jenkins Plugins` > `available` > `github`

- Configure git path
  - `Manage Jenkins` > `Global Tool Configuration` > `git`

########33creating a repo in git ############3
or create a new repository on the command line
echo "# new-new" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/gaellesimo/new-new.git
git push -u origin master
