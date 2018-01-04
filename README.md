

## Getting Started

Download/Pull the files above and download the required node packages

```
sudo npm install
```

### Prerequisites

You will require the latest version of Node.js

Functionality for spotify is using applescript and therefore this functonality will only work on macOS

You will require an ardino and servos set up on any light switches you would like to automate. I good understanding of http://johnny-five.io/ is required for physical set up of required servos, motion control etc

You will require an API key from both the new york times and open weather. These keys are to be replaced in the api.js folder

api.openweathermap.org

api.nytimes.com


### Installing

Once the prerequisites are completed go to root and run 

```
node speechServer.js
```

Then load https://localhost:3001/

This will require going through unsecure local network and allowing the microphone to listen for key words, held in the command.js file

## Running the tests

Some tests have been created for api.js, clock.js and spanish.js functions. You can run these tests at root with mocha





//Event handers for kicking off functions
const eventHandler = require('./modules/eventHandler');

//Turns the bathroom and bedroom lights to on/off

eventHandler.emit("lightsOff")
eventHandler.emit("lightsOn")

//Sends a spanish word to the front end and is read out, spanish words are held in a JSON file at root
eventHandler.emit("spanish")


//In order of events
//Sets computer volume
//Plays a defined spotify track
//Turns on the light
//Reads the weather data for the day
//Reads out loud the weather data for the day
//Reads out loud the politics news from the new york times 
//Reads out a spanish word for the day

eventHandler.emit("morning")



computer.digest(action)
