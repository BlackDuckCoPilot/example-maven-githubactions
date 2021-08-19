# Black Duck CoPilot Maven/GitHub CI Example

[![Actions](https://github.com/BlackDuckCoPilot/example-maven-githubactions/workflows/Java%20CI/badge.svg)](https://github.com/BlackDuckCoPilot/example-maven-githubactions/actions?workflow=Java+CI) [![Black Duck Security Risk](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-githubactions/branches/validation/badge-risk.svg)](https://copilot-valid.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-githubactions/branches/validation)

Shows a working setup for using Synopsys CoPilot to analyze the risk of project dependencies

## GitHub CI/CD Setup

The `.github/workflows/workflow.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- name: Upload to CoPilot
      run: bash <(curl -s https://copilot-valid.blackducksoftware.com/ci/githubactions/scripts/upload)
```
