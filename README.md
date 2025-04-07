# modbus-lorry-spotlight-emulator

## Install the project
This guide described procedure of installation of the Spotlight emulator on Windows 11 using "Command Prompt"

### Pre-requisites:
Python 3 for Windows is installed

### Installation procedure
1. Create "Emulator" working folder
    ```bash
    cd Emulator
    ```
2. Clone repo inside of "Emulator" folder
    ```bash
    git clone https://github.com/GrowTimeSoftware/modbus-lorry-spotlight-emulator.git
    ```
 
3. Create Virtual Environment "spotlight" using VENV
    ```bash
    py -m venv spotlight
    ```

4. Activate environment
    ```bash
    spotlight\Scripts\activate
    ```

5. Upgrade PIP
    ```bash
    py -m pip install --upgrade pip
    ```

6. Install Setup Tools package (optional)
    ```bash
    py -m pip install -U setuptools
    ```

7. Install dependencies
    ```bash
    py -m pip install -e modbus-lorry-spotlight-emulator
    ```

8. Start emulator (specify correct COM port)
    ```bash
    py py modbus-lorry-spotlight-emulator\mys_emulator\emulate_spotlight.py port=COM3
    ```

9. Emulator will start ...
    ```bash
    (spotlight) C:\Users\artur\OneDrive\Documents\GROWtime\Design\Spotlight\Emulator>py modbus-lorry-spotlight-emulator\mys_emulator\emulate_spotlight.py port=COM3
    Starting Modbus RTU Slave on port=COM7 at 115200 baud...
    ```
