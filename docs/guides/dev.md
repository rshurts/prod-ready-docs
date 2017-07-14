# Development Guide

Provide documentation to quickly on-board developers, so that they can begin contributing code and introducing changes into the deployment pipeline.


### Setup {#setup}

Include step-by-step instructions for cloning the code, setting up the product, getting access, and verifying the environment is working correctly.


### Code Standards {#code-standards}

Document the coding standards, including code styles and how to run and setup any linting or formatting tools necessary to adhere to the code style.

> **Tabs Versus Spaces**
>
> A lot of time can be spent debating code style, but don't let perfection prevent progress. Choose a style and just use it. Where possible, adopt community best-practices like [airbnb's JavaScript eslint config](https://www.npmjs.com/package/eslint-config-airbnb) or [Python's PEP-8](https://www.python.org/dev/peps/pep-0008/). If the language provides a canonical formatting tool, like `go fmt` or `terraform fmt`, use that.

Describe the use of version control and any branching or merging strategies or naming conventions to meet the code standards.

### Code Reviews {#code-reviews}

Outline the code review process and what the expectations for a good code review are. Detail how to provide and respond to feedback. If pull requests are used, document how to create and close them.


### Testing {#testing}

Document the frameworks being used for unit, integration, and end-to-end (e2e) testing and how to run the tests. Include any metrics being tracked, like code coverage, and how to file a bug when one is found. Proper testing helps ensure a quality product and creates a "safety net" when refactoring. 


### Deployment Pipeline {#deployment}

Describe the build system and deployment process, including descriptions and links to the different environments and build machines. Provide information for troubleshooting and debugging failed builds so a developer can quickly get the build back in the "green."
