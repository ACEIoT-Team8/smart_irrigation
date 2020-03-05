IOT BASED SMART IRRIGATION PROJECT USING NODEMCU, MOISTURE SENSOR, DHT11 AND THINGSPEAK IOT CLOUD PLATFORM


         TEAM MEMBERS

       UWIMANA Josephine: 215026137
       RUKUNDO Jean Claude:220014156
       KANYAMUNEZA Marie Noella:220012382
       MITSINDO Rene: 220014161
       UWIZEYE Marie Grace:220014347

Youtube link for this project :https://www.youtube.com/watch?v=-9ZSPoEYIng

                    INTRODUCTION
 
New technologies are helping in building automated systems resulting in a huge reduction of human work done. Watering is a crucial factor in farming and sometimes, problems occur if not well regulated due to overwatering or underwatering. This is the reason to be of our proposed system “Smart irrigation” to avoid all those incidents and ensure smart farming through smart irrigation.

                   OBJECTIVE OF THE PROJECT 

The main objective of this project was to Design and implement an IoT based smart irrigation system using NodeMCU.

Specific Objectives:

•The proposed project aims to ease the process of irrigation by supplying water when farm is dry without human presence and
• avoiding water wastage in irrigation process.

It also allows easy monitoring and visualization as the data from the sensors are sent to the client

              COMPONENTS REQUIRED:

Hardware:

