#Clean Up Your Meteor Project

Inside your project folder you will find the hidden directory *.meteor*, which contains important data for Meteor to handle your project. It includes the database data and packages. This area maintains the best practices to have some control in your project and how to remove, purge and backup your data.

To entirely remove your collection data you can use this command.

````
$ meteor reset
````

According to the manual:

####meteor reset

Reset the current project to a fresh state. Removes the local mongo database.

This deletes your data! Make sure you do not have any information you care about in your local mongo database by running meteor
mongo. From the mongo shell, use show collections and db.collection.find() to inspect your data.

You can not run this while a development server is running. Quit all running meteor applications before running this.
