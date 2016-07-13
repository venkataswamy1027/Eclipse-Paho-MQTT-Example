<<<<<<< HEAD
=======
# Eclipse-Paho-MQTT-Example

>>>>>>> dfe8f18272e4e5f22f3c3c55b9263b98bb635104
# Eclipse Paho Java Client

The Paho Java Client is an MQTT client library written in Java for developing applications that run on the JVM or other Java compatible platforms.MQTT is a protocol and protocols need client implementations.
The Paho Java Client provides two APIs: MqttAsyncClient provides a fully asychronous API where completion of activities is notified via registered callbacks. MqttClient is a synchronous wrapper around MqttAsyncClient where functions appear synchronous to the application.

# MQTT

MQTT( Message Queue Telemetry Transport)  is a machine-to-machine (M2M)/Internet of Things connectivity protocol.It was designed as an extremely lightweight publish/subscribe messaging transport.Using Eclipse Paho to implement MQTT protocal to publishing/subsrcibe messages to clients with Mosquitto broker.

# Mosquitto

Mosquitto is an open-source message broker service that uses the MQTT protocol to send and receive messages,typically with IOT (Internet of Things) devices.It contain main responsibility of providing a communication between publisher and subscriber.In order to receive published messages and send them on to any clients who have subscribed, we need a broker. Mosquitto is one of such brokers which is easy to configure and run for MQTT messages.

Mosquitto's default configuration means it is set up to not use username/password authentication and it accepts all connections on port 1883.It also comes with two clients, mosquitto_pub and mosquitto_sub. mosquitto_pub client is used for publishing simple messages, while the later is for subscribing to a topic and printing the message that it received.

# installation steps for Mosquitto in Linux

step 1: sudo apt-add-repository ppa:mosquitto-dev/mosquitto-ppa
stpe 2: sudo apt-get update
step 3: sudo apt-get install mosquitto

# For Testing the Broker

step 4: sudo apt-get install mosquitto-clients

open two terminals.

Terminal A: receive the publishing message from terminal B
Command : mosquitto _sub -d -t "hello/world"

Terminal B:
Command : mosquitto_pub -d -t hello/world -m "Hi! how are you"
<<<<<<< HEAD
=======
------------------------
# Bridgelabz Tasks
(1). Sample code of the Java client to access a MQTT broker and publishing/subscribing the messages.
>>>>>>> dfe8f18272e4e5f22f3c3c55b9263b98bb635104
