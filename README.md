[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/kzkUPShx)
# a14g-final-submission

    * Team Number: 16
    * Team Name: EcoSavers
    * Team Members: Erica Feng, Xinyu Chen
    * Github Repository URL: https://github.com/ese5160/a14g-final-submission-t16-ecosavers
    * Description of test hardware: (development boards, sensors, actuators, laptop + OS, etc)   Embedded hardware, laptops, MCU and Wi-Fi, QR code reader to I2C, Distance sensor, Temperature and Humidity sensor and LED


## 1. Video Presentation
- Link of the video:
   - https://drive.google.com/file/d/11lY0ysqGzHl-wxLwl-oEmPQDffJTwq_s/view?usp=share_link
  
## 2. Project Summary
- Device Description
   - The project we designed is called "Smart Bin", which aims to address the issue of inefficient waste management by utilizing humidity and temperature sensor to classify garbage and sort it into appropriate bins. The primary problem it solves is the challenge of separating wet and dry waste effectively, which is crucial for efficient recycling and disposal processes. Meanwhile, in our smart bin system, the automatic sorting process is facilitated by a motor-driven platform that dynamically adjusts to sort garbage based on the detection from the humidity and temperature sensor. When garbage is deposited into the bin, the sensors immediately detect its characteristics, either it is wet or dry. This information triggers the motor to move the platform accordingly, directing the garbage to the appropriate compartment within the bin. For instance, if the sensor detects wet waste, the motor adjusts the platform to direct it towards the wet waste compartment. Conversely, if dry waste is detected, the platform redirects it to the dry waste compartment. The automation aspect of our system significantly reduces the need for manual intervention in sorting waste, thereby enhancing efficiency and reducing human effort. Users can simply deposit their waste into the bin without worrying about sorting it themselves, making the process more convenient and user-friendly. Additionally, the automatic sorting mechanism ensures greater accuracy and consistency in waste segregation, minimizing the risk of contamination and improving overall recycling outcomes. The Internet connectivity allows for seamless integration with a user-friendly interface (UI), accessible through web or mobile applications. This UI primarily focuses on displaying real-time data related to the detection of wet or dry levels within the bin. Users can easily monitor the status of the bin, including the current levels of wet and dry waste, as well as historical data for analysis and optimization. In addition to monitoring and control features, our smart bin also incorporates QR code technology in this project. Users can scan a QR code located on the bin to reset its status or perform other maintenance tasks. This QR code functionality simplifies user interaction with the device, eliminating the need for manual inputs or complex procedures. By leveraging the Internet in combination with automatic sorting technology and QR code functionality, our smart bin offers a comprehensive solution for efficient waste management. It not only simplifies waste disposal for users but also enhances operational efficiency and contributes to a more sustainable environment.

- Inspiration
   - Our inspiration for the smart bin project arose from a shared concern among our team of students about the environmental impact of inefficient waste management practices. We were motivated by the desire to find innovative solutions to address this pressing issue and contribute to a cleaner, healthier planet. Also, our project was driven by a genuine passion for sustainability and a desire to create positive change. We believed that by developing a smart bin that automates waste sorting and promotes recycling, we could help reduce pollution and conserve valuable resources. Throughout the project, we remained focused on the needs of our users. We understood that for our solution to be effective, it needed to be user-friendly and easily integrated into everyday life. This led us to incorporate features like QR code scanning for status reset and a simple, intuitive interface.

- Device Functionality
- Sensors:
   - Humidity and Temperature Sensor: This sensor detects the level of humidity of the garbage deposited into the bin. It helps in distinguishing between wet and dry waste, facilitating accurate sorting. Also, this sensor measures the temperature of the garbage, providing additional data for waste classification and environmental monitoring, and preventing the risk caused by high-temperature waste.

- Actuators:
   - Stepper Motor: The stepper motor is responsible for driving the platform within the corresponding bin to facilitate automatic sorting. Based on the detection from the humidity and temperature sensor, the stepper motor adjusts the position of the platform to direct garbage into the appropriate bin for sorting.

- Microcontroller (MCU):
   - A microcontroller coordinates the operation of sensors, actuators, and other related components in the system, and It processes data detected from sensors, executes sorting algorithms, and controls the movement of the stepper motor.

- Connectivity Module:
   - Wi-Fi Module: An onboard Wi-Fi module enables Internet connectivity, allowing the smart bin to communicate with external devices and platforms. Also, It facilitates data transmission to cloud-based servers for analysis and enables remote monitoring and control via web or mobile applications such as Node-RED.

- User Interface:
   - Web: A user-friendly interface accessible through web provides users with real-time data on waste composition and system performance.

