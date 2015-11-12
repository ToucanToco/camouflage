# Camouflage
Advanced techniques to integrate Toucan's in every brand environment

## Set up
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

> Example: see [`tucana`](https://github.com/ToucanToco/tucana)

## Develop using your local version
In your local `camouflage` folder:

    bower link

In your dependent project folder, in order your local's version:

    bower link tc-camouflage
