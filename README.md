# Developer Quickstart

## GitHub Authentication
1. Create a [GitHub PAT](https://github.com/settings/tokens) with the following permissions:
    - **repo** - Full control of private repositories.
    - **write:packages** - Upload packages to GitHub Package Registry.
2. Create a `.env` file in the root of the repository with the following format.
    `GITHUB_TOKEN=YOUR_PAT`
3. `npm install` should work as expected. Beform install, NPM will will leverage the  `./npm:preinstall` script to read your `.env` and authenticate with GitHub.
