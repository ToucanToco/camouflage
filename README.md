# Camouflage
Advanced techniques to integrate Toucan's in every brand environment

## Set up
### Using yarn
In `package.json`:

    {
      "dependencies": {
        "tc-camouflage": "git+ssh://git@github.com/ToucanToco/camouflage.git#vX.Y.Z"
      }
    }

Then require it's styles where needed:

    @import 'node_modules/tc-camouflage/main';

> Example: see [`tucana`](https://github.com/ToucanToco/tucana)

### Using bower
In `bower.json`:

    {
      "dependencies": {
        "tc-camouflage": "git@github.com:ToucanToco/camouflage#vX.Y.Z"
      }
    }

Or run:

    bower install --save git@github.com:ToucanToco/camouflage

Then use `wiredep` or any tool that reads bower dependencies and include them
in your app.

## Develop using your local version
Use `yarn` or `bower` depending on which one you used for setup

:warning: **This will work only if you add a new class, attribute, ... . Otherwise it will be overwritten by laputa camouflage.**:warning:

In your local `camouflage` folder:

    yarn link

Then in your dependent project folder:

    yarn link tc-camouflage


## Git Workflow

We use `master` as the main branch, pull requests should point to it.
You can then release camouflage and update the version on `tucana` and `laputa`.

For developments that cannot be merged yet on the master branch but need to be used, use a feature branch:

```
"tc-camouflage": "git+ssh://git@github.com/ToucanToco/camouflage.git#f/my-new-feature"
```
