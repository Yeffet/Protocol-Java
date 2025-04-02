This Java console application simulates a garage that repairs different types of vehicles (Motorcycle, Car, Truck). Each vehicle has a specific fix time, and the program handles repairs one by one until all vehicles are done.

Files Overview
Car.java
A Vehicle subclass representing a car. Implements getFixTime() (5 seconds) and fixed() with a custom message.

DB.java
Maintains a simple in-memory list of Vehicle objects. Provides methods to add and retrieve vehicles.

Garage.java
Manages the repair cycle using a scheduled task. Repairs vehicles based on their getFixTime(), calls their fixed() method upon completion, and notifies when all repairs are done.

MainScreen.java
The main entry point. Prompts the user for vehicle type and name, instantiates the appropriate Vehicle, stores it in DB, and starts the Garage process.

Motorcycle.java
A Vehicle subclass representing a motorcycle. Implements getFixTime() (3 seconds) and fixed() with a custom message.

Truck.java
A Vehicle subclass representing a truck. Implements getFixTime() (10 seconds) and fixed() with a custom message.

Vehicle.java
An abstract class that defines common vehicle properties and requires each subclass to specify its fix time and how it is “fixed.”

module.xml
A project configuration file (often used by IDEs such as IntelliJ), detailing module settings but not directly affecting program logic.
