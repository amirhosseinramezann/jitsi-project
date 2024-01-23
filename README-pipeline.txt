- The stages section defines the order in which the stages will run: build, test, deploy to production, deploy to preview:(We could add other stage for deploy and other test solution)

- The build stage compiles and packages the application using the mvn package command.
- The test stage runs the tests using the mvn test command. this command checked the following items:
1-Compile Source Code
2-Compile Test Code
3-Execute Tests
4-Generate Test Reports
5-Check for Failures
- The deploy stage is a placeholder for your deployment steps. You can add the necessary commands to deploy your application to your desired environment. This could include copying artifacts to a server, updating configurations, etc.

Notice:
the deploy to preview stage is dependence on test stage, and also the deploy to production stage is dependence on both of test and preview stage and Due to high sensitivity, deployment is done manually.
