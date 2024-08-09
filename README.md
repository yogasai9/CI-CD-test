# cicd-demo
CICD Demo using python-app
1.On Code Push: 
Whenever you push code changes to the main branch, the pipeline triggers automatically.
2.Build Stage:
The code is fetched from the repository.
Docker login happens using stored credentials.
Your application is built into a Docker image.
The image is pushed to your DockerHub repository (replace my-image with your actual image name).
3.Test Stage:
The code is again checked out from the repository.
A Python environment is set up.
Dependencies are installed from requirements.txt.
Tests are executed using pytest (replace pytest with your chosen test framework if different).
Code coverage is calculated using the coverage package.
