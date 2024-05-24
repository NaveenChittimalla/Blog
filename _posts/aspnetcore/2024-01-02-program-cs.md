---
title: Program.cs
permalink: /aspnetcore/programcs/
---
<div style="width:100%; background-color:grey;">
<div style="width:50%;float:left;text-align:left;">
<a href="/"><-- ASP.NET Core Home</a>
</div>
<div style="width:50%;float:right;text-align:right;">
<a href="host/">What is a Host --></a>
</div>
</div>
<div style="height:20px;">&nbsp;</div>


Program.cs is the entry point, where the application starts. 

#### What we can do in Program.cs
- Create a new instance of web application host with preconfigured default services.
- Configure services required by the application.
- Define request handling pipeline, by registering a series of middleware components.
- Run the web application host and listen to the HTTP requests.

```
namespace AspNetCore
{
   class Program
   {
      static void Main(string[] args)
      {

        var builder = WebApplication.CreateBuilder(args);

        // Configure required services.

        var app = builder.Build();

        // Define request handling pipeline by registering middleware components.

        app.Run();

      }
   }
}
```
With [top-level statements](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/program-structure/top-level-statements) feature introduced in C# 9, **Main** method or **namespace** have become optional and top-lvel statement file becomes application entry point. 

##### Program.cs with Top-level statement 
```
var builder = WebApplication.CreateBuilder(args);

// Configure required services.

var app = builder.Build();

// Define request handling pipeline by registering middleware components.

app.Run();
```
Above code create and run a web server with predefined default services and start listenting for the incoming request.
We will discuss more details in future sections.

<div style="height:20px;">&nbsp;</div>
<div style="width:100%; background-color:grey;">
<div style="width:50%;float:left;text-align:left;">
<a href="/"><-- ASP.NET Core Home</a>
</div>
<div style="width:50%;float:right;text-align:right;">
<a href="host/">What is a Host --></a>
</div>
</div>