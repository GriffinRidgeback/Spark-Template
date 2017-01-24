# Spark-Template
This repository houses work I did to create a template project for future Scala and/or Spark work.

## .gitignore
Select __Scala__ as the language and the .gitignore will contain SBT and Scala IDE-specific settings

# Scala IDE
It can be obtained from [here](http://scala-ide.org)

# Create a project
File-> New -> Project -> Maven project
Supply values for group ID and artificat ID

# pom file changes
Update to include the spark dependency

## Errors
Project configuration is not up-to-date with pom.xml. Select: Maven->Update Project... from the project context menu or use Quick Fix.
To fix, right-click on project, select Maven -> Update Project

# Add Scala Nature to this project
Right click on project -> configure - > Add Scala Nature.
This adds the Scala Library Container
