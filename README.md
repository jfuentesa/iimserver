# iimserver

iimserver is a network monitoring solution designed to provide comprehensive monitoring capabilities for nodes in an organization's network. It allows you to effectively monitor and manage various network resources and services.

## Features

- **Network Accessibility**: The server is accessible through the organization's network using a valid IP address specific to the network it operates in.

- **Alert Detection and Notification**: The server is capable of detecting and properly notifying alerts and issues detected on network nodes. It ensures timely notification of any problems or anomalies.

- **Monitoring Log**: A comprehensive monitoring log is maintained by the server, recording all relevant information related to node monitoring, including alerts, issues, and node statuses.

- **API Nodes Management**: The server provides API functionalities to manage and maintain the list of network nodes, allowing easy addition, editing, and removal of nodes.

- **Plugin Support**: Supported plugins enables effective monitoring of various services and resources on network nodes.

- **Node Features**: The nodes includes two features: 'Public' and 'Disabled'. The 'Public' feature allows you to designate specific nodes as public, making them visible in a convenient public list. This is useful when you want to share certain node information with others. On the other hand, the 'Disabled' feature allows you to activate or deactivate nodes, preventing their monitoring. This can be beneficial when you want to temporarily exclude certain nodes from monitoring or when performing maintenance tasks.

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
