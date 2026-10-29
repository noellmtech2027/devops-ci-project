\# DevOps CI Project



\## Project Title



CI Pipeline Basics with GitHub Actions



\## Technologies Used



\* Python

\* Pytest

\* Git

\* GitHub

\* GitHub Actions



\## Description



This project demonstrates a basic Continuous Integration (CI) pipeline using GitHub Actions.



The project contains a simple Python application with automated tests. Whenever code is pushed to the GitHub repository, GitHub Actions automatically sets up the Python environment, installs the required dependencies, and runs the tests.



The CI pipeline was also tested by intentionally introducing a failing test. GitHub Actions detected the failure, and after the test was corrected, the pipeline successfully passed again.



\## Project Structure



```text

devops-ci-project/

│

├── app.py

├── test\_app.py

├── requirements.txt

├── .gitignore

└── .github/

&#x20;   └── workflows/

&#x20;       └── ci.yml

```



\## Application



The Python application contains simple functions for:



\* Adding two numbers

\* Greeting a user

\* Multiplying two numbers



Automated tests are written using Pytest to verify these functions.



\## Setup Instructions



1\. Clone the repository:



```bash

git clone https://github.com/noellmtech2027/devops-ci-project.git

```



2\. Navigate to the project:



```bash

cd devops-ci-project

```



3\. Install dependencies:



```bash

python -m pip install -r requirements.txt

```



4\. Run the application:



```bash

python app.py

```



5\. Run the tests:



```bash

python -m pytest

```



\## CI Pipeline



The GitHub Actions workflow is defined in:



```text

.github/workflows/ci.yml

```



The workflow:



1\. Is triggered when code is pushed to the `master` branch.

2\. Checks out the repository code.

3\. Sets up Python 3.10.

4\. Installs the dependencies from `requirements.txt`.

5\. Runs the automated tests using Pytest.



\## CI Failure Demonstration



To demonstrate how CI detects problems, a test was intentionally changed to an incorrect expected value.



The pipeline detected the failing test and the GitHub Actions workflow showed a failed run.



The test was then corrected and pushed again. GitHub Actions automatically ran the tests again and the pipeline successfully passed.



This demonstrates how CI can automatically detect problems in code changes.



\## GitHub Repository



https://github.com/noellmtech2027/devops-ci-project



