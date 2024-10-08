# Resploit - Network and Security Scanning Tool
 Resploit is a GUI-based network and security scanning tool built with Python and PyQt5. It supports popular tools like Nmap, Wireshark, and Metasploit, allowing users to easily select tools, choose predefined scan options, input custom arguments, and view command output—all within a user-friendly interface. Perfect for quick, efficient scans.


## Table of Contents
- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [Tests](#tests)
- [Deployment](#deployment)
- [Built With](#built-with)
- [Acknowledgments](#acknowledgments)

## Features
- **Tool Selection:** Choose from a wide range of network and security tools including Nmap, Wireshark, Metasploit, Nessus, Aircrack-ng, Burp Suite, Nikto, Hydra, John the Ripper, OpenVAS, SQLmap, Snort, and DirBuster.
- **Predefined Scan Options:** Select from various predefined scan types tailored for each tool.
- **Custom Command Arguments:** Add custom command-line arguments to suit your specific needs.
- **Output Display:** View command execution results directly within the GUI.
- **Clear Output:** Clear previous results with a single click to prepare for a new scan.

## Demo
[[Resploit Demo]![thumbnail](https://github.com/user-attachments/assets/8a00fd00-3bda-4363-b906-82b80c7610ef)
](https://drive.google.com/file/d/1pOwGlngHDP4ExZ2Uq9NIBeNU-M3mq9P8/view?usp=sharing)
*Click the image above to watch a demo video of Resploit in action.*

## Installation

### Prerequisites
Ensure that you have Python 3.x and `pip` installed on your system. Additionally, the necessary security tools (e.g., Nmap, Wireshark) should be installed and accessible via the command line.

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/vijaykumargowdakk/resploit.git
   cd resploit
   ```

2. **Install Python Dependencies**
   ```bash
   pip install PyQt5
   ```

3. **Install Security Tools**
   Install the required security tools like Nmap, Wireshark, Metasploit, etc., depending on your needs.

## Usage

1. **Start the Application**
   ```bash
   python app.py
   ```

2. **Select a Tool**
   - Choose the desired tool from the dropdown menu.

3. **Select a Scan Option**
   - Based on the tool, select a predefined scan option.

4. **Input Details**
   - Enter the target IP address and any additional arguments required.

5. **Run the Scan**
   - Click on "Run Scan" to execute the selected command. The output will be displayed in the text area.

6. **Clear Output**
   - Use the "Clear Output" button to clear the results.

## Configuration
- **Updating Scan Options:** You can add or modify scan options by editing the `update_scan_options` method in the `ScannerApp` class.
- **Custom Tools:** To add a new tool, modify the `initUI` and `update_scan_options` methods to include the tool and its corresponding scan options.

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Create a Pull Request.

## Tests
To run tests, you can set up unit tests for each tool and their respective commands. Add tests to ensure that the right commands are being executed and the output is correctly handled.

1. **Install Testing Framework**
   ```bash
   pip install pytest
   ```

2. **Run Tests**
   ```bash
   pytest
   ```

## Deployment
To deploy this application:
1. Ensure all dependencies are installed.
2. Package the application using a tool like PyInstaller.
   ```bash
   pyinstaller --onefile app.py
   ```
3. Distribute the generated executable to users.

## Built With
- **[Python](https://www.python.org/):** The core programming language used.
- **[PyQt5](https://riverbankcomputing.com/software/pyqt/intro):** For creating the GUI.
- **Various Security Tools:** Nmap, Wireshark, Metasploit, etc., which are leveraged for the scanning operations.
  

## Acknowledgments
- **PyQt5 Documentation** for guidance on building the GUI.
- **Open-source security tools** that make Resploit possible.

---

This README structure provides a comprehensive guide to the project and serves as a solid foundation for users, contributors, and developers alike.
