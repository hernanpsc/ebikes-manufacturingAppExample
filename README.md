<<<<<<< HEAD
# Lightning Web Components Recipes Open Source

[![Github Workflow](https://github.com/trailheadapps/lwc-recipes-oss/workflows/CI/badge.svg)](https://github.com/trailheadapps/lwc-recipes-oss/actions?query=workflow%3ACI) [![codecov](https://codecov.io/gh/trailheadapps/lwc-recipes-oss/branch/main/graph/badge.svg)](https://codecov.io/gh/trailheadapps/lwc-recipes-oss)

A collection of easy-to-digest code examples for Lightning Web Components Open Source. Each recipe demonstrates how to code a specific task in 30 lines of code or less. A View Source link takes you right to the code in GitHub. From Hello World to data access and third-party libraries, there is a recipe for that!

<div>
   <img src="https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/projects/quick-start-explore-the-lightning-web-components-oss-recipes-sample-app/3039bf385440158b5a43a1d42cbbe82d_badge.png" align="left" alt="Trailhead Badge" height="40px" width="40px" style="padding-right: 0.5em;"/>
   <p style="padding-top:0.5em;">
      Learn more about this app by completing the <a href="https://trailhead.salesforce.com/en/content/learn/projects/quick-start-explore-the-lightning-web-components-oss-recipes-sample-app" >Quick Start: Explore the Lightning Web Components OSS Recipes Sample App</a> Trailhead project or by watching this <a href="https://www.youtube.com/watch?v=4mXCLJm8KF4&list=PLgIMQe2PKPSJcuCwM61dEc4jFG_jHqV2t&index=6">short presentation video</a>.
   </p>
</div>

## Recipes Live Version

Check out [https://lwc-recipes-oss.herokuapp.com](https://lwc-recipes-oss.herokuapp.com) live on Heroku. Or on [https://recipes.lwc.dev](https://recipes.lwc.dev).

## Deploy to Heroku

If you want to deploy LWC Recipes Open Source to Heroku, you can do the following:

1. Create a Heroku application:

```
heroku create <app name>
```

2. Deploy the application:

```
git push heroku main
```

## Local Development

1. Clone the `lwc-recipes-oss` repository:

```
git clone https://github.com/trailheadapps/lwc-recipes-oss
cd lwc-recipes-oss
```

2. Install the project dependencies using `npm` (or `yarn`, if you prefer that alternatively)

```
npm install
```

3. Build the LWR static site.

```
npm run build
```

4. Start the app in watch mode.

```
npm run dev
```

5. Enjoy the app!

## Code Tours

Code Tours are guided walkthroughs that will help you understand the app code better. To be able to run them, install the [CodeTour VSCode extension](https://marketplace.visualstudio.com/items?itemName=vsls-contrib.codetour).
=======
# E-Bikes Manufacturing Demo

This demo is built with the Lightning Web Runtime and demonstrates the use of the Pub/Sub API with Change Data Capture events and Platform Events.

🎥 Watch a short [introduction video](https://youtu.be/g9P87_loVVA).

> **Warning**<br/>
> This demo app does not use the most secure authentication mechanism. We recommend using an [OAuth 2.0 JWT Bearer Flow](https://help.salesforce.com/s/articleView?id=sf.remoteaccess_oauth_jwt_flow.htm&type=5) for production environments.

## Installation

You can either install the app on

-   [Heroku](#heroku-deploy) (quick deployment for demo purposes)
-   your [local machine](#local-setup) (prefered for development purposes)

### Heroku deploy

Click on this button and follow the instructions to deploy the app:

<p align="center">
  <a href="https://heroku.com/deploy?template=https://github.com/pozil/ebikes-manufacturing-lwc-oss">
    <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy">
  </a>
<p>

Once deployed, see the [configuration reference](#configuration-reference) section for configuring the environment variables.

### Local setup

1. Create a `.env` file at the root of the `ebikes-manufacturing` project

    ```properties
    SALESFORCE_AUTH_TYPE="user-supplied"
    SALESFORCE_LOGIN_URL="https://test.salesforce.com"
    SALESFORCE_API_VERSION="56.0"
    SALESFORCE_USERNAME="YOUR_SALESFORCE_USERNAME"
    SALESFORCE_PASSWORD="YOUR_SALESFORCE_PASSWORD"
    SALESFORCE_TOKEN="YOUR_SALESFORCE_SECURITY_TOKEN"

    PUB_SUB_ENDPOINT="api.pubsub.salesforce.com:7443"
    ```

1. Update the property values by referring to the [configuration reference](#configuration-reference) section

1. Install the project with `npm install`

1. Run the project with `npm start`

## Configuration reference

All variables are required.

| Variable                 | Description                                                                                                                                                                     | Example                          |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| `SALESFORCE_AUTH_TYPE`   | The Salesforce authentication type for the Pub/Sub API client. Do not change this value.                                                                                        | `user-supplied`                  |
| `SALESFORCE_LOGIN_URL`   | The login URL of your Salesforce org:<br>`https://test.salesforce.com/` for scratch orgs and sandboxes<br/>`https://login.salesforce.com/` for Developer Edition and production | `https://test.salesforce.com`    |
| `SALESFORCE_API_VERSION` | The Salesforce API version.                                                                                                                                                     | `56.0`                           |
| `SALESFORCE_USERNAME`    | Your Salesforce user's password.                                                                                                                                                | n/a                              |
| `SALESFORCE_PASSWORD`    | Your Salesforce username.                                                                                                                                                       | n/a                              |
| `SALESFORCE_TOKEN`       | Your Salesforce user's security token.                                                                                                                                          | n/a                              |
| `PUB_SUB_ENDPOINT`       | The endpoint used by the Pub/Sub API.                                                                                                                                           | `api.pubsub.salesforce.com:7443` |
>>>>>>> 6a9c1688be06c86f280c12542a18779997907763
