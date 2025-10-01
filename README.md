# Node.js Demo App

This is a simple demo app written in Node.js to demonstrate how to create and run a basic web server.

- 📦 Prerequisites
  - Node.js (version 24 or above)
  - npm (Node Package Manager)

- 🚀 Getting Started
  - Clone the repository:  
      `git clone https://github.com/asmat72/nodejs-demo-app.git`
  - Navigate to the project directory:  
      `cd nodejs-demo-app`
  - Install the dependencies:  
      `npm install`
  - Run the app:  
      `npm start`
  - Open a web browser and go to:  
      `http://13.201.136.246:3000`

- ⚙️ Functionality
  - The app listens on port **3000**
  - When you visit `http://13.201.136.246:3000`, the app returns:  
      `"Hello from Node.js!"`
  - When you visit `http://localhost:8080/about`, the app returns:  
     `"This is a simple demo app written in node.js"`

- 📦 Deployment (Using AWS Instance + Docker)
     - You can deploy this app to a production environment using the provided Dockerfile.

- 🛠️ Pipeline Setup
  - Set up an AWS account if you don't have one already.
  - In the pipeline:
     - Configure necessary environment variables like AWS credentials.
     - Define tasks to:
       - Build the container image.
       - Push it to a container registry (e.g., AWS Instance).
       - Deploy it to the production environment.
     - In the release pipeline:
       - Add steps to create or update resources like the container instance.
       - Configure environment variables or secrets as needed.
     - After configuration:
       - Trigger the pipeline to build and deploy the application.

- 🔁 Continuous Integration & Delivery (CI/CD)
  - Set up CI/CD so the pipeline runs automatically whenever new code is pushed.
  - This ensures the app is always up-to-date and easy to maintain.

## 📌 Notes
- Specific steps may vary depending on your application and deployment environment.
- Review and adapt the `azure-pipelines.yml` file to match your setup.
