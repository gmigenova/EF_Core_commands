# EF_Core_commands
Collection of command for ef core

Installing the tools
.NET CLI

   ```
dotnet tool install --global dotnet-ef
   ```
Update the tool using the following command:
   ```
 dotnet tool update --global dotnet-ef
   ```

.NET CLI
   ```
dotnet add package Microsoft.EntityFrameworkCore.Design
   ```
Verify installation
   ```
dotnet ef
   ```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 DB-First
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## EF Command create model mysql : DB-First
   ```
   dotnet ef dbcontext scaffold "Data Source=xx.xx.xx.xx;Initial Catalog=DBNAMExx;User ID=xxxx;Password=xxxx" MySql.Data.EntityFrameworkCore -o Models --force
   ```
 
## EF Command create model sql server : DB-First
 ```
 dotnet ef dbcontext scaffold "Data Source=xx.xx.xx.xx;Initial Catalog=DBNAMExx;User ID=xxxx;Password=xxxx" Microsoft.EntityFrameworkCore.SqlServer -o Models --force
 ```
 
 ```  
dotnet ef dbcontext scaffold "Server=(localdb)\mssqllocaldb;Database=Blogging;Trusted_Connection=True;" Microsoft.EntityFrameworkCore.SqlServer -o Models
 ```
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 CODE-First
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
   ## EF Command create model sql server : CODE-First
   ```
Add-Migration <NameMigration>
   ```
   ```
Update-Database
   ```
   
   
   
   
   
Reference > https://docs.microsoft.com/en-us/ef/core/cli/dotnet
