# DataHaverster
Minecraft Server(Bukkit/Spigot/paper) Analytics  tool Gathers all Event data and send to remote service for data processing 

##The Platform
The DataHavester platform will consists of 3 parts, 

1. The Minecraft Plugin 
  - This will be a drop in plugin for minecraft servers to use to gather all (well 90%) events the plan is to capture as most data as possible. The plugin will expand adding more listeners to popular plugins like worldguard worldEdit etc
  - The Plugins will batch the events up and send the to the server at certain intervals for example player events may be set once every second while tps data will be sent every 10 seconds. theses numbers are arbitary and may change in the future there role is to stop the server being overloaded. 
  - The data will be sent to the processing server to storage. 

2. Processing / Storage Server. 
  - This will store the data from each minecraft server there will be minimal inital processing on the data the aim will try and get the data into a scaleable database as fast as posible
  - The system should be able to handle multiple different servers connecting to it
  - Auth is gonna be tricky API keys or client certs may be used to authenticate with the server currently undecided

3. Viewer 
  - This third component may be a sperate service that will hook onto the data provided by (2) via a external API or some internal functions
  - This viewer will help server owners see the current status of the server and more importantly be able to track any issues that would not be instantly noticeable viewing the logs


Other Ideas
 - Macheine Learing to detect unoptimal configurations or beable to pick up extra ordinary behaviour
 - Based of the above be able to produce reports on the status of the server weekly monthly, Average player count TPS etc
 - Long Term create a Payed service????? probably wont happen I am lazy

##FAQ


