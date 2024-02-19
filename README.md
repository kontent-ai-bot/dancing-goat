# dancing-goat

The backup of the Dancing Goat Kontent.ai project can be used with old versions of the sample apps. If you would like to import this project, you should use [data-ops](https://github.com/kontent-ai/data-ops) tool.We recommend using an empty environment. To import the project into Kontent.ai app follow these steps:
1. Follow the instructions on the [data-ops](https://github.com/kontent-ai/data-ops) repository to download the data-ops tool.
2. Login to the [kontent.ai](https://app.kontent.ai) application.
3. Find the environment you would like to import the Dancing Goat project into.
4. If you don't already have a Management API key, you can generate one following [this guide](https://kontent.ai/learn/docs/apis/api-keys?sl=1#a-create-management-api-keys)
5. Don't forget to [activate MAPI in your project](https://kontent.ai/learn/docs/apis/api-keys?sl=1#a-create-management-api-keys).
6. Prepare your Management API key and Environment ID.
7. Import the the Dancing Goat project by executing the following command
```bash
npx @kontent-ai/data-ops import --fileName dancing_goat_backup.zip --environmentId <target-environment-id> --apiKey <Management-API-key>
```


