# VehiclePack

Vehicle Pack template for FiveM

VehiclePack makes it easy to combine all of your add-on vehicles into one huge pack for use with FiveM and allows server owners and devs to manage them all, rather than dealing with multiple separate resources.

-----------------

## Installation

- Download the zip folder and remove `-main` from the folder's name

- Place inside your resources folder

- Add `start VehiclePack` to your `server.cfg`

**Remove the `.gitkeep` files from the `/VehiclePack/stream` and `/VehiclePack/data` folders.**

-----------------

# Setting Up The Vehicle Pack

-----------------

# Data folder 📂

In the 'data' folder, make a folder with the vehicle's spawn code name. 

For example, 'newsvan' or 'bmwi3`. You can usually find the vehicle's spawn name within the meta files or yft name.

Your next vehicle that you add would also need a folder and so on.

Put the meta files for **each vehicle** in their **own** folder.

Example: `VehiclePack > data > newsvan > carcols.meta`

-----------------

# Stream folder 📂

Just place the YFT & YTD's of all of the vehicles here :)

-----------------

# fxmanifest.lua ⚙️

Open fxmanifest in Notepad++ or something similar and replace 'CAR NAME HERE' with the vehicle's spawn code.

Example: if the vehicle's spawn code is 'newsvan' replace 'CAR NAME HERE' with 'newsvan'.

Tip: Copy and paste the provided template and paste it a few times so you can easily rename CAR NAME.

```lua

Back up:


 --CAR NAME HERE
files {
    'data/CAR NAME HERE/vehicles.meta',
    'data/CAR NAME HERE/carvariations.meta',
    'data/CAR NAME HERE/carcols.meta',
    'data/CAR NAME HERE/handling.meta',
    'data/CAR NAME HERE/vehiclelayouts.meta',
}

data_file 'HANDLING_FILE'            'data/CAR NAME HERE/handling.meta'
data_file 'VEHICLE_METADATA_FILE'    'data/CAR NAME HERE/vehicles.meta'
data_file 'CARCOLS_FILE'             'data/CAR NAME HERE/carcols.meta'
data_file 'VEHICLE_VARIATION_FILE'   'data/CAR NAME HERE/carvariations.meta'
data_file 'VEHICLE_LAYOUTS_FILE'     'data/CAR NAME HERE/vehiclelayouts.meta'
```
-----------------

# Vehicle Names 

Open veh_names and replace "SPAWN NAME" with the spawn code of the
vehicle you want to add, it may look something like rmodbmw320 for
example.

Replace "NAME AND DESCRIPTION OF VEHICLE" with the vehicle description.

Do not remove the " ". 

Example:

    AddTextEntry("newsvan", "BBC News Van")


You can add more categories and keep the names in the veh_names.lua file neat and tidy if you wish, for example:

- Sports Cars
- Super Cars
- Off-Road Cars
- Police Cars
- Trains
- Military Vehicles

etc etc.

Backup in case you 'accidentally' deleted it:

```

    AddTextEntry("SPAWN NAME", "NAME AND DESCRIPTION OF VEHICLE")

```

-----------------

At the end, your file organization should look like this:

```cmd
VehiclePack
| stream
| | vehiclename
| | | ytd
| | | ...
| | ...
| data
| | vehiclename
| | | carcols.meta
| | | handling.meta
| | | ...
| | ...
```
