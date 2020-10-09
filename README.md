OPC UA PubSub Example
=====================

This example for OPC UA PubSub was built on NodeOPCUA.

NodeOPCUA is a OPC UA stack fully written in TypeScript for NodeJS.

This example has two distinct modules:

1) an OPC UA server simulating a PLC with a temperature transmitter (opc_ua_server.js)
2) a web application containing a OPC UA client and a simplified synoptic panel (opc_ua_client.js)

#### Install

prerequisites: npm 6.4.1 or superior

    $ git clone https://github.com/pedromoritz/opcua-pubsub-example
    $ cd opcua-pubsub-example
    $ npm install

#### Run

prerequisites: NodeJS v10.19.0 or superior

    $ cd opcua-pubsub-example
    $ # start server in background
    $ node opcua_server.js > /dev/null &
    $
    $ # start web application
    $ node opcua_client.js
    
    Now point http://localhost:3700 on your web browser
