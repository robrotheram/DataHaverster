#Plugin Events
Plugin Events get fired at different rates for example a player move event is fired hundreds of times a second while a player sleep event is fired only once ever minecraft day. Certain data such as TPS data is more important then data such as player move events
There needs to be a good way to detect if certain events fail for some reason and report that. 
There also needs to be a good schema or data structure to commonly collect data from all events as they create their own Event object such as PlayerItemBreakEvent

##
Plugin Schema
 [todo add stuff here]
