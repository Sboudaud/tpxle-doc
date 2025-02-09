
# Using Abeeway Device Manager to encode or decode payloads
The easiest way to encode or decode Abeeway tracker payloads is to use Abeeway Device Manager. You can do that even if you do not have trackers linked to ThingPark Location.
 
1. Create a free account on: [https://community.thingpark.org/](https://community.thingpark.org/)
2. Log in to Abeeway Device Manager at the following URL: [here](https://community.thingpark.io/thingpark/abeewayDeviceAnalyzer/index.php?dxprofile=community-api). If using another platform, see [ThingPark platforms URLs](/D-Reference/ThingParkLocationURLs/).
3. You can then encode or decode Abeeway payloads from the device configuration page.
<img src="./images/ADM_device_configuration_encode_decode_payloads.png" border="0" />
# Using Abeeway driver
In this scenario, your application will directly interface with the LoRaWAN® network server to communicate with Abeeway trackers.
Our Abeeway driver docker service will run directly within your application framework to help you decode/encode uplink/downlink messages from/to Abeeway trackers.
<img src="./images/AbeewayDriver.png" border="0" />
## Installing the Abeeway driver
The Abeeway driver gives you access to the driver service and the relative API documentation.
1. Install Docker on the customer’s server using the following URL:<br/>[https://hub.docker.com/search/?type=edition&offering=community](https://hub.docker.com/search/?type=edition&offering=community)<br/>

2. Download Docker image from the public Docker repository. You can do it by executing the following command:
<code>[docker pull actility/iot-flow-drivers]</code>
3. Run Docker image from the public Docker repository. You can do it by executing the following command:
<code>docker run -d -p 8095:8095 actility/iot-flow-drivers</code>
4. After the command has been executed successfully, the container will download autonatically the latest driver version before been accessible and the driver service will be available locally on port 8095
5. Access the API documentation using the following url:
[http://localhost:8095/v1/swagger-ui/](http://localhost:8095/v1/swagger-ui/)

## Using the Abeeway driver - Some examples
You will use the following examples that you can apply to your application:
* **Example 1** [Decoding an uplink message](/C-Procedure-Topics/DecodeUplinkMessage_T/)<br/>

* **Example 2** [Encoding a downlink message](/C-Procedure-Topics/EncodeDownlinkMessage_T/).
* **Example 3** [Decoding a downlink message](/C-Procedure-Topics/DecodeDownlinkMessage_T/).

### Reference guide
You can access the comprehensive documentation of Abeeway drivers.

|  | Resource | 
| - | -------- | 
| **Driver** | [Asset Tracker Driver User Guide](/D-Reference/DocLibrary_R/#reference-guides-and-tools) | 
