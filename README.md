# SAM Quick Commands List
- `sam init` : guided steps to create a new SAM stack using cloud formation.
- `sam build` : builds application artifacts and prepares the deployable cloud formation
- `sam deploy --guided` : deploy application to was
- `sam sync --watch` : Modify and sync application changes
- `sam delete` : Delete application flow AWS Cloud


## Testing Changes
- **Hit Rest Endpoint via API Gateway** : Copy the API Gateway url and run from Postman
- **Directly Invoke Lambda Function** : `sam remote invoke [LambdaFunctName] --stack-name [sam-stack-name]`
- **Locally test lambda function** : `sam local invoke`
- **Locally deploy API Gateway** : `sam local start-api`

## Troubleshooting Steps
- **List stacks available** : `aws cloudformation list-stacks --stack-status-filter CREATE_COMPLETE`
