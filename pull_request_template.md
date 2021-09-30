## Related Issue(s)
> Github issue related to the pull request

## Related PR(s)
> Other PRs related to the pull request

## Approach/Solution
> Describe how you are implementing the solutions. Include an animated GIF or screenshot if the change affects the UI (email documentation@wso2.com to review all UI text). Include a link to a Markdown file or Google doc if the feature write-up is too long to paste here.

## Release Note
> Brief description of the new feature or bug fix as it will appear in the release notes

## Documentation
> Link(s) to product documentation that addresses the changes of this PR. If no doc impact, enter “N/A”.

## PR Validation

### Changes to OpenAPI definition

- [ ] Added the below sentence into the `description` under `info` section of the OpenAPI definition file.

      `This is a generated connector from [API NAME AND VERSION](URL TO THE OPENAPI DOC OR VENDOR WEBSITE) OpenAPI Specification.`
      
- [ ] Added `x-ballerina-init-description` OpenAPI extension into the `info` section of the OpenAPI definition file describing the connector initialization details (ie: How to obtain authentication tokens)
- [ ] Added `x-ballerina-display` OpenAPI extension into the `info` section of the OpenAPI definition file mentioning the connector name and path to the connector icon as below.
      ```info:
        x-ballerina-display:
          label: <Connector Name>
          iconPath <Icon Path> ---> Path described at [Changes to connector module]
      ```
- [ ] Added proper description each API Key, if API Key authentication is defined in OpenAPI definition file 

### Changes to connector module

- [ ] Added license header at the top of each .bal file. 
- [ ] Added Package.md as per the guide [here]()
- [ ] Added Module.md for the generated module of the  connector as per the guide [here]()
- [ ] Created a directory called `resources` at the root of the generated connector and copied the connector icon there. Name of the icon file need to be `<connector-name>.svg`
- [ ] Added Ballerina.toml file with following information. Make sure keywords are added according to the following guide. 
   ```
  [package]
    license = ["Apache-2.0"]
    keywords = ["<key word 1>", "<key word 2>"]
    org = "ballerinax"
    name = "<connector-name>"
    repository = "https://github.com/ballerina-platform/ballerinax-openapi-connectors"
    version = "0.1.0-SNAPSHOT"
    authors = ["Ballerina"]

  [build-options]
   observabilityIncluded = true
   ```

### Verifying connector module

- [ ] Compiled the connector successfully with the targeted ballerina version. 
- [ ] Conducted smoke tests on the connector (Recommended when OpenAPI definition is obtain from an unofficial source)

## Security checks
 - [ ] Followed secure coding standards in http://wso2.com/technical-reports/wso2-secure-engineering-guidelines? 
 - [ ] Confirmed that this PR doesn't commit any keys, passwords, tokens, usernames, or other secrets? 

## Test environment
> List all JDK versions, operating systems, databases, and browser/versions on which this feature/fix was tested

