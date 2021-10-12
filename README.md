# Build Moonbeam Docs Site Static Locally

This repo helps you build the Moonbeam Docs site (all Languages) locally as a static site.

It uses a bash script to build the entire static structure, and then the npm package `http-server` to serve the static site locally.

## Getting Started - Building the File Structure

To get started clone the repo (via SSH as it is private):

```
git clone git@github.com:albertov19/BuildDocsSite.git
cd BuildDocsSite
```

Then you can run the bash file `buildSite.sh` - You might need to change execution permissions by doing:

```
chmod u+x ./buildSite.sh
```

With the right execution permssions run:

```
./buildSite.sh
```

You can also provide the flag `-f` to force a new build.

## Serving the Static Site

Once the file structure has been built, you need to install the npm packages with `yarn` or `npm i`:

```
yarn
```

Or:

```
npm i
```

Then you can serve the static site in port `8000` with the following command:

```
npx http-server ./moonbeam-docs-static/ -p 8000
```

You can find more info on `http-server` [here](https://www.npmjs.com/package/http-server).