### Question 1:
Which Azure service is primarily used to store and query App Service File Audit Logs?

- a) Azure SQL Database
- b) Azure Blob Storage
- c) Azure Monitor Logs (Log Analytics)
- d) Azure Cosmos DB

<details>
  <summary>Show Answer</summary>
  <b>c) Azure Monitor Logs (Log Analytics)</b>
</details>

### Question 2:
What type of information is typically captured within App Service File Audit Logs?

- a) Application performance metrics
- b) User authentication attempts
- c) File system operations (create, modify, delete)
- d) Network traffic details

<details>
  <summary>Show Answer</summary>
  <b>c) File system operations (create, modify, delete)</b>
</details>

### Question 3:
Your company requires detailed tracking of all file modifications within an Azure Web App for compliance purposes. You need to enable and configure App Service File Audit Logs. Which of the following steps is essential to ensure these logs are available for analysis?

- a) Configure Application Insights to capture file system events.
- b) Enable Diagnostic Settings for the Web App and direct the logs to a Log Analytics workspace.
- c) Create a custom script to monitor file system changes and store them in Azure Blob Storage.
- d) Enable Azure Security Center's file integrity monitoring feature.

<details>
  <summary>Show Answer</summary>
  <b>b) Enable Diagnostic Settings for the Web App and direct the logs to a Log Analytics workspace.</b>
</details>

### Question 4:
Which Kusto Query Language (KQL) function is commonly used to filter App Service File Audit Logs based on specific file operations, such as "Delete"?

- a) `where`
- b) `project`
- c) `summarize`
- d) `join`

<details>
  <summary>Show Answer</summary>
  <b>a) `where`</b>
</details>

### Question 5:
A developer accidentally deleted a critical configuration file from an Azure Web App. Your team needs to identify who performed the deletion and the exact timestamp of the event. To retrieve this information, you should:

- a) Review the Web App's deployment history.
- b) Analyze the App Service File Audit Logs in Log Analytics using KQL queries.
- c) Check the Azure Activity Log for resource deletion events.
- d) Restore the Web App from a recent backup.

<details>
  <summary>Show Answer</summary>
  <b>b) Analyze the App Service File Audit Logs in Log Analytics using KQL queries.</b>
</details>

### Question 6:
Which App Service Plan tier is best suited for a production application that requires predictable performance and dedicated resources?

- a) Free (F1)
- b) Shared (D1)
- c) Basic (B1)
- d) Isolated (I1)

<details>
  <summary>Show Answer</summary>
  <b>c) Basic (B1)</b>
</details>

### Question 7:
In an App Service Plan using the Standard (S1) tier, how does Azure handle scaling out to accommodate increased traffic?

- a) It automatically increases the CPU quota on the existing VM.
- b) It adds new VM instances with the same applications and services.
- c) It distributes the load across different Azure regions.
- d) It switches to a higher tier App Service Plan automatically.

<details>
  <summary>Show Answer</summary>
  <b>b) It adds new VM instances with the same applications and services.</b>
</details>

### Question 8:
A development team is deploying a new web application for internal testing. They need a cost-effective solution but understand that performance may vary. Which App Service Plan tier is most appropriate for this scenario?

- a) PremiumV3 (P1V3)
- b) IsolatedV2 (I1V2)
- c) Free (F1) or Shared (D1)
- d) Standard (S1)

<details>
  <summary>Show Answer</summary>
  <b>c) Free (F1) or Shared (D1)</b>
</details>

### Question 9:
What is a key characteristic of the Isolated (I1) App Service Plan tier that differentiates it from other tiers?

- a) It offers a lower cost than the Shared (D1) tier.
- b) It provides network isolation through dedicated Azure Virtual Networks.
- c) It limits the number of VM instances for scaling.
- d) It charges based on CPU quota usage.

<details>
  <summary>Show Answer</summary>
  <b>b) It provides network isolation through dedicated Azure Virtual Networks.</b>
</details>

### Question 10:
If you have an App Service Plan with no deployed applications, what is the billing implication?

- a) You are not charged.
- b) You are charged only for storage.
- c) You are charged for the reserved VM instances.
- d) You are charged a reduced rate.

<details>
  <summary>Show Answer</summary>
  <b>c) You are charged for the reserved VM instances.</b>
</details>

### Question 11:
A company has a critical application that experiences high resource utilization and requires independent scaling. Which action should be taken regarding the App Service Plan?

- a) Deploy the application to a Shared (D1) tier to minimize costs.
- b) Add more applications to the existing App Service Plan to optimize resource usage.
- c) Move the application to a new, dedicated App Service Plan.
- d) Enable auto-scaling within the existing App Service Plan.

