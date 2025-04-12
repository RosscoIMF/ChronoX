CHRONOX v1.01
Software for the HT-X3006 WiFi Series Chronograph

1. Launching the Application

    Run the Program:
    Double-click the executable (ChronoX.exe) to launch the program. The program opens with GUI that displays real-time chronograph data from the sensor.

2. Understanding the Main Screen

   Top Section (Digital Displays):

   Kinetic Energy & Muzzle Velocity:
        Two large digital readouts display your current kinetic energy and muzzle velocity.

   Wi‑Fi Icon: In the middle column, there is a Wi‑Fi icon:
        Blue Icon: Indicates a successful connection to the sensor.
        Red Icon: Indicates no active connection or a connection issue.

   Control Buttons: Two round buttons are present beneath the digital displays:
         Toggle Button: Switches between IMPERIAL (ft-lbs, fps) and METRIC (J, m/s) units.
         Reset Button: When pressed, resets the displayed values. Press and hold for 3 seconds to clear the CSV data files.

4. Navigating the Tabs

   At the bottom of the window, you will find multiple tabs with additional features:

    VELOCITY: Displays a real-time velocity graph of your measurements.

    ENERGY: Shows a kinetic energy graph.

   Tip: If the energy exceeds a certain threshold, the graph will highlight these points (e.g., in red).

PELLET DB (Pellet Database):
    Search: Use the search box to filter pellets by description.
    View & Select: Click on a pellet to view detailed information and automatically set its weight for calculations.

RIFLE DB (Rifle Database):
     Search: Filter rifles by make or model.
     Select a Rifle: Click an item to update the muzzle velocity display with your chosen rifle’s details.

Toggle Sorting: Clicking the “Type” column toggles the sorting order (for example, prioritizing “PCP” if applicable).

SETTINGS: Provides options such as enabling the UK Regulatory Warning. Adjust these settings to suit your preferences.

ABOUT: Contains information about ChronoX, a brief description of the software’s purpose, and important disclaimers regarding sensor accuracy.

4. Additional Features

    Graph Context Menu: Right-click on either graph (VELOCITY or ENERGY) to reveal extra options:
          Export Graph as PNG: Save a screenshot of the current graph.
          Save Details to Text File: Export the current velocity and energy data readings to a text file.

    Automatic Updates: The application continuously monitors a CSV file for new data. Displays and graphs update automatically to reflect the latest measurements.

    Background Processes: Internally, ChronoX uses a Flask server for inter-process communication and a monitoring thread that keeps real-time track of sensor readings.

5. Tips for Best Use

    Unit Switching: Use the toggle button to switch between measurement systems, which will update labels, graphs, and numerical displays.

    Data Reset: If you ever need to clear the recorded CSV data (for a fresh start), press and hold the reset button for 3 seconds.

    Resource Awareness: The application is designed to correctly load resource files (such as the Wi‑Fi icons) whether run as a script or from an executable—just be sure you have included the “Data” folder with your build.

These basic instructions should get you started with ChronoX. Enjoy!
