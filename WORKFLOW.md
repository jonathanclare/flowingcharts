# Workflow

Use the following workflow when editing the flowingcharts repo.

## Get the latest changes from the master branch

Open GitHub Desktop

Select
```
flowingcharts 
```

Click
```
Sync
```

## Rebuild the repo

Open a command prompt in `C:\Work\GitHub\flowingcharts`.

Windows: open Windows Explorer > navigate to the `C:\Work\GitHub\flowingcharts` > shift + right click > Open command window here.

Install any new node project dependencies
```
npm install
```

Rebuild the repo
```
grunt
```

## Running Grunt Tasks

Open a command prompt in `C:\Work\GitHub\flowingcharts`.

Windows: open Windows Explorer > navigate to the `C:\Work\GitHub\flowingcharts` > shift + right click > Open command window here.

Run this to generate `gen_build`, `gen_doc`, `gen_release` and `gen_test_coverage` directories.
```
grunt
```

Run this to rebuild the repo during development.
```
grunt build
```

Run this to automatically rebuild the repo whenever a file is saved.
```
grunt watch
```

Carry out unit testing on the JavaScript module files and generate a test coverage file at `gen_test_coverage/coverage.html`.
```
grunt test
```

Publish a release version to `gen_release/<%= pkg.version %>/`. 
```
grunt publish
```

Generate API documentation in `gen_doc`. 
```
grunt doc
```

## Commit your changes

This should be done regularly as you make changes to the repo

Open GitHub Desktop

Select the repo
```
flowingcharts 
```

Click
```
Changes
```

Add a summary and description of the changes you've made

Click
```
Commit to master
```

Click
```
Sync
```

## Sync your changes back to the master branch

At the end of the day in GitHub Desktop

Select
```
flowingcharts 
```

Click
```
Sync
```