<details>
  <summary>Show Answer</summary>
  <b>c) Move the application to a new, dedicated App Service Plan.</b>
</details>

### Question 12:
Which of the following Azure App Service features share the same VM instances within an App Service Plan?

- a) Deployment slots and Azure SQL Database.
- b) Diagnostic logs and Azure Cosmos DB.
- c) WebJobs and deployment slots.
- d) Azure Functions and Azure Blob Storage.

<details>
  <summary>Show Answer</summary>
  <b>c) WebJobs and deployment slots.</b>
</details>

### Question 13:
For applications requiring maximum scale-out capabilities and network isolation, which App Service Plan tier is the most suitable?

- a) Basic (B1)
- b) Standard (S1)
- c) PremiumV3 (P1V3)
- d) Isolated (I1)

<details>
  <summary>Show Answer</summary>
  <b>d) Isolated (I1)</b>
</details>

### Question 14:
A web application within a Standard (S1) App Service Plan experiences a sudden surge in traffic. To ensure optimal performance, auto-scaling is enabled. What happens when the traffic exceeds the current VM instance capacity?

- a) The existing VM instance automatically upgrades to a higher tier.
- b) Azure creates new VM instances within the same App Service Plan.
- c) The application becomes temporarily unavailable.
- d) Azure switches to a different App Service Plan.

<details>
  <summary>Show Answer</summary>
  <b>b) Azure creates new VM instances within the same App Service Plan.</b>
</details>

### Question 15:
What is the primary difference in charging between the Shared (D1) tier and the Dedicated (Standard S1) tier?

- a) Shared tiers are charged per VM instance, while Dedicated tiers are charged per CPU quota.
- b) Shared tiers are charged per CPU quota, while Dedicated tiers are charged per VM instance.
- c) Shared tiers are free, while Dedicated tiers are based on usage.
- d) There is no difference in charging between the two tiers.

<details>
  <summary>Show Answer</summary>
  <b>b) Shared tiers are charged per CPU quota, while Dedicated tiers are charged per VM instance.</b>
</details>

### Question 16:
When cloning an App Service Plan, which of the following conditions must be met?

- a) The source and destination plans must be in different resource groups.
- b) The source and destination plans must be in the same geographical region.
- c) The source and destination plans must have different operating system types.
- d) The source and destination plans must support different features.

<details>
  <summary>Show Answer</summary>
  <b>b) The source and destination plans must be in the same geographical region.</b>
</details>

### Question 17:
You need to create a new App Service Plan and deploy a copy of an existing web app to it. The source web app is named "MyAppService" and is in the "SourceAzureResourceGroup". The destination plan should be in "DestinationAzureResourceGroup". Which Azure CLI command correctly performs this operation?

- a) `az appservice plan create --name DestinationAppServicePlan --resource-group DestinationAzureResourceGroup && az webapp create --name MyAppService2 --resource-group DestinationAzureResourceGroup`
- b) `New-AzAppServicePlan -Location $destinationLocation -ResourceGroupName DestinationAzureResourceGroup -Name DestinationAppService
-Tier Standard && New-AzWebApp -SourceWebApp $srcapp -AppServicePlan DestinationAppServicePlan -Location $destinationLocation -ResourceGroupName DestinationAzureResourceGroup -Name MyAppService2`
- c) `az appservice copy --source-plan SourceAzureResourceGroup --destination-plan DestinationAzureResourceGroup && az webapp deploy --name MyAppService2`
- d) `az appservice plan clone --source-plan SourceAzureResourceGroup --destination-plan DestinationAzureResourceGroup && az webapp create --name MyAppService2 --plan DestinationAppServicePlan`

<details>
  <summary>Show Answer</summary>
  <b>b) `New-AzAppServicePlan -Location $destinationLocation -ResourceGroupName DestinationAzureResourceGroup -Name DestinationAppServicePlan -Tier Standard && New-AzWebApp -SourceWebApp $srcapp -AppServicePlan DestinationAppServicePlan -Location $destinationLocation -ResourceGroupName DestinationAzureResourceGroup -Name MyAppService2`</b>
</details>

### Question 18:
What is the primary difference between "Manual scaling" and "Autoscale" in Azure App Service?

- a) Manual scaling is based on schedules, while Autoscale is a one-time event.
- b) Manual scaling is a one-time event, while Autoscale is based on schedules or resource metrics.
- c) Manual scaling affects only one app, while Autoscale affects all apps in the plan.
- d) Manual scaling requires PremiumV2 or higher, while Autoscale works on Basic and higher.

