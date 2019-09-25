# Black Duck CoPilot Maven/Travis CI Example

[![Travis CI](https://travis-ci.org/BlackDuckCoPilot/example-maven-travis.svg?branch=master)](https://travis-ci.org/BlackDuckCoPilot/example-maven-travis) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-travis/branches/master/badge-risk.svg)](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-travis/branches/master)

Shows a working setup for using Black Duck CoPilot to analyze the risk of project dependencies

## Travis CI Setup

The `.travis.yml` file has been modified to upload the generated data to Black Duck CoPilot:

```yaml
after_success:
  - bash <(curl -s https://copilot.blackducksoftware.com/ci/travis/scripts/upload)
```
