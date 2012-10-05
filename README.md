Maven-Multi-Module-Example
==========================

An example of a multi module maven project

Requires Maven 3.x to build.  To build, cd to root directory and then
    
    mvn clean install
    
This project has 4 modules.  The top level is the logical entity, and is the Maven Project.  There are four modules underneath this:

    api - the API module
    implementation - the Implementation module
    test-util - the Test Utilities module
    stand-along - an example of a stand alone implementation
    
It's best practice to create a seperate implementation module and then run with both the API and Implementation jars.  But I've included the stand-alone module to demonstrate how to package up everything into a single jar file using the Maven shade plugin.