<details>
  <summary>Show Answer</summary>
  <b>b) Manual scaling is a one-time event, while Autoscale is based on schedules or resource metrics.</b>
</details>

### Question 19:
Which App Service Plan tier offers "Automatic scaling" with pre-warmed instances to avoid cold start issues?

- a) Basic (B1)
- b) Standard (S1)
- c) PremiumV2 (P1V2)
- d) Shared (D1)

<details>
  <summary>Show Answer</summary>
  <b>c) PremiumV2 (P1V2)</b>
</details>

### Question 20:
A web application experiences fluctuating traffic patterns. You need to configure scaling based on CPU utilization. If CPU utilization exceeds 70%, you want to add an instance. If it falls below 30%, you want to remove an instance. What type of scaling should you use?

- a) Manual scaling
- b) Vertical scaling
- c) Autoscale
- d) Horizontal scaling

<details>
  <summary>Show Answer</summary>
  <b>c) Autoscale</b>
</details>

### Question 21:
What is "Flapping" in the context of Azure App Service scaling?

- a) Adding and removing VM instances manually.
- b) A loop condition where scale-out and scale-in events alternate rapidly.
- c) Scaling up or down by changing the App Service Plan tier.
- d) Scaling based on a predefined schedule.

<details>
  <summary>Show Answer</summary>
  <b>b) A loop condition where scale-out and scale-in events alternate rapidly.</b>
</details>

### Question 22:
Which Azure CLI command is used to enable automatic scaling for an App Service Plan?

- a) `az appservice plan scale --name $appServicePlanName --resource-group $resourceGroup --elastic-scale true`
- b) `az appservice plan update --name $appServicePlanName --resource-group $resourceGroup --elastic-scale true --max-elastic-worker-count <YOUR_MAX_BURST>`
- c) `az appservice plan autoscale --name $appServicePlanName --resource-group $resourceGroup --enable`
- d) `az webapp config appsettings set --name $appServicePlanName --resource-group $resourceGroup --settings ELASTIC_SCALE=true`

<details>
  <summary>Show Answer</summary>
  <b>b) `az appservice plan update --name $appServicePlanName --resource-group $resourceGroup --elastic-scale true --max-elastic-worker-count <YOUR_MAX_BURST>`</b>
</details>

### Question 23:
A developer wants to set up continuous deployment for their web app from a Git repository to Azure App Service. Which built-in deployment options are available?

- a) Azure SQL Database, Azure Cosmos DB
- b) Azure DevOps, GitHub, Bitbucket, Local Git
- c) Azure Blob Storage, Azure Files
- d) Azure Functions, Logic Apps

<details>
  <summary>Show Answer</summary>
  <b>b) Azure DevOps, GitHub, Bitbucket, Local Git</b>
</details>

### Question 24:
What is the difference between vertical and horizontal scaling in Azure App Service?

- a) Vertical scaling adds or removes VM instances, while horizontal scaling changes the App Service Plan tier.
- b) Vertical scaling changes the App Service Plan tier, while horizontal scaling adds or removes VM instances.
- c) Vertical scaling is automatic, while horizontal scaling is manual.
- d) Vertical scaling is based on schedules, while horizontal scaling is based on resource utilization.

<details>
  <summary>Show Answer</summary>
  <b>b) Vertical scaling changes the App Service Plan tier, while horizontal scaling adds or removes VM instances.</b>
</details>

### Question 25:
For a scale-in event to occur in an App Service Plan with configured autoscale rules, which condition must be met?

- a) At least one scale-in rule must be triggered.
- b) All scale-in rules must be triggered.
- c) Any scale-out rule must not be triggered.
- d) A manual scale-in action must be performed.

<details>
  <summary>Show Answer</summary>
  <b>b) All scale-in rules must be triggered.</b>
</details>

### Question 26:
A company wants to automate their deployment process from Azure Container Registry (ACR) to an Azure Web App. Which Azure App Service feature supports this integration?

- a) Azure Backup
- b) Built-in CI/CD with container registries
- c) Azure Monitor Logs
- d) Azure Traffic Manager

<details>
  <summary>Show Answer</summary>
  <b>b) Built-in CI/CD with container registries</b>
</details>

### Question 27:
What is the primary purpose of setting a `max-elastic-worker-count` when enabling automatic scaling for an App Service Plan?

- a) To define the minimum number of VM instances.
- b) To limit the maximum number of VM instances that can be added.
- c) To set the CPU utilization threshold for scaling.
- d) To specify the schedule for automatic scaling.

<details>
  <summary>Show Answer</summary>
  <b>b) To limit the maximum number of VM instances that can be added.</b>
</details>

