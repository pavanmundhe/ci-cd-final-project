# CI/CD Final Project: Counter Service

This repository contains the Counter Service project for the Coursera **Continuous Integration and Continuous Delivery (CI/CD)** course.

The project uses Python, Flask, and Redis, with automated linting and unit tests through GitHub Actions. It also includes Tekton task definitions for running lint and test steps in an OpenShift pipeline.

## Project setup

In the Skills Network lab, run:

```bash
bash bin/setup.sh
```

Then open a new terminal so the Python virtual environment is activated.

## Continuous integration

The GitHub Actions workflow runs flake8 and the nose test suite on pushes and pull requests to `main`.

## Tekton tasks

The `.tekton/tasks.yml` file defines cleanup, lint, and test tasks for the OpenShift pipeline.

## License

Licensed under the Apache License. See [LICENSE](LICENSE).
