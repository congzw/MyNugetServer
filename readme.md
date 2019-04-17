# my nuget server

my nuget server with:

- Nuget.Server 3.1.2
- .Net Framework 4.6

## why foo.nupkg copy to Packages, not working?

check log: Error: Package foo is a symbols package (it contains .pdb files and a /src folder). The server is configured to ignore symbols packages. 
change web.config ignoreSymbolsPackages value from true to false, will solve it.
