# This is where we store our Services
# Here our repositories are just classes that will mediate the communication between our controller and our data.
# Our controllers won't need to know where the data comes from, and you can use more than one repository on a controller if you need to.
# The repositories must be separated by entities, and can almost always be based on their database tables.
# And inside it will contain all its functions that will request data from a local api or database.
# That is, if we have a user table that we will persist as, edit, add, update and delete, all these functions are requested 
# from an api, we will have a repository with this object of the api where we will call all the respective 
# functions to the user. So the controller does not need to know where it comes from, the repository being a 
# mandatory attribute for the controllers in this model, you should always initialize the controller with at - /repository
            