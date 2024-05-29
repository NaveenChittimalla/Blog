---
title: Web Api Versioning - Controllers
category: aspnetcore
hidden: true
---
# 

### Prerequisites
- Visual Studio 2022 or above.
- .Net SDK 8.0 or Above

### What we will do
- Create an empty ASP.NET Core application.
- Configure web api services and middleware in **Program.cs**.
- Create models.
	- /Models/V1/Product.cs
	- /Models/V2/Product.cs
- Create Controllers.
	- /Controllers/V1/ProductController.cs
	- /Controllers/V2/ProductController.cs
- Install the packages
	- Asp.Versioning.Http
	- Asp.Versioning.Mvc.ApiExplorer
- Configure api versioning settings in Program.cs.
- Apply and map api version to controllers and action methods.
- Test the api versioning functionality.

### Implementation
- Open visual studiio 2022 IDE.
- Create a new project using the template **ASP.NET Core Empty**.
- Remove the line app.MapGet("/", () => "Hello World!"); in **Program.cs**.
- Configure the Web Api controllers services and middleware in **Program.cs**.
	<div class="code">                                                
		<p>var builder = WebApplication.CreateBuilder(args);</p>
		<p class="highlight">builder.Services.AddControllers();</p>
		<p>var app = builder.Build();</p>
		<p class="highlight">app.MapControllers();</p>
		<p>app.Run();</p>
	<div>
- Create a models Product

<style>

.code{
	background-color: #f0f0f0;
	font-size: 14px;
	padding: 10px;
	margin: 10px;
	border-radius: 10px;
}

.highlight {
   font-weight: bold;
   font-size: 15px;
   background-color: #f0f0f0;
}

</style>
To be continued....
........
........
........
## Breaking Changes
To prioritize security, enhance features, and maintain code quality, new versions of our software might include breaking changes. While we strive to minimize these changes through careful architectural choices, they can still occur. In such cases, we make it a priority to announce them and provide possible solutions.

***
Important

We might make changes without prior notice if the change is considered non-breaking, or if it is a breaking change being made to address critical product bugs or legal, security, or privacy concerns.
***

### What is a breaking change?
A breaking change is a modification that requires you to update your application to prevent disruptions. In Data API builder, breaking changes can include alterations to REST API contracts, GraphQL schema generation, and other elements that affect compatibility and functionality.

Breaking change examples
The following examples are a nonexhaustive list of breaking changes to Data API builder:

- REST API contract modifications
- Alterations in GraphQL schema generation
- Changes affecting backwards compatibility
- Removal or renaming of APIs or parameters
- Changes in error codes
- Adjustments to permission definition functionality
- Removal of allowed parameters, request fields, or response fields
- Addition of mandatory parameters or request fields without default values
- Modifications to intended API endpoint functionality
- Definition of a nonbreaking change
- A non-breaking change refers to a change that can be integrated into your application without causing disruption. Nonbreaking changes are typically communicated after implementation. Your application should be designed to handle these changes without prior notice.

### Non-Breaking Change Examples
The following examples are a nonexhaustive list of nonbreaking changes to Data API builder:

- Introduction of new endpoints
- Addition of methods to existing endpoints
- Incorporation of new fields in responses and requests
- Adjustments to field order within responses
- Introduction of optional request headers
- Changes to data length and response size
- Alterations to error messages and codes
- Fixes to HTTP response codes
- Extra metadata in generated OpenAPI documents

### How do we communicate breaking changes?
We make it a priority to inform you promptly about breaking changes. You can find breaking change notifications in the release notes of Data API builder releases on GitHub, and in the dedicated breaking changes list article.
