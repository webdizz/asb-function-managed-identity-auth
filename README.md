# asb-function-managed-identity-auth
POC to understand how to connect to Azure Service Bus using Managed Identity instead of credentials

## Steps to reproduce
1. Create Azure Function App `msi-func-poc`
2. Create Azure Service Bus `msi-asb-poc`
3. Create Topic in ASB `msi-poc-sbt`
4. Perform configuration according to instruction provided here https://docs.microsoft.com/en-us/azure/azure-functions/functions-identity-based-connections-tutorial-2

Note: Use `MSIServiceBusConnection` instead of `ServiceBusConnection`
5. Deploy Function App `npm run deploy`