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
