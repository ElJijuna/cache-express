# Coffee Express Cache Middleware (Fork)

This is a fork of "cache-express", with minor and specific changes to avoid caching in services that return code other than 2xx and others.

Original Npm Page: <https://www.npmjs.com/package/cache-express>

## Install and Usage

You can install the Express Cache Middleware package using npm. Open your terminal or command prompt and run the following command:

```sh
npm install cache-coffee-express
```

To use the Express Cache Middleware, simply import it and apply it as middleware to your Express.js routes.

```javascript
import express from "express";
import expressCache from "cache-coffee-express";

const app = express();

// Apply the caching middleware to a route
app.get(
 "/api/data",
 expressCache({
  /*options*/
 })
);
