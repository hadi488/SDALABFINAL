Smart Home Energy Saving System - Control Smart Light

This project demonstrates a simple implementation of a Smart Home Energy Saving System with a focus on controlling smart lights. The system is implemented in Java and allows users to authenticate, connect to a smart home hub, and control smart light features via a mobile app interface.

Project Overview

The system enables users to:
- Authenticate securely using their credentials.
- Connect to the Smart Home Hub.
- Establish a connection with smart light sensors.
- Control a Smart Light via a Mobile App with the following functionalities:
  - Turn the light ON/OFF.
  - Set a timer for the light.
  - Adjust the intensity of the light.
  - Change the color of the light.

Features

User Authentication
- Securely authenticate users using a valid username and password.

Smart Home Hub
- Manage the connection to the smart home hub to control the light.

Smart Light Control
- Turn ON/OFF the light.
- Set intensity to adjust the light's brightness.
- Change color for customized lighting.
- Set a timer for automatic control of the light.

Mobile App Interface
- Offers a user-friendly interface to control the light features.

Class Structure

User
- Handles user authentication.
  - Attributes: name (String), password (String).
  - Methods: authenticate(inputName: String, inputPassword: String): boolean.

SmartHomeHub
- Manages connection to the smart home hub.
  - Attributes: connectionEstablished (boolean).
  - Methods: establishConnection(), isConnectionEstablished().

Connection
- Represents a connection to a specific sensor.
  - Attributes: sensorName (String), sensorID (String).
  - Methods: connectToSensor().

SmartLight
- Handles operations related to the smart light.
  - Methods: setTimer(), changeState(isOn: boolean), setIntensityLevel(level: int), setColor(color: String), showAllFeatures(), turnOn(), turnOff().

MobileApp
- Provides an interface to control the smart light via the mobile app.
  - Methods: setTimer(), setState(isOn: boolean), setIntensityLevel(level: int), setColor(color: String).

Main
- The entry point of the application.
  - User authentication.
  - Connecting to the Smart Home Hub.
  - Establishing sensor connection.
  - Controlling the Smart Light using the Mobile App.

How to Run the Project

1. Clone the Repository
   Clone the project to your local machine:
   git clone https://github.com/your-username/SmartHomeEnergySavingSystem.git

2. Put All Files in One Folder
   After cloning the repository, ensure all .java files (e.g., User.java, SmartHomeHub.java, Connection.java, SmartLight.java, MobileApp.java, Main.java) are located in the same folder.

3. Compile the Java Files
   - Open Command Prompt (Windows) or Terminal (macOS/Linux).
   - Navigate to the folder where the .java files are located using the cd command:
     cd path/to/SmartHomeEnergySavingSystem
   - Compile all .java files:
     javac *.java

4. Run the Main File
   - Run the Main class to start the application:
     java Main

5. Input the Data When Prompted
   The program will ask for user input at various stages (e.g., username, password, control light settings). Use the following example credentials for authentication:
   - Username: jalalkhan
   - Password: 111

   Enter the required data as prompted to control the smart light features.

Example Interaction

Enter username:
haider
Enter password:
111
Authentication successful.
Connection to Smart Home Hub established.
Connected to sensor: Living Room Light (ID: Sensor123)

Please select an action:
1. Turn ON/OFF light
2. Set Timer
3. Adjust Intensity
4. Change Color

Enter your choice:
1
Enter the light state (true for ON, false for OFF):
true
Light turned ON.

Please select another action:
1. Turn ON/OFF light
2. Set Timer
3. Adjust Intensity
4. Change Color

Project Structure

SmartHomeEnergySavingSystem/
├── User.java
├── SmartHomeHub.java
├── Connection.java
├── SmartLight.java
├── MobileApp.java
├── Main.java
├── README.txt

License

This project is licensed under the MIT License - see the LICENSE file for details.
