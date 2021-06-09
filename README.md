# Hello Managed Runtime!

"Hello World" example of an app that will run on Managed Runtime..

To deploy, you'll need a Runtime Admin API key: 

From there, create a file `~/.mobify`:

```json
{
    "username": "john@example.com",
    "api_key": "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"
}
```

Confirm you can access test project: 

https://runtime.commercecloud.com/salesforce-internal/hello-mobify

After that you can get things running locally:

```bash
# Use Node 12.x to run:
nvm use 12
npm ci

# Show available commands:
npm run

# Run locally, available on localhost:3000
npm start

# Create a "bundle", the code release  artifact used by Managed Runtime
npm run bundle

# Upload the bundle to Runtime Admin
npm run upload

# Build, upload and deploy the current code to Managed Runtime
npm run deploy
```

You should be able to see your changes here:

https://hello-mobify-production.mobify-storefront.com/