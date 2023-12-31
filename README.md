# Website

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:
(must configure deploy key in deployment repo and secrete private ssh key with pem format in source repo. Must include begin and end lines of private key)
```
$ USE_SSH=true yarn deploy

> cmd /C "set "USE_SSH=true" && yarn deploy"
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy

> cmd /C "set "GIT_USER=<GITHUB_USERNAME>" && yarn deploy"
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
