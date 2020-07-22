# Train Simulator global track section database tsection.dat

The purpose of this project is to provide a standardized \global\tsection.dat file that can be shared by all track section developers. 

Facing a Tower of Babel situation where every route that used extended track sections needed its own unique \global\tsection.dat file, this project includes extended sections and is compatible with the default routes. This \global\tsection.dat file includes many extended shapes from several different developers, and is completely compatible with the default routes as issued by MS/KUJU.

## Add-On Packages Covered:
|Add-On|Included In|Download at|
|-------------|------------|------------|
|Autobahn Roads|Newroads|www.train-sim.com|
|Conrail Indy Custom Roads|Newroads|www.train-sim.com|
|CykWorks Pack 1|XTracks||
|Dirt Roads|Newroads||
|DualTracks V1.1|XTracks|www.train-sim.com|
|Europeanbahn (Commercial Add-Ons)||http://www.europeanbahn.co.uk/|
|Gravel Roads v1.0|Newroads|www.train-sim.com|
|"Magnetic" Platforms (Ashphalt, Brick, Marble, White Stone)||www.uktrainsim.com|
|MTracks V1.9||http://home.comcast.net/~markhyams/mtracks|
|Newroads V4.01||www.train-sim.com, www.uktrainsim.com|
|Residential City Roads V1.0|Newroads|www.train-sim.com|
|RET Metro (Commercial Add-Ons)||www.retmetro.netmenu.nl|
|ScaleRail Beta||www.3dtrains.com|
|ScaleRoad Beta||www.3dtrains.com|
|STracks V1.0|| ?|
|UK FineScale V3.1.6||ukfs.trainsimfiles.com|
|XTracks V3.18||www.train-sim.com, www.uktrainsim.com|
|YTracks V1||www.train-sim.com|

### Other Download Sites
- Australia Steam4Me: http://www.railpage.org.au/steam4me/index.htm
- Denmark Team Routebuilders: http://team.routebuilders.dk/Engelsk/Engelsk.htm
- Germany Train DE: http://www.the-train.de

### WARNING:

If you have any \global\tsection.dat file installed other than the MS/KUJU default \global\tsection.dat file or an earlier build of this standardized \global\tsection.dat file, use of this file may initially cause MSTS to crash. See item 4 below for how to resolve this.

## How to use:

1. BACK UP YOUR EXISTING \GLOBAL\TSECTION.DAT FILE.

2. Copy the tsection.dat file included with this file into the ..\Train Simulator\Global\ folder.

3. Chris Cyko's Original L2 route (released in early 2002) is not compatible and the combination of that route and this file will cause MSTS to fail to completely start. Chris' work released after late July 2003 is compatible.

4. First use of the standardized \global\tsection.dat file will impact existing routes in one of three ways (Updating a previously installed standardized \global\tsection.dat file as no additional impact):

    - Routes which do not use any extended track sections are not impacted so long as they remain as they are. This includes all six of the default routes included in the original program and many other routes. Editing these routes may require that track section id number be updated prior to editing, see below for id updating. Any edit of a section of dynamic track, unless the route has been updated, will corrupt all other sections of dynamic track. DO NOT EDIT ANY DYNAMIC TRACK without updating the route. It is possible to edit dynamic track without realizing that the track is being edited.

    -  Routes which use extended track sections that are included in this file will require one id number updating. One means of updating id numbers is to use Okrasa Ghia's program "Horace" which is available for download in the files library at train-sim.com, search for the word Horace in the file descriptions to get the latest version. Horace is also included in the Xtracks collection.

    - Routes which use extend track sections that are not included in this file are not compatible and will likely cause program errors (known as crashes). There is a relatively easy, though possibly time consuming solution, have those sections included in the file. See below for further detail on having sections included in the file. Until the sections are added to this file, it will be necessary to move all routes using those sections out of the routes folder while using this \global\tsection.dat file.

5. If you use Horace to update the id numbers, be sure to follow all of the instructions included with the program, particularly in regards to uncompressed world files, the need to delete the .RDB, .RIT, .TDB, and .TIT files, any .BK versions thereof, and do a track data base rebuild.

6. New routes, those started after the first use of any build of this file, are fully compatible.

## How to get shapes/sections included:

1. If you have shapes/sections you wish to have included, email the .S, .SD files and the relevant tsection.dat entries to tsection@train-sim.com. New versions will be released as warranted.

2. If you are developing shapes/sections and wish to have a block of id numbers allocated, please send an email to tsection@train-sim.com with a request for the number of id numbers desired.

3. My intent is to maintain reasonable compatibility with the naming convention that MS/KUJU mostly used for their shapes. So I may request that you rename files to maintain the naming convention. If you wish, you may email your proposed .S file names with a brief description of the object to me at tsection@train-sim.com and I will let you know if the names seem appropriate.

4. All files sent will be kept in strict confidence and will not be available from me. The only file I will release is a version of the \global\tsection.dat file that includes reference to the sections and shapes. This file will only be released through train-sim.com.

5. When developing shapes, try to use existing sections. For example if your shape is for a 10 meter long track with a 1.5 meter gauge, use track section 0, rather than making a new SectionSize ( 1.5 10 ) entry.

## General Notes:

1. Please do not distribute any modified version of the standardized \global\tsection.dat file. The file may be freely distributed in its unmodified form, but it is no longer standardized if anyone else modifies it.

2. If you are distributing a route that relies on the standardized \global\tsection.dat file, please add the following to your distribution and install package:

    - Include notification in the readme file of your route that you are using the standardized \global\tsection.dat file and that it may introduce incompatibilities with routes that use extended track sections that are not included in the file.

    - Read the _INFO(Build nnnnn) line of the \global\tsection.dat file on the machine the route is being installed on (if present).

    - Do not install a lower build number over a higher build number.
    
    - If the build number ends with an alpha character, stop and ask the user to continue or skip. A trailing alpha character indicates a development beta version of the file.
    
    - If the build number is not present - if a _Skip line appears before the _INFO(Build ... line is found - warn the user and ask if they wish to continue.

3. Questions about the file itself should be send to tsection@train-sim.com.

4. Questions about any of the sections or shapes included should be directed to the developers. Each developer is listed, with contact information, and the file is sufficiently annotated to tell who the developed any section or shape.

5. Questions of general interest should be directed to the route developers forum at train-sim.com.