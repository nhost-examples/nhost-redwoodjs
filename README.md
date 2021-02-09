# Todo

This is an example app built with Nhost and RedwoodJS, implementing a very simple todo application. Nhost is used as the entire backend by providing auth, a GraphQL API (Hasura) and PostgreSQL.

- The GraphQL API endpoint is configured in `./redwood.toml` with `apiProxyPath`.
- The auth endpoint is configured in `./web/src/index.js` with `baseURL` passed to the AuthProvider component. The PR for adding Nhost as an auth provider is not merged yet (https://github.com/redwoodjs/redwood/pull/1725) so in the meantime, you have to checkout that branch and point this example app to use that updated auth package. Instructions on how to do that can be found here: https://github.com/redwoodjs/redwood/blob/main/CONTRIBUTING.md   


### Setup

RedwoodJS uses yarn. To get the dependencies installed, just do this in the root directory:

```terminal
yarn install
```

### Start the app

```terminal
yarn redwood dev web
```

Your browser should open automatically to `http://localhost:8910` to see the web app.
