**Model Binding** is a process of mapping data from HTTP request to controller action method parameters.

Generally, controllers get data from different sources such as route data, query strings, form fields, and request body as a key-value pairs in string-like data format. Writing our own code to retrieve each of these values and convert them from string to .NET types is tedious and error-prone. **Model Binding**  automates this process.

Simply, **Model Binding** is a layer that acts like a bridge between HTTP request and controllers, transform the data to .NET types and supplies to controller action methods as parameters.

### Process
- Retrieve data from various sources such as route data, query strings, form data, and request body of HTTP request.
- Convert string values to .NET types.
- Provide the data to controllers in method parameters and public properties.
- Intialize the complex type and assign the values to properties of it.

#### Example
HTTP request to updata contact resource

| Url  | https://api.contactapp.com/contacts/1?timestamp=2024-01-02  |
| :------------ |:---------------|
| Method     | PUT |
| Headers     | Accept: application/json User-Agent: Mozilla/5.0        |
| Body | { "firstName":"",  "lastName":"",  "email:"", "PhoneNumber":"", "active":true } |



