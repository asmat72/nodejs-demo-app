node.js Demo App This is a simple demo app written in node.js to demonstrate how to create and run a basic web server.

Prerequisites Node.js (version 24 or above) npm (Node Package Manager) Getting Started Clone the repository: git clone https://github.com/asmat72/nodejs-demo-app.git Navigate to the project directory: cd nodejs-demo-app Install the dependencies: npm install Run the app: npm start Open a web browser and go to http://13.201.136.246:3000 Functionality The app listens on port 3000 When you visit http://13.201.136.246:3000 in a web browser, the app will return "Hello from Node.js!" When you visit http://localhost:8080/about in a web browser, the app will return "This is a simple demo app written in node.js"
Deployment You can use AWS Instance for Docker to deploy this app to a production environment using the provided Dockerfile. Here's an example of how you can set up a pipeline to deploy the app to AWS Instance
Set up an AWS account if you don't have one already.
In the pipeline, configure the necessary environment variables like AWS.
In the pipeline, you can configure the tasks of the pipeline to build the container image, then push it to a container registry like AWS Instance, then deploy it to the production environment.
In the release pipeline, you can configure the necessary steps to deploy the image to the production environment. This can include steps to create or update the necessary resources, like the container instance, and configure any necessary environment variables or secrets.
After you configure the pipeline, you can trigger the pipeline to build and deploy the application to the production environment.
It's important to keep in mind that the specific steps will depend on the specific configuration of your application and the environment you are deploying to. Make sure to review the azure-pipelines.yml file and adapt it to your specific needs.
You can trigger the pipeline to deploy the app to the production environment. You can also set up continuous integration and continuous delivery (CI/CD) so that the pipeline automatically runs whenever new code is pushed to the repository.
By using Azure Pipelines, you can automate the process of building, testing, and deploying the app, making it easy to maintain and update the app in the production environment.
