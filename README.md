[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/kzkUPShx)
# a14g-final-submission

    * Team Number: 16
    * Team Name: EcoSavers
    * Team Members: Erica Feng, Xinyu Chen
    * Github Repository URL: https://github.com/ese5160/a14g-final-submission-t16-ecosavers
    * Description of test hardware: (development boards, sensors, actuators, laptop + OS, etc)   Embedded hardware, laptops, MCU and Wi-Fi, QR code reader to I2C, Distance sensor, Temperature and Humidity sensor and LED


## 1. Video Presentation

## 2. Project Summary
- Device Description
   - The project we designed is called "Smart Bin", which aims to address the issue of inefficient waste management by utilizing humidity and temperature sensor to classify garbage and sort it into appropriate bins. The primary problem it solves is the challenge of separating wet and dry waste effectively, which is crucial for efficient recycling and disposal processes. Meanwhile, in our smart bin system, the automatic sorting process is facilitated by a motor-driven platform that dynamically adjusts to sort garbage based on the detection from the humidity and temperature sensor. When garbage is deposited into the bin, the sensors immediately detect its characteristics, either it is wet or dry. This information triggers the motor to move the platform accordingly, directing the garbage to the appropriate compartment within the bin. For instance, if the sensor detects wet waste, the motor adjusts the platform to direct it towards the wet waste compartment. Conversely, if dry waste is detected, the platform redirects it to the dry waste compartment. The automation aspect of our system significantly reduces the need for manual intervention in sorting waste, thereby enhancing efficiency and reducing human effort. Users can simply deposit their waste into the bin without worrying about sorting it themselves, making the process more convenient and user-friendly. Additionally, the automatic sorting mechanism ensures greater accuracy and consistency in waste segregation, minimizing the risk of contamination and improving overall recycling outcomes. The Internet connectivity allows for seamless integration with a user-friendly interface (UI), accessible through web or mobile applications. This UI primarily focuses on displaying real-time data related to the detection of wet or dry levels within the bin. Users can easily monitor the status of the bin, including the current levels of wet and dry waste, as well as historical data for analysis and optimization. In addition to monitoring and control features, our smart bin also incorporates QR code technology in this project. Users can scan a QR code located on the bin to reset its status or perform other maintenance tasks. This QR code functionality simplifies user interaction with the device, eliminating the need for manual inputs or complex procedures. By leveraging the Internet in combination with automatic sorting technology and QR code functionality, our smart bin offers a comprehensive solution for efficient waste management. It not only simplifies waste disposal for users but also enhances operational efficiency and contributes to a more sustainable environment.

- Inspiration
   - Our inspiration for the smart bin project arose from a shared concern among our team of students about the environmental impact of inefficient waste management practices. We were motivated by the desire to find innovative solutions to address this pressing issue and contribute to a cleaner, healthier planet. Also, our project was driven by a genuine passion for sustainability and a desire to create positive change. We believed that by developing a smart bin that automates waste sorting and promotes recycling, we could help reduce pollution and conserve valuable resources. Throughout the project, we remained focused on the needs of our users. We understood that for our solution to be effective, it needed to be user-friendly and easily integrated into everyday life. This led us to incorporate features like QR code scanning for status reset and a simple, intuitive interface.

- Device Functionality
1. Sensors:

Humidity Sensor: This sensor detects the moisture content of the garbage deposited into the bin. It helps in distinguishing between wet and dry waste, facilitating accurate sorting.
Temperature Sensor: The temperature sensor measures the temperature of the garbage, providing additional data for waste classification and environmental monitoring.
2. Actuators:

Stepper Motor: The stepper motor is responsible for driving the platform within the bin to facilitate automatic sorting. Based on the readings from the humidity and temperature sensors, the stepper motor adjusts the position of the platform to direct garbage into the appropriate compartment.
3. Microcontroller:

Central Processing Unit (CPU): A microcontroller serves as the brain of the smart bin, coordinating the operation of sensors, actuators, and other components. It processes data from sensors, executes sorting algorithms, and controls the movement of the stepper motor.
4. Connectivity Module:

Wi-Fi Module: An onboard Wi-Fi module enables Internet connectivity, allowing the smart bin to communicate with external devices and platforms. It facilitates data transmission to cloud-based servers for analysis and enables remote monitoring and control via web or mobile applications.
5. User Interface:

Web/Mobile Application: A user-friendly interface accessible through web or mobile applications provides users with real-time data on waste composition, bin status, and system performance. Users can also remotely control certain aspects of the smart bin, such as initiating cleaning cycles or adjusting sorting parameters.
6. Power Supply:

Power Management Unit: A power management unit regulates the voltage supplied to various components of the smart bin, ensuring stable and efficient operation. It may include features such as battery charging and energy-saving modes.
7. QR Code Scanner:

QR Code Reader: A QR code scanner is integrated into the smart bin, allowing users to perform tasks such as resetting the status of the bin or accessing maintenance information. Users can simply scan the QR code located on the bin using a compatible device to execute these actions.
8. Cloud Platform:

Cloud Server: Data collected from the smart bin, including sensor readings, operational logs, and user interactions, is transmitted to a cloud-based server for storage and analysis. Cloud-based analytics enable optimization of waste management strategies and provide insights for continuous improvement.
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
   - Include a link to your A12G code repository


## 3. Hardware & Software Requirements

## 4. Project Photos & Screenshots
- Project Photos:
- ![IMG_8498](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/9c15b9a5-5bf4-448f-b8d2-d20b55a3be87)
- ![IMG_8503](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/d296a31f-806b-46aa-afff-4e076c79f219)
- ![IMG_8500](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/0cb3baad-e006-4a4f-91f0-09c5daf80209)
- ![IMG_8502](https://github.com/ese5160/a14g-final-submission-t16-ecosavers/assets/147103564/ed49738e-6fd4-4608-91b7-45a35e2a5876)




