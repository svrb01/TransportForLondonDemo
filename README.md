# TransportForLondonDemo
Readme for TFL Demo Automation Framework 

This is to give an overview understanding of some of the development approaches
I have undertaken to successfully implement the test project also considering some of the future implementation.

- Firstly, Created a specflow project since the tests were to be written in gherkin style format,
and also to make use of srprofile file and generation of test report without having to use third party tools for report generation.
- While developing the framework, I considered making use of most of the Object oriented concepts for architecture, which will help us
to organise, mantain and understanding the code better.
- Framework consists of Actor/Actions, Features,Screens, Steps and Hooks.

  - Features would contain all the scenarios to test the application under test
  - Screens offer Page Object Modelling pattern where all the elements/objects of the screens are defined in classes
  - Steps contains the code for the feature files individual steps in the form of step definition classes and these are organised on the basis of screens
  - Hooks is a class which contains additional code apart from the step definition code. Here we can specify how we want to run our tests and also include any dependencies
    that would help whilst running the code like setting up the environment before and after scenario execution.
  - Actions - Are a way of defining methods on the basis of interactions (interacting with the control like setting a field or clicking on a button)
    and expectations (checking/verifying the result of interactions)

Note: Since the framework is developed using specflow project, it uses specrun to run the tests. Hence signing in to the free specflow account would be necessary.
I will attach a screenshot for the same.
Also, the feature files should be run using Test Explorer and the report is generated in Test Results folder
