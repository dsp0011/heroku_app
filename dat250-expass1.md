# PROCESS



### INSTALLATION 🌴
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
