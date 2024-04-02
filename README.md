a. Pre-Requisits
  1. Install Docker on Machine
  2. docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home jenkins/jenkins [to run Jenkins using Docker].
  3. Open your web browser and navigate to http://localhost:8080 to access the Jenkins web interface.
  4. GitHub Account and JDK - Latest version

b. Creating a Simple Pipeline
  To create a new Pipeline in Jenkins, we’ll start by creating a new project.

  1. From the Jenkins dashboard, click the “New Item” link in the sidebar.
  2. Enter a name for your project ("Jenkins-Deployment") and select “Pipeline” as the project type.
  3. Click the “OK” button to create the project.

c. Adding Version Control
  One of the key benefits of using Jenkins Pipelines is the ability to version control your Pipeline definition.
  Let’s add a GitHub repository to our project and store our Pipeline definition there.

  1. Create a new repository on GitHub, named “Jenkins-Deployment”.
  2. In the project configuration page, scroll down to the “Pipeline” section and select “Pipeline script from SCM” from the “Definition” dropdown.
  3. Select “Git” as the SCM, and enter the URL of your GitHub repository (https://github.com/shreekanth7899/Jenkins-Deployment.git).
  4. Select the branch.
  5. Click the “Save” button to save the Pipeline configuration.

d. Pipeline Script for Jenkins
  1. Create a file called "Jenkinsfile" and add the pipeline script
  2. Save the file on GitHub repo and build it on Jenkins

e. Check build history to check recent changes