- Power Supply:
   - Power Management Unit: A power management unit regulates the voltage supplied to various components of the smart bin, ensuring stable and efficient operation. It include a 5V boost and 3.3V buck for adjusting the system volatge to the what is required for different components.

- QR Code:
   - QR Code Reader: A QR code scanner is integrated into the smart bin, allowing users to perform tasks such as resetting the status of the UI showing for the bin, and users can simply use the specific QR code and make it scaned by the QR code reader located on the bin.

- Cloud Platform:
   - Cloud Server: Data collected from the smart bin, including sensor readings, and user interactions, is transmitted to a cloud-based server for storage and analysis. It also helps user easy to control the system and update the firmware. Cloud-based analytics enable optimization of waste management strategies and provide insights for continuous improvement.

- Challenges
   - For the firmware, we encountered challenges reading bin file from SD card in bootloader. There was always the same error of memory shortage which caused whole program would stuck. To overcome the memory shortage issue in the bootloader, we optimized the code by removing unnecessary tasks and freeing up memory, which do helps us to fix this error. Based on this method, the memory usage was optimized, allowing the program to execute without encountering memory shortages. Also, for the hardware, we had difficulty using uart interface because we elected the pins with different SERCOMs in our testing. To solve this problem, we made a comprehensive review of the hardware pin mapping and SERCOM configurations was conducted. By carefully reconfiguring the UART interface and selecting appropriate SERCOMs compatible with the chosen pins, the communication issues were resolved. 

- Prototype Learnings
   - It is extremely important for us to arrange pin mappings at the beginning of designing a PCBA and thoroughly reviewing component datasheets was emphasized.  The datasheet of every component is required to be checked carefully and the standard mentioned in the datasheet should be satisfied fully. Following the datasheet specifications ensures compatibility and optimal performance of hardware components. Meanwhile, the testing of the power architecture on the board is crucial to prevent voltage-related issues that could potentially damage other components,and it can minimizes risks and ensures the reliability of the hardware design.
   - If you had to build this device again, there would be lots of things to change in the beginnng of the design. First of all, we will select other buck chip for our power architecture because our buck chip does not work as expected. Beacuse of that,we had to use the buck dev board supported by teaching team. Others, we will reconfigure the UART interface by selecting appropriate SERCOMs and rearrange pins which might be undertaken to optimize communication efficiency and prevent conflicts in the system.

- Next Steps
   - Since the project is the prototype of our smart bin, for the next step, we can try to make it as the actual size of the garbage bin on the street for comprehensive real-world testing for the performance of the project.
   
- Takeaways from ESE5160
   - From this course, we learned a lot about hardware and software aspects of electronics engineering. Also, we gain valuable insights, skills and experience from this course. For the part of the hardware, we learned the intricacies of multi-layer PCB design, including the application of jumpers and test points to facilitate debugging and testing processes. Additionally, we learned the importancte of the power architecture, either buck or boost, which are the essential and significant components in ensuring the reliability and efficiency of electronic systems. These hardware skills were complemented by our software learnings, which encompassed a wide array of communication protocols, including I2C, UART, and SPI. Furthermore, we learned more about the IoT design using NODE-RED, which enhanced our understanding of connected systems and data processing. Lastly, our proficiency in real-time programming with FreeRTOS enabled us to develop responsive and reliable embedded software solutions, completing our comprehensive skill set in electronics engineering. For the whole course, we also tried Altium Designer, which is also an importent engineering tool. It is an significant industry-standard software for PCB design. Through this course, we ger more experience on designing our own PCBA and generating it as the manufacturing files for getting the actual board. These experience would empowered us to navigate the intricacies of electronic product development.
   
- Project Links
   - Provide a URL to your Node-RED instance for our review (make sure it’s running on your Azure instance!)
   - http://172.212.88.24:1880/
   - http://172.212.88.24:1880/ui/
   - Include a link to your A12G code repository
   - https://github.com/ese5160/a12g-firmware-drivers-t16-ecosavers.git


## 3. Hardware & Software Requirements
-Hardware Requirements
- Overview:

The device served as the smart bin with integrated sensors and motors for automated garbage sorting. The moisture sensor, stepper motors, distance sensor and a control interface with PC connectivity would be the key components in this device, and some other components would be used to complete the project.

- Definition:

1. Moisture sensor = MS
2. Stepper motor = SM
3. Distance sensor = DS

- Functionality:

1. HRS_01: The device shall categorize the trash in the bins.
2. HRS_02: The device shall be able to put the sorted garbage into the corresponding bins.
3. HRS_03: The device shall be initialized when the users scan the QR code.

