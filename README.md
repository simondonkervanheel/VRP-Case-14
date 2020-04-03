# VRP-Case-14

## Remarks:
Solver  should  be  able  to  run  using  only  the  locations’ coordinates.
The delivery of a request can not be split:  if several units are requested, all have to bedelivered by one vehicle on the same day.
It is not allowed to visit a location, and leave there some tools that arenot requested.

## instance structure
Sections always appear in the same order, additional line breaks or spaces may be present between.
Entries in a line are separated by tabs

General info

Vehicle related costs 

Tools (ID, Size, Cap., Cost)

Coordinates(0=depot) (ID, X, Y)

Requests (ID, Loc., S.day, E.day, Stay, Tool, Qty)

Distance Matrix(optional)

## solution structure
`DATASET = VeRoLog solver challenge 2017

NAME = testInstance`

`MAX_NUMBER_OF_VEHICLES = 1
NUMBER_OF_VEHICLE_DAYS = 12
TOOL_USE = 3 1 1 3
DISTANCE = 1028
COST = 113828`

## Git vanuit je terminal
Clone command van deze map `git clone https://github.com/FallBosk/VRP-Case-14`.

Voordat je begint met werken `git pull`.

Om je wijzigingen up te loaden:
1) `git add <files>`
2) `git commit -m "message"`
3) `git push origin master`

## Validator
Gebruik dit voor de validatior:
`pyhton3 SolutionCVRPTWUI.py -i instance.txt -s solution.txt`