NodeMCU ESP8266
 NodeMCU is an open source IoT platform. it includes firmware which runs on the ESP8266 Wi-Fi SoC from Expressive Systems, and hardware which is based on the ESP-12 module.

 ![nodemcu](https://user-images.githubusercontent.com/23235363/75878001-882fff00-5e21-11ea-8770-2d16563cb1b0.JPG)
 
              Soil Moisture Sensor Module
 
A simple soil moisture sensor for gardeners. Soil moisture sensors measure the volumetric water content in soil. Since the direct gravimetric measurement of free soil moisture requires removing, drying, and weighting of a sample, soil moisture sensors measure the volumetric water content indirectly by using some other property of the soil, such as electrical resistance, dielectric constant, or interaction with neutrons, as a proxy for the moisture content. The relation between the measured property and soil moisture must be calibrated and may vary depending on environmental factors such as soil type, temperature, or electric conductivity. Reflected microwave radiation is affected by the soil moisture and is used for remote sensing in hydrology and agriculture. Portable probe instruments can be used by farmers or gardeners.

![moisture](https://user-images.githubusercontent.com/23235363/75878166-db09b680-5e21-11ea-8c17-c2eb49008d83.JPG)

	         Water Pump Module
	
![waterpump](https://user-images.githubusercontent.com/23235363/75878364-24f29c80-5e22-11ea-890d-be47087f1055.JPG)

                Relay Module

A relay is an electrically operated switch. Many relays use an electromagnet to mechanically operate a switch, but other operating principles are also used, such as solid-state relays. Relays are used where it is necessary to control a circuit by a separate low-power signal, or where several circuits must be controlled by one signal. The first relays were used in long distance telegraph circuits as amplifiers: they repeated the signal coming in from one circuit and re-transmitted it on another circuit.

![relay](https://user-images.githubusercontent.com/23235363/75879018-430ccc80-5e23-11ea-941c-8837d661ca79.JPG)

              DH11

Humidity Sensor is one of the most important devices that has been widely in consumer, industrial, biomedical, and environmental etc. applications for measuring and monitoring Humidity values. For monitoring the temperature and humidity we use the DHT11 sensor. The DHT11 detects the water vapor by measuring the electrical resistance between two electrodes. The humidity sensing component is a moisture holding substrate with electrodes applied to the surface. When water vapor is absorbed by the substrate, ions are released by the substrate which increases the conductivity between the electrodes. The change in resistance between the two electrodes is proportional to the relative humidity. Higher relative humidity decreases the resistance between the electrodes, while lower relative humidity increases the resistance between the electrodes. The principle in the humidity sensor is They consist of a humidity sensing component, a NTC temperature sensor (or thermistor) and an IC on the back side of the sensor. For measuring humidity, they use the humidity sensing component which has two electrodes with Humidity moisture holding substrate between them. Humidity indicates the likelihood of predications, dew, or fog. Higher humidity reduces the effectiveness of sweating in cooling the body by reducing the rate of evaporation of moisture from the skin. This effect is calculated in a heat index table or humidex the amount of water vapor that is needed to achieve saturation increases as the temperature increases. As the temperature of a parcel of water becomes lower it will eventually reach the point of saturation without adding or losing water mass.

![dht11](https://user-images.githubusercontent.com/23235363/75879069-5f106e00-5e23-11ea-8401-2998fc054a47.JPG)

              BREADBOARD

A breadboard is a rectangular board with many mounting holes. They are used for creating electrical connections between electronic components and single board computers or microcontrollers such as Arduino and Raspberry Pi. The connections aren't permanent and they can be removed and placed again.

![breadboard](https://user-images.githubusercontent.com/23235363/75879117-78191f00-5e23-11ea-95b9-c6c0d1f5d4df.JPG)

           Jumpers 

A jump wire (also known as jumper wire, or jumper) is an electrical wire, or group of them in a cable, with a connector or pin at each end (or sometimes without them  simply "tinned"), which is normally used to interconnect the components of a breadboard or other prototype or test circuit, internally or with other equipment or components, without soldering.

![jumpwires](https://user-images.githubusercontent.com/23235363/75879158-8f580c80-5e23-11ea-8c55-019c8f6cb02e.JPG)

         SOFTWARE 
we have used the following software during our project implementation:

1.Adruino IDE
2.Blynk app
3.Thingspeak iOt Cloud platform


         METHODOLOGY 

          Sensor and Data Acquisition 

This stage consists of the moisture sensor to measure the amount of water in the soil and DHT11 sensor for continuously measures   temperature and humidity of the field. The sensors convert moisture, humidity and temperature content into electronic signals and send them to microcontroller. 

          Control 

The microcontroller used in this study is node MCU 8266. Its work is to process the data from sensors and control the status of the pump depending to the sensed data. node MCU 8266 receives measures value from two sensors in form of analog voltages and digitizes them. It then computes the appropriate control scheme meant to implement the irrigation based on the soil moisture, humidity and temperature of the field. The controller output is sent as a digital control to the irrigation pumps via the relay. The sensed data obtained are transmitted through wireless transmission and the user can monitor them through his or her mobile by using mobile application platform. In this project Blynk and thinkspeak iot cloudpage have been used as mobile application platform to read, store, and visualize sensor data and control hardware remotely. If soil moisture, temperature and humidity is less than the threshold value the pump is switched ON and if the soil moisture, temperature and humidity exceed the threshold value the pump is switched OFF.  

       IMPLEMENTATION

Working: 

IoT based smart irrigation system is capable of automating the irrigation process by analyzing the moisture of soil and the climate condition. Also, the data of sensors will be displayed on Thinkspeak and Blynk page. When the power supply is ON, the microcontroller checks the soil moisture content. If the moisture content is not up to the threshold then it makes the pump to get ON automatically and turns OFF automatically if reaches the threshold level. When the weather condition is such that it is raining then the microcontroller puts off the pump. After the raining it checks for threshold and takes the necessary action. If the power supply is off suddenly then after the power is on microcontroller turns on automatically there is no need of manually turn on and off the pump. All the data from the sensors and water is graphically shown in the thingspeak IoT cloud page which is used for monitoring. Advantages of these method is that it is a cost-effective irrigation controller, increase efficiency and decrease wastage, easy to monitor, reduces man cost, reduced runoff water and nutrients.

         flow chart 

![flowchart](https://user-images.githubusercontent.com/23235363/75879270-c4fcf580-5e23-11ea-942a-442c51f89d8b.JPG)

Circuit diagram using fritiz

 ![fullcircuit](https://user-images.githubusercontent.com/23235363/75879310-da721f80-5e23-11ea-8342-7914c5f33777.JPG)

        EXPERIMENTAL RESULTS

In this project we can control the motor in the field based on humidity, temperature and moisture level. The Moisture level of soil is measure or sensed by the sensors. These values are converted into digital form and applied to Arduino Nano. If the moisture levels of soil are dropped to a certain level the motor is turned on automatically without human interaction. The data from IoT is sent to the client using Cloud. Thus, any variations in the crop can be identified easily and early diagnosis is done as such.
The data is in graphical form so we can easily monitor
           
![th1](https://user-images.githubusercontent.com/23235363/75879381-01305600-5e24-11ea-9c1a-dd2c1017e9a8.JPG)
 Soil Moisture Graph on Thingspeak
![th2](https://user-images.githubusercontent.com/23235363/75879401-09889100-5e24-11ea-934c-0b51f20db173.JPG)
![th3](https://user-images.githubusercontent.com/23235363/75879407-0db4ae80-5e24-11ea-908d-cc0c7f488012.JPG)

          OUTPUT RESULT ON BLYNK APPLICATIONS 
	  
 ![blynk](https://user-images.githubusercontent.com/61824844/75997318-d6b7c900-5f07-11ea-9f7c-bd2dd2281a1b.jpeg)
          OUTPUT ON SERIAL MONITOR 
 
 ![result](https://user-images.githubusercontent.com/23235363/75879585-494f7880-5e24-11ea-9c4f-eb08aa60f16b.JPG)

 
         APPLICATIONS
	 
This system is applied in modern smart griculture of many crops types .

        REFERENCES

 1. IJACT: International Journal of Advancements in Computing Technology, 2.Vol. 4, No. 5, pp. 83-90, 2012. [16]
Xun-yi Ren, Lin-juan Chen, Hai-shan Wan, "Homomorphic Encryption and Its Security Application", JDCTA:
International Journal of Digital Content Technology and its Applications, Vol. 6, No. 7, pp. 305-311, 2012.

  2.Nicholas D., Darrell B., Somsak S., “Home Automation using Cloud Network and Mobile Devices”, IEEE Southeastcon 2012, Proceedings of IEEE.
 
  3.S.D.T. Kelly, N.K. Suryadevara, S.C. Mukhopadhyay, “Towards the Implementation of IoT for Environmental Condition Monitoring in Homes”, IEEE, Vol. 13, pp. 3846- 3853, 2013.
 



   FULL CIRCUIT 

![g81](https://user-images.githubusercontent.com/23235363/75876854-2373a500-5e1f-11ea-92ac-69da39176cda.jpeg)
GROUP 8
![g8](https://user-images.githubusercontent.com/23235363/75876461-6b45fc80-5e1e-11ea-93f4-56c7a71be07b.jpeg)
