# .NET Core and VS Code

* Open VS Code from any folder by right-clicking and selecting "Open with Code"
* Create a new terminal:
    * Ctrl + Shift + P > "Create Terminal"
* Create directory:
    * `mkdir src`
    * `cd src`
* Create empty solution with .NET CLI:
    * `dotnet new sln --name MySolution # leaving name blank copies from the folder name`
* Create new MVC project and add to solution:
    * `dotnet new mvc --name MyProject --output MyProject # optionally add auth method etc.`
    * `dotnet sln add .\MyProject\MyProject.csproj # looks for first .sln in working dir`
* Create new XUnit project and add to solution:
    * `dotnet new xunit --name MyProject.Tests --output MyProject.Tests`
    * `dotnet sln add .\MyProject.Tests\MyProject.Tests.csproj # looks for first .sln in working dir`
    * `dotnet add [optional project ref] reference [path to new project]`
* Build and run the app:
    * `dotnet restore`
    * `dotnet build # optionally add --configuration Release/Debug`
    * `cd MyProject`
    * `dotnet run # add --no-build to use already built project`
* Navigate to the site
* Add .gitignore extension:
    * Ctrl + Shift + P > "Install Extensions"
    * Search for "gitignore" and install
    * Ctrl + Shift + P > "Add gitignore"
    * Search for VisualStudio and add
* Add to Git and GitHub
    * `git init`
    * `git add`
    * `git commit -m "Add empty MVC project"`
    * Create a new repo in GitHub
    * `git remote add origin https://github.com/robbell/myproject.git`
    * `git push -u origin master`
