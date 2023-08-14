# action-templates

## Actions are now under development and are not tested until further notice

### Configuration
Actions need input values of `app` and `url`

#### App
App variable defines under what name should be the apps be tracked. This name should be same for all pipelines regarding same code.

#### Url
Internet endpoint which accepts Pelorus webhook data.

### Example of usage

```yaml
name: Send-Data
on: push
jobs:
    check-committime-template:
        runs-on: ubuntu-latest
        steps:
            - uses: ./committime_template 
              with: 
                  app: "GitHub-test"
                  url: "http://pelorus.endpoint.com

```
