# e-commerce-store
The store provides a comprehensive dashboard for managing products,
product categories, and orders. It also allows users to register, browse
products, search for products, add products to their cart, and checkout.
The backend is built with ASP.NET Core and Frontend by HTML,CSS,JS
through a friend
Features:
- Full dashboard
- Responsive frontend
- Account and cart for sell
- The store is designed to be easy to use for both customers and
administrators.

## Setting Up the E-Commerce Store

It's important to note that this project requires the following versions and packages to be installed:

- .NET SDK version 7.0 or higher
- Microsoft.AspNetCore.Identity.EntityFrameworkCore version 7.0.5
- Microsoft.EntityFrameworkCore.Design version 7.0.5
- Microsoft.EntityFrameworkCore.SQLite version 7.0.5
- Microsoft.EntityFrameworkCore.SqlServer version 7.0.5
- Microsoft.EntityFrameworkCore.Tools version 7.0.5
- Microsoft.VisualStudio.Web.CodeGeneration.Design version 7.0.6

If you're using Visual Studio, you may need a `.sln` file, we work on vs code and use dotnet command so we do not need one ,so if you're using VS, create a new empty MVC project and move the project files to it.

**Note:** that in VS Code, you may see errors in all files on the first open. However, these problems will disappear completely after you click on "build". It appears that before starting the build process, it is difficult for VS Code to recognize some things. The important thing is that these problems will disappear and not return. Also, don't forget to add the C# extension if you're using VS Code.



In default project use SQL Lite and project have Included database with some products to test.

if you want to create new database : 

1. delete images on Image folder and Image/Description sub-folder , do not delete background image or folder.
2. Delete ApplicationDvContext.db ApplicationDbContext.db-shm ApplicationDbContext.db-wal
3. Open the project folder and use the `dotnet ef` command.
4. Run the following command to generate a migration: `dotnet ef migrations add {migrationName}`
6. Run the following command to update the database: `dotnet ef database update`
6. remove comment from //await SeedData.SeedUsersAndRolesAsync(app); on Program.cs
6. run project
6. recomment //await SeedData.SeedUsersAndRolesAsync(app); on Program.cs

the included sql light ApplicationDbContext.db , the  Admin user is : `Admin`

and Passsword is : `Coding@1234?`

and non admin user is : `app-user` and with same password

if you create new database , the admin user also will be : Admin and Password : Coding@1234?

you can change this from `/data/SeedData.cs`.

If you prefer to use SQL Server, simply change the source to connect to your database then also :

1. Open the project folder and use the `dotnet ef` command.
2. Run the following command to generate a migration: `dotnet ef migrations add {migrationName}`
3. Run the following command to update the database: `dotnet ef database update`
4. You can now run the project.


