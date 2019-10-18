# Lightning Conference 2019 Workshop

Congrats! You found the second part of the workshop. This is a very basic Lightning app that will allow us to get paid for users to post and replace content in a King of the Hill style page.

In order to set this up properly, we'll need to make some adjustments from the work we just did:

## Setup the Project

In our `.env` file, we'll need to change the following fields, and add one as well:

* `API_PATH` - This will point our frontend app which will run on port 3000 to the backend server, this should be `API_PATH="http://localhost:3001/api"`
* `LND_MACAROON` - We now need to make more advanced calls on our node, so we need more permissions. Change this from your `base64 readonly.macaroon` to your `base64 invoice.macaroon` that you can find in the same directory.

## Run the Project

Install dependencies and run the app with
```sh
npm install && npm run dev
```
