---
sidebar_position: 1
description: "A simple how-to guide to the editor interface."
---
# The Basics

In order to go about creating your own C3 scenarios, you will need to download and install the Caesar 3 Assigment Editor, available from Gamespot (amongst other places). Once installed, this programme runs as a stand-alone package, accessible from outside Caesar 3.

What follows is a brief step-by-step guide to the use of the Editor. Much of this information has been pilfered from the excellent ReadMe file that comes with the editor, but there will be some new bits and pieces here and there.

To create a Caesar 3 scenario, there are essentially three tasks that need to be performed, each of which will now be considered in turn.

- Choose the Empire State
- Create the terrain
- Set the Map Attributes

## Empire States

The empire selection screen is accessed from the menu bar at the top of the screen ('Empire' --> 'Choose Location'). You must then choose one of the forty available empire states to base your scenario around. The choice of empire state is a very important one, since this determines the raw materials your city will be able to produce, and what goods you will be able to trade. Unfortunately, there is no way to create your own empire state, with customised trade routes and raw materials, but the range of options available is quite extensive.

In my opinion, choosing the empire state is the most important step in the creation of a new scenario. The trading opportunities determine the amount of money a city can make in its early years, and hence the speed with which the city can expand its tax base. The choice of empire state also places constraints on the map design. For example, an empire state that is reliant on sea trade needs to have a substantial body of water, capable of supporting several docks. Similarly, an empire state where farming is of paramount importance should have ample farmland.

To help in the selection of a suitable empire state, I have created a document listing all the available empire states, the raw materials available, and their trading opportunities. It's a little large to be included here, so I've added it to the Download section here.

## Terrain

The first thing you should do when creating a new map is to choose its size. To do this, choose the 'New Map' option from the 'File' menu at the top of the screen and then select a map size.

All of the terrain editing buttons are located on the bottom half of the toolbar on the right side of the screen. While the main screen section gives a close-up picture of the terrain you are editing, a broader overview can be seen on the radar map at the top of the toolbar.

The 15 terrain editing buttons on the toolbar are:

- **Grass**:
Clears all other types of terrain (except elevation)
- **Trees**:
Timber yards must be built next to trees (or scrub).
Trees are impassable, but may cleared.
- **Water**:
All maps must have at lest some water.
Required for fishing, sea trade, and clay pits.
- **Elevation**:
Raise and lower land, and build access ramps.
Raised land is not accessible unless you build an access ramp.
- **Scrub**:
Work exactly like trees, look different.
- **Rocks**:
Required for marble quarries or iron mines.
Rocks are impassable.
- **Farmland**:
Required for farms of all types
- **Road**:
Not necessary but used by most designers to link the entry and exit points.
- **Brush Size**:
Sets the brush size (the area you alter with a single mouse click).
- **Earthquake**:
Sets the epicentre of the earthquake (if in use).
- **Invasion Points**:
Specify up to eight invasion points on a map.
- **People points**:
Set entry and exit points. All maps must have both-
- **River Points**:
Set river entry and exit points. Required for sea trade.
- **Native Structures**:
The area around a native building cannot be built on until natives are pacified
Native centres are required for trade with natives-
- **Animals**:
Set fishing and animal spawn points.

The interface here is reasonably intuitive, and extremely straightforward. You just point and click. The brush size button is, in my opinion, the most important. I tend to use a medium or large brush size to sketch out the general features of my map, and then switch to the tiny brush to tidy things up. I have found this allows me to create realistic looking terrain. I usually add at least one native village, and a few herds of animals, to provide some eye candy.

When designing the terrain, it is important that you work within the limitations imposed by your choice of empire state. You will look a bit silly if you end up with a map containing acres of farmland, but no farms to put on there!

Of all the terrain types, water is the most important. It is required for sea trade, fishing, the placement of clay pits, and also for evolution of housing beyond the lowest possible level. You should ensure that you have enough water on the map for all of the water dependent industries you wish the player to be able to use. Alternatively, you can limit the availability of water to force the player to make strategic decisions as to how to use that water. When you require a player to cross a body of water, you should ensure that a bridge can be built across it.

You can do similar things with the other resource types. If you want the player to be able to build lots of farms, timber yards, marble quarries, or iron mines, then you need to place a sufficient amount of farmland, trees (scrub), or rocks on the map. Again, you can choose to limit the availability of these resources to force the player into making strategic decisions.

The entry and exit points are also absolutely vital. Every map needs people points, or no housing can be built. If you want sea trade to be possible, you must set river points. Similarly, invasions require at least one valid invasion point. When placing entry and exit points, you should ensure that there is a clear path between them. It is a common convention to link the map entry and exit points with a road. This ensures that there is a clear path, and also gives the player a clear indication of the location of entry and exit points.

