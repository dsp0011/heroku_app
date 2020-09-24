## Techincal Problems and Summary

There were two main issues for this project. The first issue was making maven imports work for the counter example (https://github.com/selabhvl/dat250-sparkjava-counter). Running regular mvn clean install command in the command prompt seemed to not install the dependencies correctly. In order to fix it I had to use an intelij maven plugin that fixed dependencies automatically.

The second issue was converting the results fromt the http put and delete requests into a string (tasks in my implementation we defined as strings). In the end I've used JsonObject class to do it.

The implemenation for this Lab was fairly simple, it was done by expanding the already existing counter class. The methods that handle HTTP requests are very similar to the existing ones and a new class called Todo was added.

The todo class uses a list to store all the tasks. When the App class receives a http request /todo path it does the following:
 - if it's a POST request, it creates a new list from one provided in the request
 - if it's a PUT request, it adds an task to the list
 - if it's a DELETE request, it deletes given task from the list
 - if it's a GET request, it returns the list with all the tasks

Link to the code: https://github.com/dsp0011/DAT250LAB4