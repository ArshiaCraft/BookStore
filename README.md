# BookStore

Certainly! If you're looking for a concise and appealing description for your GitHub repository, here's a suggestion:

---

📚 **Book Store App with ABP Framework**

Explore the world of literature with our Book Store App! 🌐 This simple yet powerful application, crafted with the ABP (Asp.Net Boilerplate) framework, allows you to effortlessly manage your book collection.

✨ **Key Features:**
- **Effortless Book Management:** Add, edit, and delete books with ease.
- **Category Classification:** Keep your library organized with intuitive categorization.
- **Secure Authentication:** Ensure the safety of your data with a robust user authentication system.

⚙️ **Technologies:**
ABP Framework, ASP.NET Core, Entity Framework Core, Bootstrap, C#

### Pre-requirements

* [.NET 7.0+ SDK](https://dotnet.microsoft.com/download/dotnet)
* [Node v18 or 20](https://nodejs.org/en)

### Configurations

The solution comes with a default configuration that works out of the box. However, you may consider to change the following configuration before running your solution:

* Check the `ConnectionStrings` in `appsettings.json` files under the `Acme.BookStore.HttpApi.Host` and `Acme.BookStore.DbMigrator` projects and change it if you need.

### Before running the application

* Run `abp install-libs` command on your solution folder to install client-side package dependencies. This step is automatically done when you create a new solution with ABP CLI. However, you should run it yourself if you have first cloned this solution from your source control, or added a new client-side package dependency to your solution.
* Run `Acme.BookStore.DbMigrator` to create the initial database. This should be done in the first run. It is also needed if a new database migration is added to the solution later.

### Solution structure

This is a layered monolith application that consists of the following applications:

* `Acme.BookStore.DbMigrator`: A console application which applies the migrations and also seeds the initial data. It is useful on development as well as on production environment.
* `Acme.BookStore.HttpApi.Host`: ASP.NET Core API application that is used to expose the APIs to the clients.
* `Acme.BookStore.Blazor`: ASP.NET Core Blazor Server application that is the essential web application of the solution.

🤝 **Contribute:**
We welcome contributions! Submit issues, share your ideas, or open pull requests to make this Book Store App even better.

📜 **License:**
This is a layered startup solution based on [Domain Driven Design (DDD)](https://docs.abp.io/en/abp/latest/Domain-Driven-Design) practises. All the fundamental ABP modules are already installed. 
