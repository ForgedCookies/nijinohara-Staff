# Driver timetable display system
Use this system at https://forgedcookies.github.io/nijinohara-Staff/
(Nijinohara BRT only)

> [!CAUTION]
> Unreliabilities, glitches and non-legally compliant practices are used in this project. Under no circumstances shall this web app be used in real life vehicular operations.
>
A real-time timetable display system for transit drivers of various form.
Originally designed for Nijinohara BRT, a bus driving game on roblox, this web app can be adapted for other games and creative uses. 
This system is very rudimentary and basic as it-is, you are more than welcomed to derive this system for your own use.


## How do use (as consumer)?
1. Select a route you are driving today.
2. Once in the driving interface, press "Start Driving"
3. Press Already arrived for starting station, if applicable
4. Press Already Departed once your bus/train/cardboard box started to move
5. Once you have finished the whole route, either press End shift, or;
6. ....Press Turnaround which allows you to run the route back to your starting point. You will have roughly 15 seconds to key in your destination rollsign, configure fareboxes, etc
DO NOT press turnaround button if you are taking a break!

## Timetable authoring
Authoring timetable is easy. All timetables are placed in routes.json file and 3 keys are defined for each item in the table.
If you get dizzy reading code you can load a JSON file into this site and edit: https://forgedcookies.github.io/JSONNest-Edit/

### Keys in each object
1. ```"station": "example", ```
Station name in strings. This station is called "example".

2. ```"runningTime": ```
Designated time, in seconds, allocated for running from this station to the next one. 
> [!TIP]
> Collect driving time data across multiple shifts and calculate the median value.

3. ```"remarks": "" ```
Remarks to a station.

4. ```"dwellTime"```
How long, in seconds, the service is scheduled to stop at a station

5. ```"isPass":```
Do we skip or pass this station?
True = pass
False = stop

Each object will translate to one row in the timetable itself.



