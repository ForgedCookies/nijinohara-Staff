# Driver timetable display system
Use this system at https://forgedcookies.github.io/nijinohara-Staff/
(Nijinohara BRT only)

> [!CAUTION]
> Unreliabilities, glitches and non-legally compliant practices are used in this project. Under no circumstances shall this web app be used in real life vehicular operations.
>
A real-time timetable display system for transit drivers of various form.
Originally designed for Nijinohara BRT, a bus driving game on roblox, this web app can be adapted for other games and creative uses. 
This system is very rudimentary and basic as it-is, you are more than welcomed to derive this system for your own use.

## Timetable authoring
Authoring timetable is easy. All timetables are placed in routes.json file and 3 keys are defined for each item in the table.

1. ```"station": "example", ```
Station name in strings. 

2. ```"runningTime": ```
Designated time for running from this station to the next one. 
> [!TIP]
> Collect driving time data across multiple shifts and calculate the median value.

3. ```"remarks": "" ```
Remarks to a station.

Each object will translate to one row in the timetable itself.



