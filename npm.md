# npm

### Installation

    Node comes with npm

### Upgrade

    npm install npm -g
  
## Packages

Install locally (in present working directory) to `./node_modules`

    npm install <package-name>
    
Install globally 

    npm install -g <package-name>


Check versions of package available in npm

    npm view <package> versions

Install and register to `package.json`

    npm install -g <package-name> --save-dev
    
Update and register to `package.json`

    npm install <package-name>@<version> --save
    
Remove package 

    npm uninstall <package-name> [--save-dev|--save|--save-optional]

Explanation of flags

- --save: Package will be added/removed from your dependencies.

- --save-dev: Package will be added/removed from your devDependencies.

- --save-optional: Package will be added/removed from your optionalDependencies.


When to use local vs global (from https://docs.npmjs.com/files/folders):

- Local install (default): puts stuff in ./node_modules of the current package root.
- Global install (with -g): puts stuff in /usr/local or wherever node is installed.
- Install it locally if you're going to require() it.
- Install it globally if you're going to run it on the command line.
- If you need both, then install it in both places, or use npm link.
