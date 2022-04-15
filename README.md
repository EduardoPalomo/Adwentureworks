# Adwentureworks
Azure sample

c:\AdventureWorks>dotnet new mvc

dotnet run

Sample https://docs.microsoft.com/en-us/ef/core/cli/dotnet

Scaffold Database First

dotnet ef dbcontext scaffold "Server=tcp:sqlserver.database.windows.net,1433;Initial Catalog=database;Persist Security Info=False;User ID=youruser;Password=yourpassword;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;" Microsoft.EntityFrameworkCore.SqlServer -o Models
