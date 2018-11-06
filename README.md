# React + Redux + Shopify-Buy Boilerplate Code!

To get started, clone this repository:

`git clone https://github.com/frewinchristopher/react-redux-shopify-storefront-api-example.git`

This app was bootstrapped with create-react-app, so it should install just fine with:

`npm install`

The only thing to do before running is add your Shopify store credentials, both of which are in `index.js` in the `buildClient()` call:

```
const client = Client.buildClient({
    storefrontAccessToken: 'YOUR_SHOPIFY_STOREFRONT_ACCESS_TOKEN',
    domain: 'YOUR_MYSHOPIFY_STORE_URL'
});
```

Until you provide proper credentials, you'll see these errors in the console:
```
OPTIONS https://your_store_url/api/graphql net::ERR_NAME_NOT_RESOLVED
localhost/:1 Uncaught (in promise) TypeError: Failed to fetch
```

Run the development site with:

`npm run start`

Build a production version with:

`npm run build`

This is all described in detail [in a Medium post that goes step by step through this code base](https://github.com/frewinchristopher/react-redux-shopify-storefront-api-example). I highly suggest reading that so you know what the heck is going on!