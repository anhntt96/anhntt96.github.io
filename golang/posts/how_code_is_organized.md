### How code is organized in Go?

#### Workspaces

- Three subdirectories:
  - src: Contains source code files
  - pkg: Contains packages (lib)
  - bin: Contains executables
- Common organization is good for sharing
- Programmer usually has one workspace for many projects.
- Workspace directory defined by $GOPATH environment variable.

#### Packages
- Group of related source code files.
- Each package can imported by other packages

#### Package Main
- There must be one package called `main`
- Building the main package generated an executable program
- Main package need a `main()` function
- `main()` is where the code execution start

#### Import
- `import` keyword is used to access other packages
- Go standard library includes many packages
- Search package directories specified by GOROOT and GOPATH.

#### Go Tool
- `go build`: compiles the program
  - Arguments can be a list of packages or `.go` files
  - Create executable for the main package, same name as the first `.go` file.
- `go doc`: print documentation for a package.
- `go fmt`: formats source code files.
- `go get`: download packages and install them.
- `go list`: list all installed packages.
- `go run`: compare `.go` files and run the executable.
- `go test`: run tests using files ending in `_test.go`
