# Adwentureworks
Command Usage – dotnet new mvc:
1. “dotnet new mvc”
The command creates a new “ASP.NET Core MVC Web Application”, the application contains basic boilerplate files and directory. The name of the project is not specified in the command, so by default, the name of the project will be taken from the name of the folder the command has been executed in. The command also restores the dependencies required by the web project. As the default language is C#, a C# ASP.NET MVC project will be created.

The MVC application created is ready to use, on executing the command “dotnet run”, the application will be hosted on local IIS Express server and the same will be listening on the following ports:

c:\AdventureWorks>dotnet new mvc

dotnet run

Sample https://docs.microsoft.com/en-us/ef/core/cli/dotnet

Installing the tools
dotnet ef can be installed as either a global or local tool. Most developers prefer installing dotnet ef as a global tool using the following command:

dotnet tool install --global dotnet-ef

Before you can use the tools on a specific project, you'll need to add the Microsoft.EntityFrameworkCore.Design package to it.

.NET CLI


dotnet add package Microsoft.EntityFrameworkCore.Design

Verify installation
Run the following commands to verify that EF Core CLI tools are correctly installed:

.NET CLI


dotnet ef

The following example scaffolds all schemas and tables and puts the new files in the Models folder.

dotnet ef dbcontext scaffold "Server=tcp:sqlserver.database.windows.net,1433;Initial Catalog=database;Persist Security Info=False;User ID=youruser;Password=yourpassword;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;" Microsoft.EntityFrameworkCore.SqlServer -o Models
