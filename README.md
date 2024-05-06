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
   - Humidity and Temperature Sensor: This sensor detects the moisture content of the garbage deposited into the bin. It helps in distinguishing between wet and dry waste, facilitating accurate sorting. Also, this sensor measures the temperature of the garbage, providing additional data for waste classification and environmental monitoring.

- Actuators:
   - Stepper Motor: The stepper motor is responsible for driving the platform within the bin to facilitate automatic sorting. Based on the detection from the humidity and temperature sensors, the stepper motor adjusts the position of the platform to direct garbage into the appropriate bin.

- Microcontroller (MCU):
   - : A microcontroller serves as the brain of the smart bin, coordinating the operation of sensors, actuators, and other components. It processes data from sensors, executes sorting algorithms, and controls the movement of the stepper motor.

- Connectivity Module:
   - Wi-Fi Module: An onboard Wi-Fi module enables Internet connectivity, allowing the smart bin to communicate with external devices and platforms. It facilitates data transmission to cloud-based servers for analysis and enables remote monitoring and control via web or mobile applications.

- User Interface:
   - Web: A user-friendly interface accessible through web provides users with real-time data on waste composition and system performance.

- Power Supply:
   - Power Management Unit: A power management unit regulates the voltage supplied to various components of the smart bin, ensuring stable and efficient operation. It include a 5V boost and 3.3V buck for adjusting the system volatge to the volatge required for different components.

- QR Code:
   - QR Code Reader: A QR code scanner is integrated into the smart bin, allowing users to perform tasks such as resetting the status of the UI showing. Users can simply use the specific QR code and make it scaned by the QR code reader located on the bin.

- Cloud Platform:
   - Cloud Server: Data collected from the smart bin, including sensor readings, and user interactions, is transmitted to a cloud-based server for storage and analysis. It also helps user easy to control the system and update the firmware. Cloud-based analytics enable optimization of waste management strategies and provide insights for continuous improvement.

- Challenges
   - Where did you face difficulties? This could be in firmware, hardware, software, integration, etc.
   - How did you overcome these challenges?
- Prototype Learnings
   - What lessons did you learn by building and testing this prototype?
   - If you had to build this device again, what would you do differently?
- Next Steps
   - What steps are needed to finish or improve this project?
- Takeaways from ESE5160
   - What did you learn in ESE5160 through the lectures, assignments, and this course-long prototyping project?
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

## 4. Project Photos & Screenshots
- Project Photos:
- ![IMG_8498](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/9c15b9a5-5bf4-448f-b8d2-d20b55a3be87)
- ![IMG_8503](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/d296a31f-806b-46aa-afff-4e076c79f219)
- ![IMG_8500](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/0cb3baad-e006-4a4f-91f0-09c5daf80209)
- ![IMG_8502](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/ed49738e-6fd4-4608-91b7-45a35e2a5876)




