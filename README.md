# Cordova FileChooser Plugin

Originally created by [don](https://github.com/don/cordova-filechooser). 

Forked to create an NPM compatible package, so it's installable via the CLI. 

# Requirements

Requires Cordova >= 2.8.0

# Installation

Install with Cordova CLI
	
	$ cordova plugin add http://github.com/don/cordova-filechooser.git

Install with Plugman 

	$ plugman --platform android --project /path/to/project \ 
		--plugin http://github.com/don/cordova-filechooser.git
		
# Usage

API

	fileChooser.open(successCallback, failureCallback);

The success callback get the uri of the selected file

	fileChooser.open(function(uri) {
		alert(uri);
	});
	
Screenshot

![Screenshot](filechooser.png "Screenshot")

TODO rename `open` to pick, select, or choose.
