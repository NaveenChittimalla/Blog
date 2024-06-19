---
title: Web Api Versioning - Controllers
category: aspnetcore
---

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
- Open visual studiio 2022 IDE and click on **Create a new project**. 

  ![Create a new project](/blog/assets/img/versioning/controllers/1-open-vs-create-project-VS2022.png)
- Choose project template **ASP.NET Core Empty**.

	![Choose project template](/blog/assets/img/versioning/controllers/2-choose-project-template.png)
- Configure project details such as name, location to store the project files, and solution name and click on **Next**.

  ![Configure project details](/blog/assets/img/versioning/controllers/3-configure-project.png)
- Configure the additional information such as framework version, https, etc., and click on **Create**. To make it simple, I have not selected any additional settings.

  ![Configure project additional info](/blog/assets/img/versioning/controllers/4-configure-project-additional-info.png)
  
- New project created with some default files as showm below.

    ![New project and files](/blog/assets/img/versioning/controllers/5-new-project.png)
	
- Project execution starts from Program.cs class

    ![Program.cs file](/blog/assets/img/versioning/controllers/6-program-cs-default.png)
	
- Configure web api controller services and middleware in Program.cs file as shown below.
	
	![Configure controllers services and middleware](/blog/assets/img/versioning/controllers/7-configure-web-api-controllers-program-cs.png)
	
- Create a models Product

<style>

.code{
	background-color: #f0f0f0;
	font-size: 14px;
	padding: 10px;
	margin: 10px;
	border-radius: 10px;
	color: #000;
}

.highlight {
   font-weight: bold;
   font-size: 15px;
   background-color: #f0f0f0;
}

</style>
To be continued....