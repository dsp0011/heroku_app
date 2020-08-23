# Installatiion process and notes 🌴


### INSTALLATION
The following plugins were installed:
  - JDK
  - Maven
  - Heroku

------------------
### HEROKU
The following steps were performed while setting up and experimenting with Heroku:
   - Heroku was installed 
   - A getting-started app was cloned by the use of git
   - The app was deployed by the use of heroku
   - The logs are viewed with the command : heroku logs --tail
   - Heroku has a plaintext file called Procfile, declaring commands to be executed upon start
   - "heroku ps" is used to chech dynos (free dyno, monthly hour quota, sleeps after 30 min)
      - heroku "ps:scale web = n" can be used to scale up/down
   - The starting app has a pom.xml file declaring dependencies
     -  Heroku reads this file and dependencies are installed by the use of mvn clean install
   - Heroku apps can be run locally with the command "heroku local"
   - Short tutorial on git version control
   - The database tutorial also showed how to connect a database to the app  


# Technical issues  🍔

There were no techincal issues encountered as most of the programs (Maven, JDK) have already been installed. Installation of Heroku went smooth, as its well described in its website.


# Validation 🌵

Maven and JDK was working from before, it was only updatedto the most recent versions. This was verified by following the Heroku tutorial, which required building the project with maven and running it both locally and on a dyno.

# Pending Issues 🎨

There are no pending issues at this point. 



