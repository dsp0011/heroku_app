## Technical problems during installation JPA 🗿
Quite a few problems were encountered during this assignemnt, including:

-  Changing java version 
   -  The version of java used in the global environment did not meet the   requirements specified by Apache Derby server. In order to fix it, global variables had to be adjusted.


-  Experiment 1 problems
   - There were issues installing javax.persistence.jar. The latest version of eclipselink did not have the neeeded .jar, as it has been changed to a different one. In order to fix it, Intelij's auto import assistance was used
   - There were also different compilation errors, which included requiring to specify derby's .jar file for the project and adjusting some of the names of classes and packages in the persistance.xml file, as naming was slightly different than that from the tutorial


- Experiment 2 problems:
  - The main challenge with experiment 2 was to figure out how to use JPA properly and also figurting out how to access the database, which was automatically created by the JPA. The content of database tables could be simply inspected by SQL queries, but it was more difficult to find the proper way of accessing meta-information of the database. In the end, the database was accessed directly with the ij command provided by derby, rather than trying to execute SQL statements from the main class in order to view it

---

## Link to the assignemt 🧿
  Note that the main class used in experiment 1 was overwritten when testing experiment 2 
  https://github.com/dsp0011/DAT250LAB2

---
## Explanation on how the database was accessed 🎈
  The database was accessed by Derby's IJ command. The following tables were created:

  - ADDRESS
  - ADDRESS_PERSON
  - BANK
  - BANK_CREDITCARD
  - CREDITCARD
  - PERSON
  - PERSON_ADDRESS
  - PERSON_CREDITCARD
  - PINCODE 

---