# VehiclePack

Vehicle Pack template for FiveM

VehiclePack makes it easy to combine all of your add-on vehicles into one huge pack for use with FiveM and allows server owners and devs to manage them all, rather than dealing with multiple separate resources.

---

## Installation

- Download the zip folder and remove `-main` from the folder's name

- Place inside your resources folder

- Add `start VehiclePack` to your `server.cfg`

**Remove the `.gitkeep` files from the `/VehiclePack/stream` and `/VehiclePack/data` folders.**

---

## Setting Up The Vehicle Pack

---

## Data folder 📂

In the `data` folder, make a folder with the vehicle's spawn code name.

For example, `newsvan` or `bmwi3`. You can usually find the vehicle's spawn name within the meta files or yft name.

Your next vehicle that you add would also need a folder and so on.

Put the meta files for **each vehicle** in their **own** folder.

Example: `VehiclePack > data > newsvan > carcols.meta`

---

## Stream folder 📂

Like with the `data` folder, make a folder with the vehicle's spawn code name and place the YFT & YTD's inside of it.

---

## fxmanifest.lua ⚙️

You won't have to modify this file. It uses [globbing](https://docs.fivem.net/docs/scripting-reference/resource-manifest/resource-manifest/#globbing) to find all `.meta` files, and every files in the stream folder is automatically used.

---

## Vehicle Names

Open `veh_names.lua` and replace "SPAWN NAME" with the spawn code of the
vehicle you want to add, it may look something like `"newsvan"` for
example.

Replace "NAME AND DESCRIPTION OF VEHICLE" with the vehicle description.

Do not remove both guillemets (`""`).

Example:
```lua
AddTextEntry("newsvan", "BBC News Van")
```

You can add more categories and keep the names in the veh_names.lua file neat and tidy if you wish, for example:

- Sports Cars
- Super Cars
- Off-Road Cars
- Police Cars
- Trains
- Military Vehicles

etc etc.

Backup in case you 'accidentally' deleted it:

```lua
AddTextEntry("SPAWN NAME", "NAME AND DESCRIPTION OF VEHICLE")
```

---

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
