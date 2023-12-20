# How to Generate of Client SDK using Open API Generator 

Creating an SDK using the OpenAPI Generator involves several steps. OpenAPI Generator is a tool that allows you to generate client libraries, server stubs, and API documentation from an OpenAPI Specification. Below is a step-by-step guide for creating an SDK using OpenAPI Generator: 

**Step 1: Install Node.js** 

Open API Generator requires Node.js installed in your machine for generating SDK. Ensure that you have Node.js installed on your system. You can download Node.js from the official website: [https://nodejs.org/ ](https://nodejs.org/) 

**Step 2: Generate OpenAPI Specification** 

Create or obtain an OpenAPI Specification (formerly known as Swagger Specification) for your API. This specification is a JSON or YAML file that outlines your API's endpoints, data models, and other pertinent details. You can create one manually or leverage tools such as Swagger Editor or Swagger UI to design your API and export the specifications. Additionally, you can automatically generate the OpenAPI Specification from existing code or API endpoints. 

**Step 3: Install OpenAPI Generator** 

Open a terminal or command prompt and run the following command to install the OpenAPI Generator globally: 

```bash
npm install @openapitools/openapi-generator-cli -g 
```

**Step 4: Generate SDK** 

Navigate to the directory where you have your OpenAPI Specification file. Run the following command to generate the SDK: 

```bash
openapi-generator-cli generate -i your-api-spec.yaml -g your-sdk-generator -o output-directory --package-name package 
```

Replace your-api-spec.yaml with the path to your OpenAPI Specification file, your-sdk- generator with the name of the generator you want to use (e.g., csharp, python, javascript,java), output-directory with the desired output directory for the generated SDK and package with your desired name for the package. If you don't add package name it will give open API-client. 

For example, to generate a Python SDK named PythonSDK, you might use: 

```bash
openapi-generator-cli generate -i your-api-spec.yaml -g python -o ./output/js-sdk --package-name PythonSDK 
```

**Step 5: Explore the Generated SDK** 

Once the generation process is complete, navigate to the specified output directory (./output/js- sdk in the example) to find the generated SDK files. The structure of the SDK will depend on the generator used. 

**Step 6: Customize the SDK (Optional)** 

Customize the generated SDK as needed for your specific requirements. Refer to the documentation of the specific generator for customization options. 

**Step 7: Use the SDK in Your Application** 

Integrate the generated SDK into your application. The SDK will provide classes and methods corresponding to the API endpoints defined in your OpenAPI Specification. Refer to the SDK documentation for details on how to use it in your programming language. 

**Step 8: Update SDK as Needed** 

If your API evolves or changes, update the OpenAPI Specification and regenerate the SDK using the same process to keep it in sync with your API. 

Please consult the documentation of the[ OpenAPI Generator ](https://openapi-generator.tech/docs/generators/)and the specific generator you're using for detailed options and instructions.  

**Step 8: Publish the package in their respective package manager** 

1. Python - Python Package Index(PyPI)/GitHub
2. Dotnet - Nuget Package Manager
3.  Node.Js - NPM/GitHub
4.  Java - Maven/GitHub
5.  Go - Go packages/GitHub


## Author

- [Devi Prakash](https://github.com/dprakash2101)
  




   
