# IEOR E4501 Final Project - Squirrel Tracker

## Introduction

A web application based on Django is developned using python to manage data stored in dbsqlite3. Users can see the location of the squirrels on the map as well as add/update suqirrels and check the common statistics features of all squirrels. 

## Contributors

Group Name: Project Team Illini

Contributors: Yang Rong, Zheyuan Hu

UINs: [yr2387, zh2447]

## Data Soucre

Squirrel data [**2018 Central Park Squirrel Census**](https://data.cityofnewyork.us/Environment/2018-Central-Park-Squirrel-Census-Squirrel-Data/vfnx-vebw) was used

## Management Commands
Import: A command that can be used to import the data from the 2018 census file (in CSV format). The file path should be specified at the command line after the name of the management command. 

```sh
python manage.py import_squirrel_data /path/to/file.csv
```

Export: A command that can be used to export the data in CSV format. The file path should be specified at the command line after the name of the management command.

```sh
python manage.py export_squirrel_data /path/to/file.csv
```

## Views

### Map View    
Map is a view shows the location of all squirrels. 
>Located at: /map    

### Sightings View   
Sightings is a view that lists all squirrel sightings.
>Located at: /sightings   

### Update View   
Update is a view to update some information of a squirrel sighting.    
>Located at: /sightings/<unique-squirrel-id>    

### Add View   
Add is a view to add a new squirrel sighting.   
>Located at:/sightings/add     

### Stats View   
Stats is a view with general stats about all squirrel sightings.
>Located at: /sightings/stats   

## Documentation
The official documentation is [**Squirrel Tracker**](https://docs.google.com/document/d/1SPv3fMDKiemrR86rD-S9ecvI2npz3PljDzwCfxK2x5g/edit)

