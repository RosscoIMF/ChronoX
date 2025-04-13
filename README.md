ChronoX - Ballistic Chronograph Analysis Software v1.01 for Windows x86/x64.

ChronoX is a Python-based GUI application designed to interface with the HT-X3006 chronograph, providing real-time monitoring, analysis, and visualization of projectile velocity and kinetic energy. Built for airgun enthusiasts and hobbyists, it offers tools to track performance metrics, manage equipment databases, and ensure compliance with regulatory standards.

Key Features

Real-Time Monitoring:

Track muzzle velocity, kinetic energy, standard deviation, extreme spread (ES), and averages.
Live-updating graphs for velocity and energy trends over 250 shots.

Unit Conversion:

Toggle between imperial (fps, ft-lbs) and metric (m/s, joules) units instantly.

Data Management:

Pellet & Rifle Databases: Search and select from CSV-stored profiles (e.g., pellet weight, rifle specs).
Export Options: Save graphs as PNG or shot-by-shot data to text files.
CSV Integration: Automatically reads/writes gui_data.csv for persistent data storage.

Safety Compliance:

UK regulatory warning toggle to highlight shots exceeding energy limits (12 ft-lbs or 16.27 J).

Modern UI:

Retro GUI design based on the old Casio digital watches from the 80s with animated LCD displays.
Responsive tabs for graphs, databases, settings...

Sensor Integration:

Wi-Fi status indicator for HT-X3000 sensor connectivity.
Flask-based backend for inter-process communication (IPC).

Technologies Used

Frontend: PyQt5, PyQtGraph
Backend: Flask (for REST API), threading
Data Handling: CSV, JSON, QSettings

Use Cases

Optimize air rifle performance by analyzing velocity consistency.
Validate compliance with local energy regulations.
Catalog and compare pellets/rifles for precision tuning.

====================================================================

Instructions:

Turn on your HT-X3006 Chronograph and ensure that WiFi is enabled. ChronoX automatically detects and connects to the HT-X3006.

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
