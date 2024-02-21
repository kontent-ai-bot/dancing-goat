# dancing-goat

The backup of the Dancing Goat Kontent.ai project can be used with old versions of the sample apps. To import this project, you should use our tool [data-ops](https://github.com/kontent-ai/data-ops) tool. An import of the project into the Kontent.ai app consists of the following steps:
1. Login to the [kontent.ai](https://app.kontent.ai) application
2. [Create a new project](https://kontent.ai/learn/docs/projects#a-create-projects) or find the [project environment](https://kontent.ai/learn/docs/environments#a-select-an-environment-in-the-ui) you would like to import the Dancing Goat project into. We recommend using an empty environment
3. If you don't already have a Management API key, you can generate one following [this guide](https://kontent.ai/learn/docs/apis/api-keys?sl=1#a-create-management-api-keys)
> Be aware that the content import depends on the permission you select for the MAPI Key!
4. Don't forget to [activate MAPI in your project](https://kontent.ai/learn/docs/apis/api-keys?sl=1#a-create-management-api-keys)
5. Import the Dancing Goat project by executing the following command
```bash
npx @kontent-ai/data-ops import --fileName dancing_goat_backup.zip --environmentId <target-environment-id> --apiKey <Management-API-key>
```