### Question 28:
A development team is implementing a blue/green deployment strategy for a critical web application. They need to deploy a new version to a staging slot, warm it up, and then swap it with the production slot to minimize downtime. Which App Service Plan tier is required to use deployment slots?

- a) Free (F1)
- b) Shared (D1)
- c) Basic (B1)
- d) Standard (S1)

<details>
  <summary>Show Answer</summary>
  <b>d) Standard (S1)</b>
</details>

### Question 29:
Which of the following application settings is typically *not* swapped between deployment slots during a swap operation?

- a) Connection strings
- b) Custom domain names
- c) Managed identities
- d) Public certificates

<details>
  <summary>Show Answer</summary>
  <b>c) Managed identities</b>
</details>

### Question 30:
A web application uses a local server for data retrieval. Due to security policies, direct firewall modifications are prohibited. Which Azure App Service feature allows the application to securely communicate with the local server without changing firewall settings?

- a) Azure Traffic Manager
- b) Hybrid Connections
- c) Azure Content Delivery Network (CDN)
- d) Azure Virtual Network integration

<details>
  <summary>Show Answer</summary>
  <b>b) Hybrid Connections</b>
</details>

### Question 31:
What is the purpose of the `.deployment` file in Azure App Service custom deployments?

- a) To define the application's scaling rules.
- b) To specify the build and deployment scripts to be executed.
- c) To configure the application's connection strings.
- d) To set the application's authentication settings.

<details>
  <summary>Show Answer</summary>
  <b>b) To specify the build and deployment scripts to be executed.</b>
</details>

### Question 32:
A development team wants to manually route a small percentage of production traffic to a staging slot for testing purposes. Which HTTP header parameter should they use to achieve this?

- a) `x-ms-routing-percentage`
- b) `x-ms-traffic-routing`
- c) `x-ms-routing-name`
- d) `x-ms-slot-routing`


<details>
  <summary>Show Answer</summary>
  <b>c) `x-ms-routing-name`</b>
</details>

### Question 33:
When are App Settings and Connection Strings applied to an Azure App Service application, and what happens when they are changed?

- a) They are set during runtime and can be dynamically updated without a restart.
- b) They are set during deployment and require a manual restart to apply changes.
- c) They are set at app startup and trigger a restart when changed.
- d) They are set only through the Azure portal and don't trigger a restart.

<details>
  <summary>Show Answer</summary>
  <b>c) They are set at app startup and trigger a restart when changed.</b>
</details>

### Question 34:
A web application uses Application Insights Profiler for performance monitoring. The application frequently unloads due to inactivity, causing gaps in the profiling data. Which App Service configuration setting should be enabled to prevent this?

- a) ARR affinity
- b) CORS
- c) Always On
- d) IP restrictions

<details>
  <summary>Show Answer</summary>
  <b>c) Always On</b>
</details>

### Question 35:
In a multi-instance App Service deployment, what is the purpose of ARR affinity?

- a) To ensure that all requests are load-balanced across all instances.
- b) To route requests to the nearest geographic instance.
- c) To ensure that a client's session is maintained on the same instance.
- d) To enable automatic scaling based on client traffic.

<details>
  <summary>Show Answer</summary>
  <b>c) To ensure that a client's session is maintained on the same instance.</b>
</details>

### Question 36:
A developer needs to ensure that specific application settings are preserved across deployment slot swaps. They understand that by default, certain settings are swapped. What app setting needs to be added, and what should it's value be, to ensure these settings are not swapped?

- a) `WEBSITE_PRESERVE_SLOT_SETTINGS` set to `true`
- b) `WEBSITE_OVERRIDE_PRESERVE_DEFAULT_STICKY_SLOT_SETTINGS` set to `0` or `false`
- c) `WEBSITE_DISABLE_SLOT_SWAPPING` set to `1` or `true`
- d) `WEBSITE_ENABLE_SLOT_STICKINESS` set to `1` or `true`

<details>
  <summary>Show Answer</summary>
  <b>b) `WEBSITE_OVERRIDE_PRESERVE_DEFAULT_STICKY_SLOT_SETTINGS` set to `0` or `false`</b>
</details>

### Question 37:
How are App Service application settings passed to a containerized application running in App Service?

- a) As command-line arguments.
- b) Using environment variables set with the `--env` flag.
- c) Through a mounted configuration file.
- d) As HTTP headers in the application's requests.

<details>
  <summary>Show Answer</summary>
  <b>b) Using environment variables set with the `--env` flag.</b>
</details>

### Question 38:
A developer needs to configure an App Service application setting named `ApplicationInsights:InstrumentationKey` in a Linux-based App Service. How should this nested setting name be formatted in the Azure CLI command?

