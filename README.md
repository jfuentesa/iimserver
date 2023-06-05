# iimserver

iimserver is a network monitoring solution designed to provide comprehensive monitoring capabilities for nodes in an organization's network. It allows you to effectively monitor and manage various network resources and services.

## Features

- **Network Accessibility**: The server is accessible through the organization's network using a valid IP address specific to the network it operates in.

- **Node Monitoring Configuration**: The server is configured to monitor network nodes, including the installation and setup of required plugins for monitoring different services and resources on the nodes.

- **Alert Detection and Notification**: The server is capable of detecting and properly notifying alerts and issues detected on network nodes. It ensures timely notification of any problems or anomalies.

- **Monitoring Log**: A comprehensive monitoring log is maintained by the server, recording all relevant information related to node monitoring, including alerts, issues, and node statuses.

- **Database Integration**: The server is properly configured and connected to a functioning database, ensuring seamless integration with the web platform.

- **Node Management**: The server provides functionalities to manage and maintain the list of network nodes, allowing easy addition, editing, and removal of nodes.

- **Plugin Support**: Supported plugins are stored and configured correctly, enabling effective monitoring of various services and resources on network nodes.

## Requirements

- Python 3.x
- Database (e.g., MariaDB, MySQL)

## Getting Started

1. Clone the iimserver repository.
2. Install the required dependencies using `pip`.
3. Configure the server's network settings and ensure accessibility.
4. Set up the database and establish the necessary connections.
5. Start the server.

For detailed installation and configuration instructions, please refer to the [Documentation](docs/README.md).

## Dependencies

### 1. Database

- Create the database and import the file `src/iimserver.sql` to set up the necessary tables.

### 2. Python Dependencies

To install the Python dependencies, execute the following commands:
```
pip install mysql-connector-python
pip install ping3
```
Make sure you have Python and pip installed before running these commands. These dependencies are required for the proper functionality of iimserver and enable database connectivity and network monitoring features.

## Contributing

Feel free to contribute.

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

Feel free to explore the capabilities of iimserver and leverage its monitoring features to maintain a robust and reliable network infrastructure.
