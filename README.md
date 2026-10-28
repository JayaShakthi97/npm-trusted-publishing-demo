# trusted-publishing-demo

A small demo package for npm trusted publishing. New versions are published from GitHub Actions through OIDC, without an npm token stored in the repository.

The workflow is in [`.github/workflows/publish.yml`](.github/workflows/publish.yml). It runs when a GitHub release is published.

```js
const hello = require("@jayashakthiwso2/trusted-publishing-demo");

console.log(hello()); // Published with npm trusted publishing
```
