# Power BI to Xero Connector

This repository provides a custom connector for integrating Xero with Power BI, enabling seamless data extraction from Xero into Power BI for reporting and analytics purposes.

## Features

- Extract data from Xero directly into Power BI.
- Create custom reports and dashboards using Xero data.
- Automate data refresh from Xero to Power BI for up-to-date insights.
- Support for multiple Xero organizations.
- Easy setup and configuration using Power BI's custom connector feature.

## Prerequisites

Before you can use this connector, ensure you have the following:

- A valid [Xero API](https://developer.xero.com/documentation/getting-started) account and app credentials.
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed on your machine.
- .NET Framework 4.6 or later (for building the connector if you plan to modify it).
- IDE for developing or customizing the connector.

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/1202DREAMSCAPE/PowerBI-To-Xero-Connector.git
    ```

2. Navigate to the project directory:

    ```bash
    cd PowerBI-To-Xero-Connector
    ```

3. Follow the Power BI Custom Connector setup guide for loading the connector into Power BI Desktop:

    - Copy the `.mez` file located in the `dist` folder to your `Documents\Power BI Desktop\Custom Connectors` directory.
    - Restart Power BI Desktop.
    - In Power BI, go to `File > Options and Settings > Options > Security` and enable custom connectors.
    - After restarting, navigate to `Get Data`, and search for "Xero" to find the connector.

## Usage

1. Open Power BI Desktop.
2. Select `Get Data` and search for `Xero`.
3. Authenticate using your Xero account.
4. Once authenticated, choose the data tables you want to import into Power BI.
5. Build custom reports and dashboards using the imported Xero data.

## Configuration

You can modify the connector to suit specific needs:

1. Open the `.mez` file in a text editor or development environment like Visual Studio.
2. Update any API calls or endpoints to match the Xero data you need.
3. Compile the changes and re-load the updated connector into Power BI.

## Troubleshooting

- **Authentication Issues**: Ensure your Xero API credentials are correct and have the required permissions.
- **Data Refresh Issues**: Make sure your API rate limits haven't been exceeded. Xero imposes limitations on the number of API calls you can make per day.
- **Connector Not Appearing**: Verify that custom connectors are enabled in Power BI's settings as described in the installation instructions.

## Contributing

We welcome contributions! If you'd like to contribute, please fork this repository and submit a pull request.

1. Fork the repo.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
