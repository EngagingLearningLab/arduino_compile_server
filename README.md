## About

This project was forked from spaceneedle's [Chromeduino](https://github.com/spaceneedle/Chromeduino) project. This aims to act as the compilation server the University of Florida STEM + C research team will use to facilitate arduino development for 5th - 6th grade students. Some notes on getting it running can be found [here](https://docs.google.com/document/d/13f7hb5UgCkwAou8Az4E6lW59aWp_nS1hyylQRfvLfwo/edit).

## Buy them a Coffee
[Spaceneedle](https://github.com/spaceneedle) has done great work with this project and has allowed the community to utilize it at will. We really appreciate this so please help out and buy them a coffee if you can.

[![Tip A Coffee](https://i.imgur.com/NUOSLzv.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=J5NT7UVN3B76J&item_name=Coding+Open+Source+Projects&currency_code=AUD&source=url)

## Run Your Own Compile Server

### Linux

Make sure you have the latest node.js installed.

 1. `git clone https://github.com/spaceneedle/Chromeduino.git`
 2. `cd "Chromeduino/Chromeduino Server"`
 3. `npm install`
 4. check install with `ls`, if there is *no* folder called `arduino-1.8.5` then run `curl https://downloads.arduino.cc/arduino-1.8.5-linux64.tar.xz | tar -xJ`
 5. `node app`
 6. go to `http://localhost:3000/version`
 
You can change the port in the config.json.

 
### Share the Love <3
 
If you have a dev VPS or something lying around, why not help the community and run a public compile server on it. (You can also add some shameless self promotion in the description)
 
 1. Make sure you have pm2 installed `npm i pm2 -g`
 2. Launch the server with pm2 `pm2 start app.js -n chromeduino`
 3. Make it run on startup `pm2 save` and `pm2 startup` read the output of those commands.
 4. Edit the server.json file with your compile server's details and then submit a pull request. If you are unsure how to do that, post an issue with the details and we'll do it for you.


### Notice of Non-Affiliation and Disclaimer:
We are not affiliated, associated, authorized, endorsed by, or in any way officially connected with Arduino AG or Google LLC (“Google”), or any of their subsidiaries or their affiliates. The official Arduino AG website can be found at https://www.arduino.cc
The names "Chrome", "Chromebook", "Chromebox", "Arduino", and "Genuino" as well as related names, marks, emblems and images are registered trademarks of their respective owners.
