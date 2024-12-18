# dancing-goat

This backup of the Dancing Goat Kontent.ai project is compatible with older versions of the sample applications. To import the project, utilize our [data-ops](https://github.com/kontent-ai/data-ops) tool. The import process involves the following steps:
1. Login to the [kontent.ai](https://app.kontent.ai) application.
2. [Create a new project](https://kontent.ai/learn/docs/projects#a-create-projects) or find the [project environment](https://kontent.ai/learn/docs/environments#a-select-an-environment-in-the-ui) you would like to import the Dancing Goat project into. We encourage using an empty environment.
3. If you don't already have a Management API key, you can [generate one].
> Be aware that the import depends on the permission you select for the MAPI Key!
4. Don't forget to [activate MAPI in your project](https://kontent.ai/learn/docs/apis/api-keys?sl=1#a-create-management-api-keys)
5. Restore the Dancing Goat project by executing the following command
```bash
npx @kontent-ai/data-ops@latest environment restore --fileName dancing_goat_backup.zip --environmentId <target-environment-id> --apiKey <Management-API-key>
```
Alternatively, you can restore the project using the same version of the Data Ops tool that was used to create the backup:

```bash
npx @kontent-ai/data-ops@2.2.2 environment restore --fileName dancing_goat_backup.zip --environmentId <target-environment-id> --apiKey <Management-API-key>
```
