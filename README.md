# deploy-scripts-buildpack

Buildpack that runs custom shell script in project root folder

It will check for the init file `.deploy/init` in the project root folder. You can this the buildpack in any execution order

# How to use:
## Heroku
### As the first in execuion order
1. `heroku buildpacks:clear` if necessary
2. `heroku buildpacks:set https://github.com/ecratum/deploy-scripts-buildpack` as the first buildpack
3. `heroku buildpacks:add heroku/...` can add more buildpacks if needed
4. Deploy your project to Heroku.

## Dokku
### As the first in execuion order
1. `dokku buildpacks:clear` if necessary
2. `dokku buildpacks:set https://github.com/ecratum/deploy-scripts-buildpack` as the first buildpack
3. `dokku buildpacks:add heroku/...` can add more buildpacks if needed
4. Deploy your project.