- a) `ApplicationInsights.InstrumentationKey`
- b) `ApplicationInsights__InstrumentationKey`
- c) `ApplicationInsights:Instrumentation_Key`
- d) `ApplicationInsights.Instrumentation-Key`

<details>
  <summary>Show Answer</summary>
  <b>b) `ApplicationInsights__InstrumentationKey`</b>
</details>

### Question 39:
You are using Azure CLI to load app settings from a JSON file (`settings.json`). Which command correctly applies these settings to an App Service named `myWebApp` in the `myResourceGroup`?

- a) `az webapp config appsettings apply --resource-group myWebApp --name myResourceGroup --settings @settings.json`
- b) `az webapp config appsettings load --resource-group myResourceGroup --name myWebApp --settings @settings.json`
- c) `az webapp config appsettings set --resource-group myResourceGroup --name myWebApp --settings @settings.json`
- d) `az appservice appsettings set --resource-group myResourceGroup --name myWebApp --settings @settings.json`

<details>
  <summary>Show Answer</summary>
  <b>c) `az webapp config appsettings set --resource-group myResourceGroup --name myWebApp --settings @settings.json`</b>
</details>

### Question 40:
An application requires access to a secret stored in Azure Key Vault. Which format should be used in the App Service application setting to reference the secret, assuming the key vault is named `myvault` and the secret is named `mysecret`?

- a) `@Microsoft.KeyVault(SecretUri=https://myvault.vault.azure.net/secrets/mysecret/)`
- b) `@Azure.KeyVault(Vault=myvault;Secret=mysecret)`
- c) `@KeyVault(Name=myvault;Secret=mysecret)`
- d) `@KeyVault(Uri=https://myvault.vault.azure.net/secrets/mysecret/)`

<details>
  <summary>Show Answer</summary>
  <b>a) `@Microsoft.KeyVault(SecretUri=https://myvault.vault.azure.net/secrets/mysecret/)`</b>
</details>

### Question 41:
How are connection strings prefixed in Azure App Service configuration, similar to how they're set in `Web.config`?

- a) With the application name.
- b) With the resource group name.
- c) With the connection type.
- d) With the environment variable name.

<details>
  <summary>Show Answer</summary>
  <b>c) With the connection type.</b>
</details>

### Question 42:
A developer needs to configure a SQL Server connection string named `MyDb` for an App Service. Which Azure CLI command correctly sets this connection string?

- a) `az webapp config connection-string add --connection-string-type SQLServer --settings MyDb="Server=myserver;Database=mydb;User Id=myuser;Password=mypassword;"`
- b) `az webapp config connection-string set --connection-string-type SQL --settings MyDb="Server=myserver;Database=mydb;User Id=myuser;Password=mypassword;"`
- c) `az webapp config connection-string set --connection-string-type SQLServer --settings MyDb="Server=myserver;Database=mydb;User Id=myuser;Password=mypassword;"`
- d) `az webapp config conn-string set --type SQLServer --settings MyDb="Server=myserver;Database=mydb;User Id=myuser;Password=mypassword;"`

<details>
  <summary>Show Answer</summary>
  <b>c) `az webapp config connection-string set --connection-string-type SQLServer --settings MyDb="Server=myserver;Database=mydb;User Id=myuser;Password=mypassword;"`</b>
</details>

### Question 43:
Which Azure CLI command is used to enable HTTP/2.0 for an App Service named `myWebApp` in the `myResourceGroup`?

- a) `az webapp config set --name myWebApp --resource-group myResourceGroup --enable-http20`
- b) `az webapp config http20 --name myWebApp --resource-group myResourceGroup --enable`
- c) `az webapp config set --name myWebApp --resource-group myResourceGroup --http20-enabled`
- d) `az appservice config http20 --name myWebApp --resource-group myResourceGroup --enable`

<details>
  <summary>Show Answer</summary>
  <b>c) `az webapp config set --name myWebApp --resource-group myResourceGroup --http20-enabled`</b>
</details>

### Question 44:
A developer wants to map all incoming requests to the `/public` directory within their App Service's `wwwroot` folder. Which JSON configuration should be used in the `az resource update` command?

- a) `[{"virtualPath": "/public", "physicalPath": "site\\wwwroot"}]`
- b) `[{"virtualPath": "/", "physicalPath": "site\\wwwroot\\public"}]`
- c) `[{"virtualPath": "/public", "physicalPath": "wwwroot"}]`
- d) `[{"virtualPath": "/", "physicalPath": "public"}]`

