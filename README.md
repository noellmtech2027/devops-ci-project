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



The Python application contains simple functions with automated tests. Whenever code is pushed to the GitHub repository, GitHub Actions automatically installs the required dependencies and runs the tests.



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



The GitHub Actions workflow:



\* Runs whenever code is pushed to the `master` branch.

\* Runs for pull requests targeting the `master` branch.

\* Sets up Python 3.10.

\* Installs project dependencies.

\* Executes the automated tests using Pytest.



\## GitHub Repository



https://github.com/noellmtech2027/devops-ci-project



