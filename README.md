# Awair-uploader
This is a community based opensource tool that is capable of fetching data of Awair Element devices from Awair servers and send them to a custom endpoint.
The idea behind this project is to send these data to PlanetWatch servers in order to be able to be still elibile for rewards.

## Installation
Since the project is not yet approved by PlanetWatch Company, the software is basically only fetching data from Awair's servers. For the time being we discourage any usage of this project until PlanetWatch approves and shares the endpoints where to write our data.

If you still want to install this tool, just run clone the repository and run the following commands:
```sh
npm install
npm start
```

If you want to create a standalone version of Awair-uploader, run the following commands:
```sh
npm run make
```

Build on a Raspberry Pi:
Make sure you have RPM installed:  
```sh
sudo apt install rpm
```
Using Script Entry:
```sh
npm run makepi
```
OR
```sh
   electron-forge make --arch armv7l
```

If encounter errors related to @electron-forge/maker-squirrel, remove the following entry from the package.json file: 
```sh
    {
        "name": "@electron-forge/maker-squirrel",
        "config": {
        "name": "awair-uploader"
        }
    },
```
[https://github.com/electron-userland/electron-forge/issues/2656] (https://github.com/electron-userland/electron-forge/issues/2656)



## Contributing

The project was developed on MacOS and the building section is only for MacOS. Feel free to contribute to the project by adding your distro building section (Windows/Linux) with a Pull Request. 

We will appreciate any help to improve of the code.

Stay tuned for next updates coming in the next days!