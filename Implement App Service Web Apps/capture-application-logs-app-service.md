## [Source: Capture application logs in Azure App Service](https://learn.microsoft.com/en-us/training/modules/capture-application-logs-app-service/)

### Question 1:
A developer is working on an ASP.NET Core application deployed to an Azure App Service on Linux. They need to log error messages. Which log levels will be captured in the Azure App Service logs?

- A) Verbose, Information, Warning, and Error
- B) Information and Error
- C) Error only
- D) All log levels (Critical, Error, Warning, Information, Debug, Trace)

<details>
  <summary>Show Answer</summary>
  <b>C) Error only</b>
</details>

### Question 2:
You have a Node.js web application running on an Azure App Service (Windows). You want to capture both standard output and standard error messages in the application logs. Which logging method should you use?

- A) `console.debug()` and `console.trace()`
- B) `console.log()` and `console.error()`
- C) `logger.LogInformation()` and `logger.LogError()`
- D) `System.Diagnostics.Trace.WriteLine()`

<details>
  <summary>Show Answer</summary>
  <b>B) `console.log()` and `console.error()`</b>
</details>

### Question 3:
Which Azure CLI command is used to enable verbose file system logging for an Azure App Service named "mywebapp" in the resource group "myresourcegroup"?

- A) `az webapp log enable --name mywebapp --resource-group myresourcegroup --level verbose`
- B) `az webapp log config --application-logging filesystem --level verbose --name mywebapp --resource-group myresourcegroup`
- C) `az appservice log config --application-logging filesystem --level verbose --name mywebapp --resource-group myresourcegroup`
- D) `az webapp log set --name mywebapp --resource-group myresourcegroup --level verbose`

<details>
  <summary>Show Answer</summary>
  <b>B) `az webapp log config --application-logging filesystem --level verbose --name mywebapp --resource-group myresourcegroup`</b>
</details>

### Question 4:
You want to store your Azure App Service application logs in Azure Blob storage. Which of the following statements is true?

- A) Blob storage logging is available for both Windows and Linux App Services.
- B) You must configure a retention period for blob storage logs.
- C) Blob storage logs are automatically deleted after 12 hours.
- D) Blob storage logging is only available for Linux based app services.

<details>
  <summary>Show Answer</summary>
  <b>B) You must configure a retention period for blob storage logs.</b>
</details>

### Question 5:
A developer needs to log detailed performance and usage data for a production ASP.NET application hosted on Azure App Service. Which Azure service would be most suitable for this purpose?

- A) Azure Metrics
- B) Azure App Service Diagnostics logs (filesystem)
- C) Azure Application Insights
- D) Docker logs

<details>
  <summary>Show Answer</summary>
  <b>C) Azure Application Insights</b>
</details>

### Question 6:
Your Azure App Service is running on a Linux host. What is the primary factor that determines the logging functionality available to your application?

- A) The IIS Web server configuration.
- B) The application's code framework.
- C) The Docker image used for the app's container.
- D) The Azure App Service plan tier.

<details>
  <summary>Show Answer</summary>
  <b>C) The Docker image used for the app's container.</b>
</details>

### Question 7:
An ASP.NET application running on a Windows Azure App Service uses the `System.Diagnostics.Trace` class for logging. Which method should be used to write an error message to the application logs?

- A) `Trace.LogCritical("Message")`
- B) `Trace.LogError("Message")`
- C) `Trace.TraceError("Message")`
- D) `Trace.WriteLine("Message")`

<details>
  <summary>Show Answer</summary>
  <b>C) `Trace.TraceError("Message")`</b>
</details>


---

**Deploy the web app**

```bash
az appservice plan create --name $appPlan --resource-group $resourceGroup --location $appLocation --sku FREE
az webapp create --name $appName --resource-group $resourceGroup --plan $appPlan --deployment-source-url $gitRepo
```
**Create a storage account**

```bash
az storage account create -n $storageAccount -g $resourceGroup -l $appLocation --sku Standard_LRS
```


**enable app logging to the file system**
```bash
az webapp log config --application-logging filesystem --level verbose --name <app-name> --resource-group <resource-group-name>
```
**Open log stream**
```bash
az webapp log tail  --resource-group <resource-group-name> --name contosofashions<NNNNNN>
```

**Download file system log files (does not include failed request traces only)**

az webapp log download --log-file \<_filename_\>.zip  --resource-group \<_resource group name_\> --name \<_app name_\>


**Create a new set of user-level credentials**
```bash
az webapp deployment user set --user-name <name-of-user-to create> --password <new-password>
```