npm

Node Pacakage Manager
- Preinstalled
- - Modules are Javascript libraries

Install Node
npm.com: Search for packages (i.e. express)

NPM Commands:
npm --help (also -h)
npm -v
npm init : Creates NPM Script (package.json)
npm init -y (creates blank package.json)
npm config set (or npm set) - changes package.json 
Package.json: lists dependencies (Name & Version)
npm get (returns)

npm install [package name] --save (or -s) => Download package and save as dependency
- Adds Object as dependency of package.json (Dependency key will have an obeject as value, which will list all dependencies with version as value)
- Adds package-lock.json with similar information (cannot be published, npm-shrinkwrap works somewhat similarly)
- Creates node_modules directory with dependency directory(ies) inside

.gitignore file in the directory will allow you to ignore any directory or file when pushing/committing changes.
since dependencies are saved in package.json, you can save the amount of files needed to push or download.
This method is great for dependencies which are needed for the user

Dev Dependencies:
This is for when you don't want the user, just the developer to install
npm install --save-dev [package] will save as dev dependency
npm install --production will ignore dev dependencies

Uninstalling:
npm uninstall [pkg] to remove (also rm or un)
npm uninstall --save-dev [pkg] to remove as dev dependency
npm rm --save [pkg] for reg dependencies
npm update [pkg] to update package.jsoon with 

Semantic Versioning
[major version (breaks API)].[minor version (new features, no API breakage)].[patch (Bug Fixes)]
carat "^" means latest minor version
tilde ~ means latest patch version
no preceding symbol means exact
asterick * means install latest no matter what

Global Modules:
Examples (nodemon, live-server)
npm install -g nodemon
saves in npm folder? 
allows you to run file from any directory
npm rm -g  

Showing all dependencies
npm list (shows ALL Dependencies)
npm list --depth 1 (shows dependencies only to a certian level)

How to run your app:
in package.json under "scripts" you can define alias's which will create shortcuts for CLI commands
(will have to run as "npm run [pkg]")
Certian keywords like start do not need this keyword
