# CI/CD Final Project – Hit Counter Service

## Project Overview

This project was developed for the **CI/CD Tools and Practices** course by IBM Skills Network on Coursera.

The project demonstrates a Continuous Integration and Continuous Delivery (CI/CD) workflow for a Python Flask application called **Hit Counter Service**.

## Project Details

- **Project Name:** CI/CD Final Project – Hit Counter Service
- **Repository:** https://github.com/randq01/ci-cd-final-project
- **Programming Language:** Python
- **Web Framework:** Flask
- **CI Tool:** GitHub Actions
- **Pipeline Tool:** Tekton
- **Container Technology:** Docker / Buildah
- **Deployment Platform:** Red Hat OpenShift
- **Container Registry:** IBM Cloud Container Registry

## Continuous Integration (CI)

The GitHub Actions workflow is defined in `.github/workflows/workflow.yml`.

The CI workflow successfully completed, validating the project through automated checks.

## Automated Testing

The application was tested using automated unit tests and code coverage tools.

**Test Results:**
- 9 unit tests passed
- 99% code coverage
- Flake8 linting passed

## Tekton Pipeline

The Tekton configuration files are located in the `.tekton` directory.

The pipeline performs the following operations:

1. Clean up the workspace.
2. Clone the GitHub repository.
3. Run code linting.
4. Execute automated unit tests.
5. Build and push the application container image.

**Pipeline Result:** Successfully completed.

## Container Image

The application image was built using Buildah and pushed to IBM Cloud Container Registry.

Image:

`us.icr.io/sn-labs-h541969/ci-cd-final-project:latest`

## OpenShift Deployment

The application was deployed to Red Hat OpenShift.

Deployment name: `ci-cd-final-project`

The deployment started successfully, and the application returned HTTP 200 OK when tested through port-forwarding.

The OpenShift Service was connected to the application, and the public Route was admitted. Public access could not be verified because external connection attempts timed out.

## Project Results

The project successfully demonstrated automated CI testing, Tekton pipeline execution, container image creation, and application deployment to OpenShift.

## License

Licensed under the Apache License. See [LICENSE](LICENSE).