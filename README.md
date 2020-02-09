# SELF DRIVING CAR PYCON2020 WORKSHOP


## Simulation

Step 0: Install Unity from

- https://store.unity.com/download-nuo

Step 1: Go and download Udacity self driving simulator

- https://github.com/udacity/self-driving-car-sim

Step 2: Drive and collect all information in training mode and pressing rec and store it in a folder named "track"

Step 2: Open colaboratoy

- https://colab.research.google.com

Step 3: Click on File -> Open Notebook and Choose Github

Step 4: Paste https://github.com/lesthad666/pycontrack/blob/master/Behavioural_Cloning.ipynb in the field and hit ENTER.

Step 5: Execute each cell in the notebook one by one and train the model

Step 6: Download and save the model to the same level as the Drive.py file

Step 8: create the enviroment

- virtualenv sim-env 
- source ./sim-env/bin/activate or .\sim-env\Scripts\activate Windows case.
- pip install -r requirements.txt

Step 10: Run the command

- python Drive.py

Step 11: Run the simulator in autonomous mode

Resources 

https://images.nvidia.com/content/tegra/automotive/images/2016/solutions/pdf/end-to-end-dl-using-px.pdf

## Install Donkey in your PC

Step 1: install donkey
- http://docs.donkeycar.com/guide/install_software/

Step 2: create a donkeycar
- create donkey createcar --path ~/d2

Step 3: follow the instructions in your pc in order to run donkey hardware
- donkey createcar --path ~/d2
- cd ~/d2
- python manage.py drive
- open http//:localhost:8887

Step 3: Copy the generated mypilot.h5 file to your Raspberry Pi under the following location. /home/pi/d2/models/mypilot.h5

Execute the following command in your Raspberry Pi.

- cd ~/d2
- python manage.py drive --model ~/d2/models/mypilot