As a final point, Caesar 3 has three separate terrain sets (corresponding to the three climate types: Northern, Central, and Desert). These are interconverted using the Map Attributes panel, and are discussed in detail below. Unsurprisingly, the three terrain sets look different!

## Map Attributes

Once the first two parts are out of the way, all that remains is to set the map attributes. I say 'all' with a slightly wry smile on my face, because the attributes are what turns a mediocre map into a brilliant map or a terrible map. The map attributes panel is accessed by clicking this button on the toolbar: Map Attributes

You are then faced with an array of buttons which allow you to set up the scenario to your liking. Most of these open a submenu with various further optionas available to you.

- At the very top is a box that has the words "Brief description" in it. Once your map is finished, it is loaded via the City Construction Kit menu. The 'Brief description' you insert here will be displayed when you select your map, together with the win criteria,and the picture displayed at the bottom left of the attributes panel (which you can change using the arrow keys).
- **Starting Conditions**:
  Here you set the players rank, the starting date, the starting funds and value of rescue loan, all of which are farily straightforward. The remaining items are less simple. You can choose to have a scenario in which Rome supplies wheat. If you do, you should be aware that houses cannot get a second type of food, so housing cannot evolve beyond large insulae. The maximum possible prosperity rating is therefore 65.

  If you design a map where sea trade is possible, you should normally have flotsam turned on. This will flow from the river entry point to the river exit point, and indicates to the player where they should be building docks.

  The three 'milestone' years are the last thing you should set. These are times by which players should have completed 25%, 50%, and 75% of their mission goals. Success gives a five point favour bonus, while failure results in a two point favour loss.
- **Terrain Set**:
Cycle between the three available terrain sets: Northern, Central, and Desert. In addition to looking different, the different terrain also affect gameplay in the following ways:

  1. Fire risks are greatest in the desert, moderate in central provinces, and zero in northern provinces.
  2. The animals present vary with terrain set. You find wolves in the north, sheep in central provinces, and zebra in the desert.
  3. Fountains have a range of 3 tiles in the desert, and 4 tiles everywhere else.
  4. Wheat farms produce 9.6 cartloads of food per year in northern provinces, and 19.2 cartloads per year elsewhere.
- **Requests**:
  Schedule up to twenty requests here. For each request, specify when it happens, what is being requested, how much of it is needed, and how long you have to respond. The default response time is five years and I would recommend that you make it quite a lot less than that. I never set response times of more than two years, but that is simply a personal preference. Ensure that you do not request something that the player cannot produce or import! You should also be aware that troop requests are scheduled as invasions, not requests.
- **Enemy**:
If you intend to schedule invasions, select an enemy from the available list here.
- **Invasions**:
You may schedule up to twenty invasions and/or troop requests here. You should set the timing for the invasion/request, using the top left box, then set the strength of the enemy army using the next box. The strength of the invasion is the number of enemy soldiers that attack, not the number of legions or armies! You should then set the type of invasion. For a troop request, set this to 'Distant Battle'. Otherwise, you can choose between the enemy selected earlier, or local raiders. The important point here is that the player is warned of the approach of an enemy army, whereas a native uprising happens without any warning whatsoever.
For invasions, you should then set the tactics for the invaders (what they will preferentially attack), and then select an invasion point. This invasion point must be one that you have already placed on the map when editing it.
- **Buildings Allowed**:
Disallow certain buildings (and groups of buildings) by clicking on them so they turn red. If a certain building cannot be built, for example oracles and large temples in scenarios where there is no marble, then you should disallow it.
- **Win Criteria**:
Set the winning criteria for the scenario. If you want a criterion to be necessary for victory, the first column must read 'Yes'. You then set the numerical criteria in the second column.
- **Special Events**:
Most of these are random events that happen at various junctures during the scenario. Only use these if they are relevant, so don't have sea trade problems when there is no sea trade. I would also caution against setting up wage increases without wage decreases also enabled. Wages can otherwise spiral out of control.
The remaining events are one-time only occurences. A change of Emperor is meant to reset the Favour Rating to fifty, but I've never managed to get it to work properly! Gladiator revolts can cause a lot of damage, but can be avoided by deleting all gladiator schools a month before it happens. The earthquake has three different settings, minor, average, and major. As you might expect, these alter the severity of the earthquake. For an earthquake to function, an earthquake point must be placed on the map.
- **Price Changes**:
Set up to 20 price changes over the course of the level. Specify the commodity, and by how much its price will change.
