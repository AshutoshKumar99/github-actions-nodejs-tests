# Node.js CI Workflow

Author: Ashutosh Kumar
Date: 2023-09-25
Version: 1.0

## Description

This GitHub Actions workflow automates Node.js CI/CD for a Node.js project. It performs the following steps:

### Step 1: Check out the source code

The workflow starts by checking out the source code from the repository.

### Step 2: Set up different versions of Node.js for testing

It sets up different versions of Node.js (12.x, 14.x, 16.x) for testing. There would be 3 jobs for each Node.js version.

### Step 3: Perform a clean install of Node.js dependencies

The workflow performs a clean installation of Node.js dependencies using `npm ci`.

### Step 4: Cache and restore dependencies for faster builds

To speed up future builds, the workflow caches and restores dependencies using npm caching.

### Step 5: Build the source code

The source code is built as part of the workflow.

### Step 6: Run tests using different versions of Node.js

Finally, tests are run using the specified Node.js version.

## Workflow Configuration

The workflow is configured to trigger on every commit to the `main` branch and on pull requests targeting the `main` branch.

## Usage

To use this workflow, add the provided YAML configuration file (e.g., `.github/workflows/nodejs-ci.yml`) to your repository's `.github/workflows` directory.

## License

This workflow is available under the [MIT License](LICENSE).

---
For more information on GitHub Actions, see the [GitHub Actions documentation](https://docs.github.com/en/actions).

