
## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Install Node.js if not already installed. [Node.js](https://nodejs.org/)
2. Install OpenAPI Generator CLI globally:

    ```bash
    npm install @openapitools/openapi-generator-cli -g
    ```

3. Generate the SDK:

    ```bash
    openapi-generator-cli generate -i your-api-spec.yaml -g your-sdk-generator -o output-directory --package-name package
    ```

    Replace placeholders:
    - `your-api-spec.yaml`: Path to your OpenAPI Specification file.
    - `your-sdk-generator`: Name of the generator (e.g., csharp, python, javascript, java).
    - `output-directory`: Output directory for the generated SDK.
    - `package`: Desired name for the package.

    Example:

    ```bash
    openapi-generator-cli generate -i your-api-spec.yaml -g python -o ./output/js-sdk --package-name PythonSDK
    ```

## Usage

Explore the generated SDK and integrate it into your application. Refer to the SDK documentation for detailed usage instructions.

## Customization

Customize the generated SDK as needed for your specific requirements. Refer to the generator's documentation for customization options.

## Contributing

If you would like to contribute to the development of this SDK, please follow our [Contribution Guidelines](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE).
