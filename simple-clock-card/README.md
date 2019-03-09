# Simple Clock Card
A text based clock for Homeassistants' Lovelace ui

![24h clock](https://i.imgur.com/n37gyxZ.png)  

![military without seconds](https://i.imgur.com/ej4AFO3.png)

## Usage
- Download the files in this folder to your 'www' folder in the hass config directory.
- In your *lovelace-ui.yaml* or in the raw config editor add the following to resources:

		resources:
		  - type: js
	        url: /local/<your_folder>/simple-clock-card.js
- In your *lovelace-ui.yaml* add the following lines to a view in '*cards:*' or add this via the ui as a *'manual card'*:

		- type: 'custom:simple-clock-card'

thats it!
		

## Options
|option| default|description| 
|--|--|--|
|  use_millitary| true| When false shows a 24h format clock instead of a 12h format clock with AM/ PM|
|  hide_seconds| false| When true hides the seconds

## Example
- show a 24h clock without seconds:
	
		- type: 'custom:simple-clock-card'
		  use_military: false
		  hide_seconds: false
