# Docs

Requirements:

* Node v14 LTS

## Setup
When setting up this repo, any of the doc watch calls will automatically clone the doc-ui submodule for you. Only using the full preview? 

Call to clone the doc-ui
```console
git submodule update --recursive --remote
```

## UI Development

UI Development has been moved to the [doc-ui submodule](https://github.com/skalenetwork/doc-ui)

## Develop with Hot Reload

Ready to update the docs? Pick your module below or work with all the local components simultaneously. 
> Note, if you are only working on a single component, your reload time will be much faster when picking a single module over all of them*

#### All Components
```console
yarn docs:watch
```
#### Develop
```console
yarn docs:watch:develop
```
####Filestorage
```console
yarn docs:watch:filestorage
```
#### Home
```console
yarn docs:watch:home
```
#### Learn
```console
yarn docs:watch:learn
```
#### Recipes
```console
yarn docs:watch:recipes
```
#### Technology
```console
yarn docs:watch:technology
```
#### Validators
```console
yarn docs:watch:validators
```

## Run Full Preview

To pull from live repos in the playbook and serve from the UI bundle, first install ui npm libraries to allow the bundle to be built. Then cd into the parent folder, install the libraries and prepare the bundle. Then run the playbook and serve the files.

```console
yarn
yarn prepare:ui     # build UI
yarn prepare:docs   # build docs
yarn serve
```
