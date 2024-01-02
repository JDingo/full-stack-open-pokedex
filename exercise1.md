Hypothetical situation where there is an application being worked by about 6 people. Used language is Python. The application is in active development and will be released soon.

> Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked? You can search for the answers by google.

Linting is a code analysis tool used for flagging problematic code points, such as bugs, errors and style convention deviations. For Python, there are a variety of linters. Some are single linters, such as `pylint`, and some are multiple linters packaged into one, such as `Flake8`. There are linters for both logical and stylistic linting.

Testing includes the validation and verification of the program's functionality. In the context of CI, testing can be applied automatically as a part of the pipeline to ensure the functionality of the program. For testing, `pytest` is an example of a testing tool for Python.

In general, building is the step of preparing the software to run on the platform it's intended to run in. For Python, there isn't a need for a build setup at all. However, there are methods for packaging a Python project to a _Distribution Package_, which is a versioned archive file which includes all Python packages, modules, and other release files. For packaging, a _build backend_ is required. Some examples of Python build backends are `flit` and `hatch`.

> What alternatives are there to set up the CI besides Jenkins and GitHub Actions? Again, you can ask google!

In addition to Jenkins and Github Actions, there are other CI environments, such as Amazon's AWS CodePipeline, Bitbucket Pipelines, and Microsoft's Azure Pipelines.

> Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?

Based on the given information, cloud-based environment would be the more suitable solution.

In order to make the decision regarding which setup would be the best, information about the project, possibility of specific hardware requirements, and team environment are needed. Self-hosted environments are more costly, but allow for more tailored resources and support multiple teams. An example situation would be if there were multiple teams working on the same project. Cloud-based solutions are generally more suitable to small to medium software projects, simpler to set up and possibly more cost-effective, but are limited in resources and customizability.
