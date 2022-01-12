# deploy-scripts-buildpack

Buildpack that runs custom shell script

The proposed use case. Add as a first buildpack in the chain. It will check for the init file `.deploy/init` in the project root folder.

# How to use:
## Heroku
1. `heroku buildpacks:clear` if necessary
2. `heroku buildpacks:set https://github.com/ecratum/predeploy-scripts-buildpack` as the first buildpack
3. `heroku buildpacks:add heroku/...` more buildpacks you need
4. Deploy your project to Heroku.

## Dokku
1. `dokku buildpacks:clear` if necessary
2. `dokku buildpacks:set https://github.com/ecratum/predeploy-scripts-buildpack` as the first buildpack
3. `dokku buildpacks:add heroku/...` more buildpacks you need
4. Deploy your project.
