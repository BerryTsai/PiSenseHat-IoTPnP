


## Rasbian

1. Make sure all dependencies are installed before run python code. For Rasbian, you can use apt-get to install the right packages.
    ```bash
    sudo apt-get update
    sudo apt-get install -y git sense-hat python3-pip
    ```

1. Clone the preview release of the SDK to your local machine using the `master` branch
    ```bash
    git clone https://github.com/BerryTsai/PiSenseHat-IoTPnP.git
    ```
   
1. Install Azure IoT Device SDK for Python
    ```bash
    pip3 install azure-iot-device
    ``` 
   
Use Connection string 
 
1. Add connection string to your Raspberry Pi enviroment 
    ```bash
    nano ~/.bashrc
    ```
   Add device conection string from your IoThub to last line
   ```bash
   export IOTHUB_DEVICE_CONNECTION_STRING="HostName=xxxxxxxx;DeviceId=xxxxxxxxx;SharedAccessKey=xxxxxxxxxxxxxxxxxxxxxxxxxxx"
   ```
   Ctrl-o Y Save,
   Ctrl-x quit

1. Reboot Raspberry Pi  
    ```bash
    sudo reboot now
    ```   
   
1. Go to sample folder,  default_component or multi_component
    ```bash
    sudo reboot now
    ```   
    ```bash
    cd PiSenseHat-IoTPnP
    cd default_component or cd multi_component
    ```

1. Run python sample code for Sensehat 
    ```bash
    python3 pnp_snesehat.py or python3 pnp_multi_sensehat.py
    ```  

