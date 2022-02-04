Open fxmanifest in Notepad++ or something similar and replace
CAR NAME HERE with the vehicle's spawn code.


Example: if the vehicle's spawn code is 'newsvan' replace 'CAR NAME HERE' with 'newsvan'.

Tip: Copy and paste the provided template and paste it a few times so you can easily rename CAR NAME.

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

