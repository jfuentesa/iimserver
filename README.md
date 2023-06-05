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

## Dependencies

### 1. Database

Create the database and import the file `src/iimserver.sql` to set up the necessary tables. Configure the database in the `config.ini`.

### 2. Python Dependencies

To install the Python dependencies, execute the following commands:
```
pip install mysql-connector-python
pip install ping3
```
Make sure you have Python and pip installed before running these commands. These dependencies are required for the proper functionality of iimserver and enable database connectivity and network monitoring features.

## API Documentation

Below is a brief description of the functionality of each endpoint in the iimserver monitoring server API:

- **GET /status**: Retrieves the current status of the monitoring server.

- **GET /config/dump**: Returns the complete configuration of the monitoring server, including all settings and configured options (a dump of `config.ini`).

- **GET /nodes/get**: Retrieves the list of all registered network nodes in the monitoring server, providing all details of each node.

- **GET /nodes/get/{n}**: Retrieves specific details of the node with the identifier `{n}`. It provides detailed information about a particular node, such as its status, IP address, ports, etc.

- **GET /nodes/getfailed**: Returns the list of nodes that have failed or encountered any issues during the last monitoring process.

- **GET /nodes/getpublic**: Retrieves the list of public nodes registered in the monitoring server. These nodes are available for querying in the public frontend of iimclient.

- **POST /nodes/add**: Allows adding a new node to the monitoring server.

- **POST /nodes/edit/{n}**: Enables editing the information of an existing node identified by `{n}`. Changes can be made to the node's parameters.

- **POST /nodes/delete/{n}**: Deletes a specific node identified by `{n}` from the monitoring server. This action involves completely removing the node and its associated records.

- **GET /log/get**: Retrieves the log of node status changes for all nodes.

- **GET /log/node/{n}**: Retrieves the specific status log of the node identified by `{n}`. It provides detailed information about the particular node.

- **GET /plugins/get**: Retrieves a list of all installed plugins on the server.

## Contributing

Feel free to contribute.

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

Feel free to explore the capabilities of iimserver and leverage its monitoring features to maintain a robust and reliable network infrastructure.
