## Pre-requisites

1. [Install Node JS](https://nodejs.org/en/download/)
1. [Install Yarn](https://yarnpkg.com/en/docs/install)
1. Download or clone this repository

## Setup
1. Make sure that your Instant Game app is setup. For more information see [our Setup Guide](https://developers.facebook.com/docs/messenger-platform/getting-started/app-setup)
1. In the root folder of this repo, run
	```bash
	$ yarn install
	```
1. Copy or rename the file `config.template.json` to `config.json` and replace the information needed from your app.
	```json
	{
		"FB_appId":"<YOUR_APP_ID_HERE>",
		"FB_uploadAccessToken": "<YOUR_UPLOAD_TOKEN_HERE>",
		...
	}
	```
Your app ID can be found at the landing page of your app's dashboard.

Your upload access token can be found on the Instant Games -> Web Hosting tab of your app's dashboard.

* **`hello-world`**: An empty project with the boilerplate in place to get you up and running quickly

### Running Client-Side examples:

In order to run these you will need to use one of these tasks:
* **`run-mock`**: Runs on localhost against a mocked version of the SDK
* **`mock`**: It is the same as **`run-mock`**. Runs on localhost against a mocked version of the SDK
* **`run-dist`**: Runs on localhost against the production SDK
* **`dist`**: It is the same as **`run-dist`**. Runs on localhost against the production SDK

Below are some examples of how to execute these tasks:

```bash
$ yarn run-mock --project hello-world
```
Will run the **`hello-world`** project from localhost against a mocked version of the SDK (returns dummy data for every call). This way of running projects is especially useful for quickly iterating on local changes done to any of the projects.
