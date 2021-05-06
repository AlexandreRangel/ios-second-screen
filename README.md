sudo npm install -g cordova

git clone https://github.com/fraunhoferfokus/cordova-plugin-presentation-helloapp

cd cordova-plugin-presentation-helloapp

cordova platform add ios

cordova plugin add cordova-plugin-presentation

cordova build ios

cordova run ios


Steps to reproduce the problem:
Run the app in a physical device and connect the device to a physical external display. You should see black borders around the output display image

The problem is not possible to reproduce using a virtual external display on xcode

entry code for the ios plugin is:
./plugins/de.fhg.fokus.famium.presentation/src/ios/CDVPresentationPlugin.m
