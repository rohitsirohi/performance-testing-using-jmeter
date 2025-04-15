Main building blocks and element types in Jmeter

🔹 Test Plan
What it is: The root of your JMeter project. Think of it as the container that holds everything.
Use: Defines the overall structure of your test — includes thread groups, logic controllers, config elements, etc.
Extra: You can set variables and configure test-wide settings here.

🔹 Thread Groups
What it is: Represents a group of virtual users (threads).
Use: Specifies the number of users, how often they send requests, and how long the test should run.
Example: 100 users sending requests every second for 5 minutes.

🔹 Samplers
What it is: These are the actual actions (like sending HTTP requests, JDBC queries, FTP uploads).
Use: Simulates a user performing operations.
Examples: HTTP Request, FTP Request, JDBC Request, SOAP/XML-RPC Request, etc.

🔹 Config Elements
What it is: Provides config settings or variables to samplers.
Use: Used to set things like server names, default parameters, or database connection settings.
Examples: HTTP Request Defaults, CSV Data Set Config, JDBC Connection Configuration.

🔹 Listeners
What it is: Shows the results of your test.
Use: Collects and visualizes data in tables, graphs, trees, etc.
Examples: View Results Tree, Summary Report, Aggregate Report, Graph Results.

🔹 Timers
What it is: Adds delay between sampler executions.
Use: Mimics real-world user behavior where users don’t hit the server instantly after each request.
Examples: Constant Timer, Gaussian Random Timer, Uniform Random Timer.

🔹 Assertions
What it is: Used for validating responses.
Use: Checks if the response contains expected content, has the right response code, etc.
Examples: Response Assertion, Duration Assertion, Size Assertion.

🔹 Pre-Processors & Post-Processors
What they are:
Pre-Processors: Run before a sampler.
Post-Processors: Run after a sampler.
Use:
Pre: Set up data, modify requests (e.g. add headers, generate tokens).
Post: Extract data from responses (e.g. using Regular Expression Extractor).
Examples: BeanShell Pre/PostProcessor, Regular Expression Extractor, JSON Extractor.
