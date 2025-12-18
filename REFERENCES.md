# References - Test-Driven Development for IDP

This document contains curated resources for learning Test-Driven Development (TDD) with Python and Azure SDK for Internal Development Platform (IDP) development.

## 📚 Table of Contents

- [Official Documentation](#official-documentation)
- [Books](#books)
- [Articles & Blog Posts](#articles--blog-posts)
- [Video Tutorials](#video-tutorials)
- [Online Courses](#online-courses)
- [Tools & Libraries](#tools--libraries)
- [GitHub Repositories](#github-repositories)
- [Related Learning Repositories](#related-learning-repositories)
- [Community Resources](#community-resources)

-----

## 📖 Official Documentation

### Python Testing

#### Pytest

- [Pytest Documentation](https://docs.pytest.org/) - Official pytest docs
- [Pytest Good Integration Practices](https://docs.pytest.org/en/stable/goodpractices.html)
- [Pytest Fixtures](https://docs.pytest.org/en/stable/fixture.html) - Comprehensive fixture guide
- [Pytest Parametrize](https://docs.pytest.org/en/stable/parametrize.html) - Parameterized testing
- [Pytest-mock Documentation](https://pytest-mock.readthedocs.io/) - Mocking in pytest

#### Python Testing Tools

- [unittest.mock Documentation](https://docs.python.org/3/library/unittest.mock.html) - Standard library mocking
- [Coverage.py](https://coverage.readthedocs.io/) - Code coverage measurement
- [tox Documentation](https://tox.wiki/) - Testing multiple Python versions

### Azure SDK for Python

#### Core Documentation

- [Azure SDK for Python](https://learn.microsoft.com/en-us/azure/developer/python/) - Main docs
- [Azure Identity](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme) - Authentication
- [Azure Core](https://learn.microsoft.com/en-us/python/api/overview/azure/core-readme) - Core functionality

#### Service-Specific SDKs

- [Azure Resource Management](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-resource-readme)
- [Azure Storage Management](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-storage-readme)
- [Azure Network Management](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-network-readme)
- [Azure Compute Management](https://learn.microsoft.com/en-us/python/api/overview/azure/mgmt-compute-readme)

#### Testing Azure SDK

- [Azure SDK for Python - Testing](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/tests.md)
- [Azure SDK Testing Guidelines](https://azure.github.io/azure-sdk/python_design.html#testing)

-----

## 📚 Books

### Test-Driven Development

#### Essential Reading

1. **“Test Driven Development: By Example”** by Kent Beck
- The original TDD book
- Step-by-step TDD examples
- Red-Green-Refactor cycle
- [Amazon Link](https://www.amazon.com/Test-Driven-Development-Kent-Beck/dp/0321146530)
1. **“Python Testing with pytest”** by Brian Okken (2nd Edition)
- Comprehensive pytest guide
- Fixtures, parametrization, plugins
- Best practices for Python
- [Pragmatic Bookshelf](https://pragprog.com/titles/bopytest2/python-testing-with-pytest-second-edition/)
1. **“Unit Testing Principles, Practices, and Patterns”** by Vladimir Khorikov
- Modern testing principles
- What to test and what to skip
- Mocking best practices
- [Manning Publications](https://www.manning.com/books/unit-testing)

#### Infrastructure Testing

1. **“Infrastructure as Code”** by Kief Morris (2nd Edition)
- Testing infrastructure code
- Patterns for reliable infrastructure
- [O’Reilly](https://www.oreilly.com/library/view/infrastructure-as-code/9781098114664/)
1. **“Continuous Delivery”** by Jez Humble and David Farley
- Deployment pipelines
- Automated testing strategies
- [Addison-Wesley](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912)

-----

## 📝 Articles & Blog Posts

### TDD Fundamentals

#### Introduction to TDD

- [Test-Driven Development (TDD)](https://martinfowler.com/bliki/TestDrivenDevelopment.html) - Martin Fowler
- [The Three Rules of TDD](http://butunclebob.com/ArticleS.UncleBob.TheThreeRulesOfTdd) - Robert C. Martin
- [TDD is Dead. Long Live Testing](https://dhh.dk/2014/tdd-is-dead-long-live-testing.html) - DHH (critical perspective)
- [Is TDD Dead? Discussion](https://martinfowler.com/articles/is-tdd-dead/) - Fowler, Beck, DHH

#### Python TDD

- [Getting Started with Testing in Python](https://realpython.com/python-testing/) - Real Python
- [Python Testing Best Practices](https://testdriven.io/blog/testing-best-practices/) - TestDriven.io
- [Effective Python Testing With Pytest](https://realpython.com/pytest-python-testing/) - Real Python
- [Testing Flask Applications](https://flask.palletsprojects.com/en/2.3.x/testing/) - Flask Docs

### Infrastructure Testing

#### Testing Infrastructure as Code

- [Testing Infrastructure as Code](https://www.infoq.com/articles/testing-infrastructure-as-code/) - InfoQ
- [TDD for Infrastructure](https://www.hashicorp.com/resources/test-driven-development-tdd-for-infrastructure) - HashiCorp
- [Testing Strategies for Infrastructure Code](https://www.thoughtworks.com/insights/blog/testing-strategies-infrastructure-code) - ThoughtWorks

#### Azure-Specific Testing

- [Testing Azure Functions Locally](https://learn.microsoft.com/en-us/azure/azure-functions/functions-develop-local) - Microsoft
- [Best Practices for Azure SDK](https://devblogs.microsoft.com/azure-sdk/best-practices-for-using-azure-sdk-with-asp-net-core/) - Azure SDK Blog
- [Testing Azure Resources with Terraform](https://www.hashicorp.com/blog/testing-azure-resources-with-terraform) - HashiCorp

### Mocking & Test Doubles

- [Mocks Aren’t Stubs](https://martinfowler.com/articles/mocksArentStubs.html) - Martin Fowler
- [Test Doubles — Fakes, Mocks and Stubs](https://blog.pragmatists.com/test-doubles-fakes-mocks-and-stubs-1a7491dfa3da) - Pragmatists
- [Mocking in Python](https://realpython.com/python-mock-library/) - Real Python
- [When to Mock](https://blog.cleancoder.com/uncle-bob/2014/05/10/WhenToMock.html) - Robert C. Martin

### Test Organization & Patterns

- [The Practical Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html) - Martin Fowler
- [Test Fixtures Done Right](https://itnext.io/test-fixtures-with-pytest-6e3e46bb4d14) - ITNEXT
- [Arrange-Act-Assert Pattern](https://automationpanda.com/2020/07/07/arrange-act-assert-a-pattern-for-writing-good-tests/) - Automation Panda
- [Given-When-Then](https://martinfowler.com/bliki/GivenWhenThen.html) - Martin Fowler

-----

## 🎥 Video Tutorials

### TDD Fundamentals

#### Introductions

- [Test-Driven Development in Python](https://www.youtube.com/watch?v=B1j6k2j2eJg) - ArjanCodes (45 min)
- [TDD: What It Is and What It Is Not](https://www.youtube.com/watch?v=llaUBH5oayw) - Dave Farley (15 min)
- [The Three Laws of TDD](https://www.youtube.com/watch?v=qkblc5WRn-U) - Robert C. Martin (60 min)

#### Practical Examples

- [Python TDD Workflow](https://www.youtube.com/watch?v=B1j6k2j2eJg) - mCoding (20 min)
- [Test-Driven Development in Python](https://www.youtube.com/watch?v=eAPmXQ0dC7Q) - Socratica (12 min)
- [TDD in Python with pytest](https://www.youtube.com/watch?v=ULxMQ57engo) - PyOhio (30 min)

### Pytest Deep Dives

- [pytest: Rapid Testing and Simple Scaling](https://www.youtube.com/watch?v=9LVqBQcFmyw) - Holger Krekel (90 min)
- [Pytest Features](https://www.youtube.com/watch?v=LX2ksGYXJ80) - PyCon (30 min)
- [Effective Testing with pytest](https://www.youtube.com/watch?v=dJAXS-D_0Rw) - EuroPython (45 min)

### Azure & Cloud Testing

- [Testing Azure Functions](https://www.youtube.com/watch?v=V3u1FGmZjso) - Microsoft (20 min)
- [Azure SDK for Python](https://channel9.msdn.com/Shows/Azure-Friday/Azure-SDK-for-Python) - Azure Friday (15 min)
- [Infrastructure Testing with Python](https://www.youtube.com/watch?v=Eu0vJB0cHqY) - HashiConf (40 min)

-----

## 🎓 Online Courses

### Test-Driven Development

#### Free Courses

- [Test-Driven Development](https://www.coursera.org/learn/test-driven-development) - Coursera (University of London)
- [Testing in Python](https://realpython.com/learning-paths/test-your-python-apps/) - Real Python Learning Path
- [Software Testing and Automation](https://www.edx.org/course/software-testing-and-automation) - edX (TU Delft)

#### Paid Courses

- [Test-Driven Development with Python](https://testdriven.io/courses/tdd-python/) - TestDriven.io
- [Testing Python Applications](https://www.pluralsight.com/courses/testing-python-applications) - Pluralsight
- [Python Testing Masterclass](https://www.udemy.com/course/python-testing/) - Udemy

### Azure & Cloud

#### Microsoft Learn

- [Introduction to Azure SDK for Python](https://learn.microsoft.com/en-us/training/modules/intro-to-azure-python/) - Free
- [Develop Python applications with Azure](https://learn.microsoft.com/en-us/training/paths/python-azure/) - Learning Path
- [AZ-204: Developing Solutions for Microsoft Azure](https://learn.microsoft.com/en-us/training/courses/az-204t00) - Certification prep

#### Other Platforms

- [Azure for Python Developers](https://www.pluralsight.com/paths/azure-for-python-developers) - Pluralsight
- [Python on Azure](https://www.linkedin.com/learning/paths/python-on-azure) - LinkedIn Learning

-----

## 🛠️ Tools & Libraries

### Testing Frameworks

#### Core Testing

- **[pytest](https://pytest.org/)** - Primary testing framework
  - `pytest-cov` - Coverage plugin
  - `pytest-mock` - Mocking utilities
  - `pytest-asyncio` - Async testing
  - `pytest-xdist` - Parallel testing
  - `pytest-bdd` - Behavior-driven development
  - `pytest-timeout` - Test timeouts

#### Specialized Testing

- **[hypothesis](https://hypothesis.readthedocs.io/)** - Property-based testing
- **[faker](https://faker.readthedocs.io/)** - Test data generation
- **[factory_boy](https://factoryboy.readthedocs.io/)** - Test fixtures replacement
- **[responses](https://github.com/getsentry/responses)** - Mock requests library
- **[vcrpy](https://vcrpy.readthedocs.io/)** - Record and replay HTTP interactions

### Mocking & Test Doubles

- **[unittest.mock](https://docs.python.org/3/library/unittest.mock.html)** - Standard library (built-in)
- **[pytest-mock](https://pytest-mock.readthedocs.io/)** - Pytest wrapper for mock
- **[responses](https://github.com/getsentry/responses)** - Mock HTTP responses
- **[moto](https://github.com/getmoto/moto)** - Mock AWS services (reference for patterns)

### Code Quality

#### Linting & Formatting

- **[black](https://black.readthedocs.io/)** - Code formatting
- **[ruff](https://docs.astral.sh/ruff/)** - Fast Python linter
- **[mypy](http://mypy-lang.org/)** - Static type checking
- **[pylint](https://pylint.org/)** - Code analysis
- **[isort](https://pycqa.github.io/isort/)** - Import sorting

#### Code Coverage

- **[coverage.py](https://coverage.readthedocs.io/)** - Coverage measurement
- **[pytest-cov](https://pytest-cov.readthedocs.io/)** - Pytest coverage plugin
- **[codecov](https://about.codecov.io/)** - Coverage reporting service
- **[coveralls](https://coveralls.io/)** - Coverage tracking

### CI/CD Testing

- **[tox](https://tox.wiki/)** - Test multiple environments
- **[nox](https://nox.thea.codes/)** - Flexible test automation
- **[pre-commit](https://pre-commit.com/)** - Git hook management
- **[GitHub Actions](https://docs.github.com/en/actions)** - CI/CD platform
- **[Azure Pipelines](https://azure.microsoft.com/en-us/products/devops/pipelines/)** - Azure CI/CD

### Azure Testing Tools

- **[azure-devtools](https://github.com/Azure/azure-sdk-for-python/tree/main/tools/azure-devtools)** - Azure SDK testing utilities
- **[azurite](https://github.com/Azure/Azurite)** - Azure Storage emulator
- **[azure-functions-core-tools](https://github.com/Azure/azure-functions-core-tools)** - Local Azure Functions testing

-----

## 💻 GitHub Repositories

### Example Projects

#### TDD Examples

- [python-tdd-exercises](https://github.com/garora/TDD-Katas) - TDD kata exercises
- [tdd-python-samples](https://github.com/testdouble/contributing-tests) - Real-world examples
- [pytest-examples](https://github.com/okken/pytest-examples) - Comprehensive pytest examples

#### Azure SDK Examples

- [Azure SDK for Python Samples](https://github.com/Azure-Samples/azure-samples-python-management) - Official samples
- [azure-python-labs](https://github.com/Azure-Samples/azure-python-labs) - Hands-on labs
- [azure-sdk-for-python](https://github.com/Azure/azure-sdk-for-python) - Source code with tests

#### Infrastructure Testing

- [terraform-compliance](https://github.com/terraform-compliance/cli) - BDD for IaC
- [terratest](https://github.com/gruntwork-io/terratest) - Go testing library (reference)
- [kitchen-terraform](https://github.com/newcontext-oss/kitchen-terraform) - Test Kitchen for Terraform

### Learning Resources

- [awesome-pytest](https://github.com/augustogoulart/awesome-pytest) - Curated pytest resources
- [awesome-python-testing](https://github.com/thecodercoder/awesome-python-testing) - Python testing resources
- [azure-dev-docs](https://github.com/MicrosoftDocs/azure-dev-docs) - Azure developer documentation

-----

## 🔗 Related Learning Repositories

### From learning-internal-development-platform Series

1. **[learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform)**
- Main overview repository
- Architecture and roadmap
- Links to all sub-repositories
1. **[learning-idp-python-azure-sdk](https://github.com/vanHeemstraSystems/learning-idp-python-azure-sdk)**
- Azure SDK fundamentals
- Authentication patterns
- Service-specific operations
1. **[learning-idp-platform-engineering](https://github.com/vanHeemstraSystems/learning-idp-platform-engineering)**
- Platform engineering concepts
- IDP architecture
- Backstage.io exploration
1. **[learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code)**
- Bicep and ARM templates
- Infrastructure patterns
- IaC best practices
1. **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)**
- Azure DevOps pipelines
- GitHub Actions
- Deployment automation

-----

## 👥 Community Resources

### Forums & Discussion

- [Python Testing on Reddit](https://www.reddit.com/r/python/search/?q=testing) - r/python discussions
- [Pytest Discussion](https://github.com/pytest-dev/pytest/discussions) - GitHub Discussions
- [Stack Overflow - pytest](https://stackoverflow.com/questions/tagged/pytest) - Q&A
- [Stack Overflow - azure-sdk-python](https://stackoverflow.com/questions/tagged/azure-sdk-python) - Azure SDK Q&A

### Slack & Discord

- [Python Community Slack](https://pythondev.slack.com/) - #testing channel
- [Azure Community Discord](https://discord.gg/azure) - Azure discussions
- [DevOps Chat](https://devopschat.co/) - DevOps community

### Blogs & Newsletters

#### Testing Blogs

- [Test Driven Development Blog](https://www.testdrivendevelopment.com/) - TDD articles
- [Pytest Blog](https://pytest.org/en/latest/blog.html) - Official pytest news
- [Real Python Testing Articles](https://realpython.com/tutorials/testing/) - Python testing tutorials

#### Azure Blogs

- [Azure SDK Blog](https://devblogs.microsoft.com/azure-sdk/) - Official Azure SDK updates
- [Azure Developer Community Blog](https://techcommunity.microsoft.com/t5/azure-developer-community-blog/bg-p/AzureDevCommunityBlog) - Community articles
- [Python @ Microsoft](https://devblogs.microsoft.com/python/) - Python at Microsoft

-----

## 📊 Useful Cheat Sheets

- [Pytest Cheat Sheet](https://gist.github.com/kwmiebach/3fd49612ef7a52b5ce3a) - Quick reference
- [Python Mock Cheat Sheet](https://nedbatchelder.com/blog/201908/why_your_mock_doesnt_work.html) - Common pitfalls
- [Azure CLI Cheat Sheet](https://learn.microsoft.com/en-us/cli/azure/reference-index) - Azure CLI commands

-----

## 🎯 Next Steps

After completing this learning path, continue with:

1. **[learning-idp-azure-compute](https://github.com/vanHeemstraSystems/learning-idp-azure-compute)** - Apply TDD to compute resources
1. **[learning-idp-azure-networking](https://github.com/vanHeemstraSystems/learning-idp-azure-networking)** - Network infrastructure testing
1. **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)** - Integrate tests in pipelines

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*
