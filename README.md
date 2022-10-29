# DSMR_HomeAssistant_Flow
Node-Red flow to convert DSMR WS into Home Assistant Sensors

My (first) attempt to get the DSMR Logger values into Home Assistant using Node-Red. 
Ive got the first generation DSMR logger from 
https://willem.aandewiel.nl/index.php/2019/02/11/home-assistant-integratie-met-de-dsmr-logger/
It works with WebSocket to expose the values as json. Comming from Domotics into Home Assistant I want to port this over.
Rather then upgrading my old unit firmware and start messing with the new API through yaml I've decided to use Node-Red to fetch those json value's and dump these into individual sensors useing:
Node-Red with
 - node-red-contrib-home-assistant-websocket
 - and node-red Companion