<details>
  <summary>Show Answer</summary>
  <b>b) `[{"virtualPath": "/", "physicalPath": "site\\wwwroot\\public"}]`</b>
</details>

### Question 45:
Which App Service feature is not supported for function apps or containerized App Service apps?

- a) Always On
- b) Handler Mappings
- c) Local Cache
- d) App Settings

<details>
  <summary>Show Answer</summary>
  <b>c) Local Cache</b>
</details>

### Question 46:
A developer needs to add a custom script processor to handle all `.php` files in an App Service. What configuration is required in the Handler Mappings?

- a) Extension: `*.php`, Script processor: `D:\\home\\site\\wwwroot\\php-processor.exe`
- b) Extension: `.php`, Script processor: `/home/site/wwwroot/php-processor.sh`
- c) Extension: `*.php`, Script processor: `php-processor.exe`
- d) Extension: `.php`, Script processor: `D:\\php-processor.exe`

<details>
  <summary>Show Answer</summary>
  <b>a) Extension: `*.php`, Script processor: `D:\\home\\site\\wwwroot\\php-processor.exe`</b>
</details>

### Question 47:
How can you verify the custom environment variables set in an Azure App Service?

- a) Through the Azure portal's "Configuration" blade.
- b) By using the Azure CLI's `az webapp config env list` command.
- c) By navigating to `https://<app-name>.scm.azurewebsites.net/Env`.
- d) By checking the application logs in Application Insights.

<details>
  <summary>Show Answer</summary>
  <b>c) By navigating to `https://<app-name>.scm.azurewebsites.net/Env`.</b>
</details>

### Question 48:
In a Linux container App Service, when persistent storage is enabled, which directory allows file persistence and sharing across all instances?

- a) /tmp
- b) /home
- c) /var
- d) /root

<details>
  <summary>Show Answer</summary>
  <b>b) /home</b>
</details>

### Question 49:
Which Azure Storage service can be mounted as a read-only local share in a Linux App Service?

- a) Azure Queue Storage
- b) Azure Table Storage
- c) Azure Files
- d) Azure Blobs

<details>
  <summary>Show Answer</summary>
  <b>d) Azure Blobs</b>
</details>

### Question 50:
A development team needs to mount an Azure Files share to their App Service. Which Azure CLI command correctly performs this operation, assuming `share-name`, `account-name`, `access-key`, and `mount-path` are correctly defined?

- a) `az webapp storage mount add --custom-id <custom-id> --storage-type AzureFiles --share-name <share-name> --account-name <storage-account-name> --access-key "<access-key>" --mount-path <mount-path-directory>`
- b) `az webapp config storage add --custom-id <custom-id> --storage-type AzureFiles --share-name <share-name> --account-name <storage-account-name> --access-key "<access-key>" --mount-path <mount-path-directory>`
- c) `az webapp config storage-account mount --custom-id <custom-id> --storage-type AzureFiles --share-name <share-name> --account-name <storage-account-name> --access-key "<access-key>" --mount-path <mount-path-directory>`
- d) `az webapp config storage-account add --custom-id <custom-id> --storage-type AzureFiles --share-name <share-name> --account-name <storage-account-name> --access-key "<access-key>" --mount-path <mount-path-directory>`

<details>
  <summary>Show Answer</summary>
  <b>d) `az webapp config storage-account add --custom-id <custom-id> --storage-type AzureFiles --share-name <share-name> --account-name <storage-account-name> --access-key "<access-key>" --mount-path <mount-path-directory>`</b>
</details>

### Question 51:
Which of the following directories should *not* be used as a mount path to avoid issues in an Azure App Service?

- a) /opt
- b) /home
- c) /data
- d) /var

<details>
  <summary>Show Answer</summary>
  <b>b) /home</b>
</details>

### Question 52:
A developer wants to deploy a Docker Compose file to Azure App Service. Which Azure CLI command should they use?

- a) `az webapp deploy --multicontainer-config-file $dockerComposeFile`
- b) `az webapp create --multicontainer-config-file $dockerComposeFile`
- c) `az webapp config container set --multicontainer-config-file $dockerComposeFile`
- d) `az webapp container deploy --multicontainer-config-file $dockerComposeFile`

<details>
  <summary>Show Answer</summary>
  <b>b) `az webapp create --multicontainer-config-file $dockerComposeFile`</b>
</details>

### Question 53:
To enable the use of a managed identity for pulling container images from Azure Container Registry (ACR) in an App Service, what generic configuration setting should be applied?

- a) `{acrUseManagedIdentity:true}`
- b) `{acrUseManagedIdentityCreds:true}`
- c) `{acrManagedIdentity:true}`
- d) `{acrManagedIdentityCreds:true}`

