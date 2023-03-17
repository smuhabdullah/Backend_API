# Zeek and Suricata APIs using Node.js
This project demonstrates how to create APIs to search for logs in Elasticsearch indices for the popular network security monitoring tools Zeek and Suricata using Node.js.

## Prerequisites
Before running the project, you should have the following software installed on your machine:

### Node.js
### Elasticsearch
### Installation
To install the project, clone this repository to your local machine:

```
git clone https://github.com/your-username/zeek-suricata-api.git
```
Navigate to the project directory:

```
cd Get_Zeek_Data
```
or 
```
cd Get_Suricata_Data
```

Install the required packages:

```
npm install
```
Usage
To start the API server, run the following command:

```
npm start
```
This will start the server on port 3000.

Suricata API
To search for Suricata logs, send a GET request to the following endpoint:

```
http://localhost:3000/suricata
```
You can include the following query parameters:

event_type: Search for logs of a specific event type.
For example, to search for all Suricata logs, send a GET request to:

```
http://localhost:3000/suricata
```
To search for all Suricata logs of the event type http, send a GET request to:

```
http://localhost:3000/suricata?event_type=http
```
Zeek API
To search for Zeek logs, send a GET request to the following endpoint:

```
http://localhost:3000/zeek
```
You can include the following query parameters:

id.orig_h: Search for logs from a specific source IP address.
id.resp_h: Search for logs to a specific destination IP address.
service: Search for logs of a specific service.
For example, to search for all Zeek logs, send a GET request to:
```
http://localhost:3000/zeek
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
