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

In your local `camouflage` folder:

    yarn link

or

    bower link

Then in your dependent project folder:

    yarn link tc-camouflage

or

    bower link tc-camouflage
