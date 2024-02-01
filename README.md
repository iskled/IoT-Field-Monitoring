# IoT Field Monitoring
(Monitoring farm field with the use of IoT )

Components Deployed:

Raspberry Pi 4:

Acted as the primary controller for collecting data from field sensors with the Linux-based Raspberry Pi OS.
Managed data processing, storage, and communication with the cloud and other devices.

Sensors:
Various sensors deployed in the field for data collection:
Soil moisture sensors,  Temperature and humidity sensors,
Light sensors, Rainfall sensors,
Wind speed and direction sensors

Breadboard and Jumper Wires:
Used for connecting the circuit with sensors and Raspberry Pi.
Workflow:

Sensor Data Collection:
Raspberry Pi read data from connected sensors using GPIO pins and other communication interfaces (I2C, SPI).
Python scripts were developed to interface with sensors and collect data at regular intervals.

Data Processing:
Python scripts on the Raspberry Pi processed raw sensor data and aggregated.

Storage:
Processed data was sent to external databases, including AWS DynamoDB and Firebase.

Communication:
Raspberry Pi transmited processed data to the cloud platform using protocols like MQTT and HTTP.
Enabled remote monitoring and centralized data storage.

Visualization:
MATLAB was utilized for data visualization and analysis.
Plots were generated directly from the sensor data to represent key metrics.

Alerts and Notifications:
Alerting mechanisms was implemented based on specific conditions (e.g., soil moisture thresholds).
Notifications was sent via email.

Remote Access:
Secure access to monitor data remotely was facilitated through tools like SSH and VPN.

Scalability:
Performance remained unaffected as the quantity of sensors increased, thanks to the decentralized storage approach.