<details>
  <summary>Show Answer</summary>
  <b>b) `{acrUseManagedIdentityCreds:true}`</b>
</details>

### Question 54:
Which Azure CLI command is used to create an ARM template for a specific deployment within a resource group?

- a) `az group export --name $resourceGroup`
- b) `az group deployment export --name $resourceGroup --deployment-name $deployment`
- c) `az deployment group create --resource-group $resourceGroup --template-file $armTemplateJsonFile`
- d) `az resource export --name $resourceGroup`

<details>
  <summary>Show Answer</summary>
  <b>b) `az group deployment export --name $resourceGroup --deployment-name $deployment`</b>
</details>

### Question 55:
A development team wants to deploy a local ZIP file to an Azure Web App. Which Azure CLI command should they use?

- a) `az webapp deploy zip --src-path "path/to/zip"`
- b) `az webapp deploy upload --src-path "path/to/zip"`
- c) `az webapp deploy --src-path "path/to/zip"`
- d) `az appservice deploy --src-path "path/to/zip"`

<details>
  <summary>Show Answer</summary>
  <b>c) `az webapp deploy --src-path "path/to/zip"`</b>
</details>

### Question 55:
What happens to the /home/LogFiles directory in a Linux container App Service regardless of the persistent storage status, if logging is enabled?

- a) It's deleted on every restart.
- b) It's only accessible in read-only mode.
- c) It always persists.
- d) It requires separate configuration to persist.

<details>
  <summary>Show Answer</summary>
  <b>c) It always persists.</b>
</details>

### Question 56:
Which of the following scenarios is *not* recommended when mounting Azure Storage as a local share in an App Service?

- a) Placing the app and storage in the same Azure region.
- b) Using it for local databases or apps needing file locks.
- c) Avoiding regenerating the access key.
- d) Removing the mount configuration before deleting Azure Storage.

<details>
  <summary>Show Answer</summary>
  <b>b) Using it for local databases or apps needing file locks.</b>
</details>

### Question 57:
A web application deployed on Azure App Service needs to access Azure Key Vault to retrieve secrets. The application uses a system-assigned managed identity. Which environment variables are automatically defined by the App Service to facilitate this access?

- a) `KEYVAULT_ENDPOINT` and `KEYVAULT_HEADER`
- b) `IDENTITY_ENDPOINT` and `IDENTITY_HEADER`
- c) `MSI_ENDPOINT` and `MSI_HEADER`
- d) `TOKEN_ENDPOINT` and `TOKEN_HEADER`

<details>
  <summary>Show Answer</summary>
  <b>b) `IDENTITY_ENDPOINT` and `IDENTITY_HEADER`</b>
</details>

### Question 58:
A development team is implementing OAuth authentication for a single-page application hosted on Azure App Service. The application uses the server-directed authentication flow. What is the initial endpoint the client is redirected to for user sign-in?

- a) `/.auth/callback/aad`
- b) `/.auth/login/aad`
- c) `/.auth/token/aad`
- d) `/.auth/user/aad`

<details>
  <summary>Show Answer</summary>
  <b>b) `/.auth/login/aad`</b>
</details>

### Question 59:
An application running on Azure App Service needs to access user claims sent in the `x-ms-client-principal` header. Which programming construct is used to deserialize and parse this header into a `ClaimsPrincipal` object?

- a) `JsonSerializer.Deserialize<ClientPrincipal>`
- b) `XmlSerializer.Deserialize<ClientPrincipal>`
- c) `BinaryFormatter.Deserialize<ClientPrincipal>`
- d) `DataContractJsonSerializer.Deserialize<ClientPrincipal>`

<details>
  <summary>Show Answer</summary>
  <b>a) `JsonSerializer.Deserialize<ClientPrincipal>`</b>
</details>

### Question 60:
A company wants to secure their Azure App Service with a certificate that is automatically renewed and managed by Azure. They need to export this certificate for use in other applications. Which type of certificate should they use?

- a) Free Managed Certificate
- b) Self-signed certificate
- c) App Service Certificate
- d) Certificate from Azure Key Vault (non-integrated)

<details>
  <summary>Show Answer</summary>
  <b>c) App Service Certificate</b>
</details>

### Question 61:
A developer needs to make a private certificate available to their App Service application. They have uploaded a password-protected PFX file. What Azure CLI command should they use to load this certificate into the application's environment?

- a) `az webapp config ssl set --certificate-thumbprint <thumbprint>`
- b) `az webapp config appsettings set --settings WEBSITE_LOAD_CERTIFICATES=<comma-separated-certificate-thumbprints>`
- c) `az webapp config certificate load --thumbprint <thumbprint>`
- d) `az webapp ssl upload --certificate-thumbprint <thumbprint>`