- Review:
We satisfy the requirements of automated garbage sorting and initialization by scanning QR code. However, we deleted the function of alerting user when the bin is full, because the TX and RX pin of uart were selected incorrectly in A01G.
1. HRS_01: The on-board humidity and temperature sensor can detect the humidity of the garbage located on the platform and collect the moisture and the temperature into MCU. The data measured by the sensor will be printed in the Node Red UI, and the LED in UI will indicate what is the category of the garbage. In our testing, we put the dry paper and wet paper as the garbage close to the sensor, and the humidity and temperature were measured and presented on the two gauges in UI page.
![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/a3103f60-7df5-438b-aae3-fc065aa91960)

2. HRS_02: The direction of the stepper motor rotating can be controlled based on the humidity data measured by the sensor, which controls the garbage located on the platform slide down to corresponding bin. In our testing, we put the dry paper and wet paper as the garbage close to the sensor, and the stepper motor rotated clockwise or counter clockwise according to the humidity measured by the sensor.
![4d0c67feec7808b1bd10f5d20439f18](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/ecfdcdbb-874d-49ef-8210-810d1555e500)
![1d3e01860e7111351e88e4c7ea5e4ee](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/1ddf96c5-d1c5-451d-a243-26fec03c52dc)

4. HRS_03: All the data on UI can be initialized to 0 after scanning the specific QR code. After testing the humidity and temperature of the garbage, we can see the values of them are presented in UI. Then we scanned the unique QR code we prepared, all the data shown on the gauges in UI was initialized to 0.
 ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/66eb6f5b-a836-4d18-be5a-505d525703b5)

-Software Requirements
- Overview:

The software used in this device shall include the user interface for control, monitoring, alerting and functionality to interact with the hardware. In this project, the device will make user interaction and control for garbage sorting and bin reset, real-time monitoring of bin status, and alert reception and notification for full bin capacity. The software used here shall help the completion of the project with the support of wifi.

- Definition:

1. garbage info = number, type and any information about the garbage
2. alert = cleaning reminder

- Functionality:

1. SRS_01: The device shall transmit the information (number, type) of the garbage in the bins. 
2. SRS_02: The device shall remind the user when the either bin is full.
3. SRS_03: The device shall reset the status of the bins on the software once the QR code scanned.

- Review:
We satisfy the requirements of user interfacing, monitoring, and functionality to interact with the hardware. However, we failed the alert reception and notification for full bin capacity.
1. SRS_01: Our device can transmit the integer data of current humidity and temperature to the Node Red and present them on UI page. In our testing, we put the dry paper and wet paper as the garbage close to the sensor, and the measurements of humidity and temperature were collected and presented on the two gauges in UI page.
![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/a3103f60-7df5-438b-aae3-fc065aa91960)
2. SRS_02: We failed this requirement because we could not use our distance sensors. We removed the distance sensors from our system because the uart interface was selected incorrectly in A01G. 
3. SRS_03: All the data on UI can be initialized to 0 after scanning the specific QR code. After testing the humidity and temperature of the garbage, we can see the values of them are presented in UI. Then we scanned the unique QR code we prepared, all the data shown on the gauges in UI was initialized to 0.
 ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/66eb6f5b-a836-4d18-be5a-505d525703b5)
## 4. Project Photos & Screenshots
- Project Photos:
- Photo of the final project
- ![IMG_8498](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/9c15b9a5-5bf4-448f-b8d2-d20b55a3be87)
- ![IMG_8503](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/d296a31f-806b-46aa-afff-4e076c79f219)
- ![IMG_8500](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/0cb3baad-e006-4a4f-91f0-09c5daf80209)
- ![IMG_8502](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/ed49738e-6fd4-4608-91b7-45a35e2a5876)
- Top of PCBA
- ![3fcac1b9e25a4fdbcb3eb0f52144e6b](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/72db6da2-e132-4c49-8287-45325c23f848)
- Bottom of PCBA
- ![6ef747b942c67e4201e5aa9a895ed74](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/24a90785-67d5-499e-ac21-3a7d75a10793)
- Thermal camera image
- ![4c8c3e6929d3146c0d70b8a4db238d2](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/eef2f32c-031c-43d3-8cda-eca6bedf7279)
- 2D view of Altium
- ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/8724a835-8469-404a-a104-159c8a8e61c7)
- 3D view of Altium
- ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/b8d09c9d-fd15-44fc-82d3-e21c0a018f3f)
- Node-RED Dashboard
- ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/836025d7-2d3c-447b-8ae9-5e2f7b0dd396)
- ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/91c88c7a-b9d5-4c13-bb12-a5db71e5a5e7)
- Node-RED Backend
- ![image](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/a3103f60-7df5-438b-aae3-fc065aa91960)
- Block Diagram
- ![d212576f4a571209654ac763b374439](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/74052d34-b875-4944-b6fc-b38b061bf2fc)











