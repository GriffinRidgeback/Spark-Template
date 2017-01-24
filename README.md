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

<pre>
	<dependency>
		<groupId>org.apache.spark</groupId>
		<artifactId>spark-core_2.10</artifactId>
		<version>1.4.0</version>
	</dependency>
</pre>

## Errors
Project configuration is not up-to-date with pom.xml. Select: Maven->Update Project... from the project context menu or use Quick Fix.
To fix, right-click on project, select Maven -> Update Project

# Add Scala Nature to this project
Right click on project -> configure - > Add Scala Nature.
This adds the Scala Library Container

## When you hit this problem:
spark build path is cross-compiled with an incompatible version of Scala (2.10.0)
## You do this:
1. change the Scala version in the IDE: Right click on the project -> Scala -> set Scala installation or Right Click on the Scala Library Container -> Properties and choose Scala 2.10 (or the value that Spark needs)
2. Right-click on the project -> Maven -> Update Project

# Remove Scala Library Container from build path (Optional)
The following warning message appears:  _More than one scala library found in the build path_

Right click on the project -> Build path -> Configure build path and remove Scala Library Container.

# Update source folder src/main/java to src/main/scala
Right click -> Refactor -> Rename  to scala

Can do the same thing for test

# Clean and run
Project -> clean
Right-click on .scala file and Run As -> Scala Application
