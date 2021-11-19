# nx12to13

https://github.com/nrwl/nx/issues/7807


commands
```
npx create-nx-workspace@12.0.0
nx migrate 13.2.0
npm install
nx migrate --run-migrations
```

Error
```
>  NX  Running migrations from 'migrations.json'

Running migration add-target-dependencies

>  NX   NOTE  Target dependencies have been updated in nx.json

  Nx has deprecated strictlyOrderedTargets in favour of targetDependencies.
  Based on your configuration the migration has configured targetDependencies for the following targets: build.
  Read more here: https://nx.dev/core-concepts/configuration

Successfully finished add-target-dependencies
---------------------------------------------------------
Running migration set-default-base-if-not-set
Successfully finished set-default-base-if-not-set
---------------------------------------------------------
Running migration 13-0-0-config-locations
Successfully finished 13-0-0-config-locations
---------------------------------------------------------
Running migration set-parallel-default
Successfully finished set-parallel-default
---------------------------------------------------------
Running migration update-webpack-browser-config
Successfully finished update-webpack-browser-config
---------------------------------------------------------
Running migration update-storybook
Successfully finished update-storybook
---------------------------------------------------------
Running migration update-angular-eslint-rules
Successfully finished update-angular-eslint-rules
---------------------------------------------------------
Running migration convert-webpack-browser-build-target-to-delegate-build
Successfully finished convert-webpack-browser-build-target-to-delegate-build
---------------------------------------------------------
Running migration update-invalid-import-paths
Successfully finished update-invalid-import-paths
---------------------------------------------------------
Running migration add-postcss-packages
Successfully finished add-postcss-packages
---------------------------------------------------------
Running migration update-angular-config
Successfully finished update-angular-config
---------------------------------------------------------
Running migration update-libraries
Successfully finished update-libraries
---------------------------------------------------------
Running migration update-angular-jest-config
Successfully finished update-angular-jest-config
---------------------------------------------------------
Running migration update-testing-imports
Successfully finished update-testing-imports
---------------------------------------------------------
Running migration schematic-options-13
Cannot find module '@angular-devkit/core'
Require stack:
- ~\AppData\Local\Temp\tmp-24140-14Bhrtd0OOQg\node_modules\@nrwl\tao\src\commands\ngcli-adapter.js
- ~\AppData\Local\Temp\tmp-24140-14Bhrtd0OOQg\node_modules\@nrwl\tao\src\commands\migrate.js
- ~\AppData\Local\Temp\tmp-24140-14Bhrtd0OOQg\node_modules\@nrwl\tao\index.js
~\nx12to13\node_modules\yargs\build\lib\yargs.js:1132
                throw err;
                ^

Error: Command failed: ~\AppData\Local\Temp\tmp-24140-14Bhrtd0OOQg\node_modules\.bin\tao migrate --run-migrations
    at checkExecSyncError (child_process.js:790:11)
    at execSync (child_process.js:863:15)
    at Object.handler (~\nx12to13\node_modules\@nrwl\workspace\src\command-line\nx-commands.js:125:42)
    at Object.runCommand (~\nx12to13\node_modules\yargs\build\lib\command.js:196:48)
    at Object.parseArgs [as _parseArgs] (~\nx12to13\node_modules\yargs\build\lib\yargs.js:1043:55)
    at Object.get [as argv] (~\nx12to13\node_modules\yargs\build\lib\yargs.js:986:25)
    at initLocal (~\nx12to13\node_modules\@nrwl\cli\lib\init-local.js:28:79)
    at Object.<anonymous> (~\nx12to13\node_modules\@nrwl\cli\bin\nx.js:43:32)
    at Module._compile (internal/modules/cjs/loader.js:1085:14)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:1114:10) {
  status: 1,
  signal: null,
  output: [ null, null, null ],
  pid: 10076,
  stdout: null,
  stderr: null
}

```