<details>
  <summary>Show Answer</summary>
  <b>b) `az webapp config appsettings set --settings WEBSITE_LOAD_CERTIFICATES=<comma-separated-certificate-thumbprints>`</b>
</details>

### Question 62:
An application requires TLS mutual authentication. Which App Service Plan tier is required to enable client certificate authentication?

- a) Free (F1)
- b) Shared (D1)
- c) Basic (B1)
- d) Standard (S1)

<details>
  <summary>Show Answer</summary>
  <b>c) Basic (B1)</b>
</details>

### Question 63:
A Node.js application deployed on Azure App Service needs to access the client certificate sent by the browser. Which request header should the application inspect to retrieve this certificate?

- a) `X-CLIENT-CERT`
- b) `X-ARR-CLIENT-CERT`
- c) `CLIENT-CERTIFICATE`
- d) `TLS-CLIENT-CERT`

<details>
  <summary>Show Answer</summary>
  <b>b) `X-ARR-CLIENT-CERT`</b>
</details>

### Question 64:
A web application hosted on Azure App Service needs to allow cross-origin requests from a specific domain. Which Azure CLI command should be used to configure CORS settings for the application?

- a) `az webapp cors allow --allowed-origins $website`
- b) `az webapp cors add --allowed-origins $website`
- c) `az webapp cors set --allowed-origins $website`
- d) `az webapp cors enable --allowed-origins $website`

<details>
  <summary>Show Answer</summary>
  <b>b) `az webapp cors add --allowed-origins $website`</b>
</details>

### Question 65:
A web application needs to send credentials like cookies or authentication tokens in cross-origin requests. Which configuration setting is required to enable this behavior in the browser?

- a) `ACCESS-CONTROL-ALLOW-CREDENTIALS: true` header in the response
- b) `CORS-ALLOW-CREDENTIALS: true` in the request headers
- c) `CORS-CREDENTIALS: true` in the web app configuration
- d) `ALLOW-CREDENTIALS: true` in the application settings.

<details>
  <summary>Show Answer</summary>
  <b>a) `ACCESS-CONTROL-ALLOW-CREDENTIALS: true` header in the response</b>
</details>

### Question 66:
A web application deployed on Azure App Service uses a user-assigned managed identity to access Azure resources. Which of the following parameters is mandatory when requesting a token from the `IDENTITY_ENDPOINT`?

- a) `client_id`
- b) `principal_id`
- c) `resource` and `X-IDENTITY-HEADER`
- d) `mi_res_id`

<details>
  <summary>Show Answer</summary>
  <b>c) `resource` and `X-IDENTITY-HEADER`</b>
</details>

### Question 67:
A company wants to use certificates stored in Azure Key Vault for their App Service application. They need to automatically renew these certificates. Which type of certificate configuration supports automatic renewal?

- a) Non-integrated certificates created with `az keyvault certificate create`.
- b) Certificates uploaded directly to App Service.
- c) Self-signed certificates.
- d) Certificates without a default policy set in Key Vault.

<details>
  <summary>Show Answer</summary>
  <b>a) Non-integrated certificates created with `az keyvault certificate create`.</b>
</details>

### Question 68:
A developer wants to access another Azure App Service using the access token obtained from the current App Service's authentication flow. Which header should be added to the request?

- a) `X-MS-TOKEN-AAD-ACCESS-TOKEN`
- b) `Authorization: Bearer ${req.headers['x-ms-token-aad-access-token']}`
- c) `X-AAD-ACCESS-TOKEN`
- d) `Bearer ${req.headers['x-ms-token']}`

<details>
  <summary>Show Answer</summary>
  <b>b) `Authorization: Bearer ${req.headers['x-ms-token-aad-access-token']}`</b>
</details>

### Question 69:
An App Service deployed to a Linux container is configured with App Service Authentication. What is the behavior of the authentication middleware in relation to the application's environment?

- a) It shares the same IIS sandbox as the application.
- b) It runs as an integrated part of the containerized application.
- c) It runs separately from the application's container.
- d) It is not supported in Linux containers.

<details>
  <summary>Show Answer</summary>
  <b>c) It runs separately from the application's container.</b>
</details>

### Question 70:
When configuring TLS mutual authentication for an App Service, where is the TLS termination handled?

- a) On the application server.
- b) On the frontend load balancer.
- c) Within the App Service container.
- d) On the client browser.

<details>
  <summary>Show Answer</summary>
  <b>b) On the frontend load balancer.</b>