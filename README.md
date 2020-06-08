# 19th Round - service machine

### Overview
Run in service 1 and 2, under branch master a comparison run between PragueMetro, FreiburgTram and HelsinkiTram

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	FreiburgTrue, PragueMetroTrue, HelsinkiTrue
* Routing:	PRoPHET
* BufferSize:1000G
* TTL:		400
* msg size:	1M
* warmup:	18000
* endTime:	28800;39600
* interval:	5
* Scenario.updateInterval=0.1
* ProphetV2Router.beta=0.1;0.2;0.3;0.4;0.5;0.6;0.7;0.8;0.9;1.0
* ProphetV2Router.gamma=1.0
* btInterface.transmitSpeed=1M
* MovementModel.rngSeed=1;2;3
* Range 	80m 

# 20th Round - service 2 machine

### Overview
Run in service 2 a simulation to extract the contact behavior of Prague, Helsinki and Freiburg

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	FreiburgTrue, HelsinkiTrue, PragueMetroTrue, PragueTram
* Routing:	PRoPHET
* BufferSize:	1000G
* TTL:		400
* msg size:	1M
* warmup:	0
* endTime:	86400
* interval:	90000
* Scenario.updateInterval=1
* ProphetV2Router.beta=0.1
* ProphetV2Router.gamma=1.0
* btInterface.transmitSpeed=1M
* MovementModel.rngSeed=1
* Range 	80m 

# 21th Round - Service 1
Observe the behavior change between 8 and 11 hour run
* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:			PragueMetro, FreiburgTram, HelsinkiTram		
* Routing:			ProphetV2
* BufferSize:			1000			
* TTL:				400				
* msg size:			1M		
* warmup:			18000		
* endTime:			28800;39600		
* interval:			5
* Scenario.updateInterval:	0.1
* ProphetV2Router.beta:		0.6
* ProphetV2Router.gamma:	1.0
* btInterface.transmitSpeed:	1M
* MovementModel.rngSeed:	1
* Range: 			80m 

# 2?th Round - Service 1
Changing message Interval and compare PRoPHET and Epidemic

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	FreiburgTrue
* Routing: 	ProphetV2Router;EpidemicRouter
* BufferSize:	1000G
* TTL:		200;400;600;800
* Events1.size:	1M
* warmup:	18000
* endTime:	28800;39600
* interval:	1;3;5
* updateInt:	0.1
* ProphetV2Router.beta	0.6
* ProphetV2Router.gamma	1.0
* transmitSpeed	5M
* transmitRange	80
* rngSeed	1;2;3

# 22th Round - service 2
MaxProp in Prague, Freiburg und helsinki

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	Prague1MetroTrue,FreiburgTrue,Helsinki1True 
* router:	MaxPropRouter
* bufferSize: 	1000G
* msgTtl:	400
* Events1.size:	1M;5M
* warmup:	18000
* endTime:	28800
* interval:	1;3;5
* updateInterval: 0.1
* transmitSpeed: 5M
* transmitRange: 80
* rngSeed:	1

# 24th Round - service 1
PRoPHET und Epidemic in Freiburg

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	FreiburgTrue
* router:	PRoPHET, Epidemic
* bufferSize: 	1000G
* msgTtl:	200,400,600,800
* Events1.size:	1M
* warmup:	18000
* endTime:	28800,39600
* interval:	1;3;5
* updateInterval: 0.1
* transmitSpeed: 5M
* transmitRange: 80
* beta:		0.6
* gamma:	1.0
* rngSeed	1;2;3

# 25th Round - service 2 - 25.05
Running CGR in Prague and Freiburg, Helsinki was not able 
* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	Prague1MetroTrue,FreiburgTrue,Helsinki1True (helsinki did not work)
* router:	ContactGraphRouter
* bufferSize: 	1000G
* msgTtl:	400
* Events1.size:	1M;5M
* warmup:	18000
* endTime:	28800
* interval:	5
* updateInterval: 0.1
* ProphetV2Router.beta: 0.6
* ProphetV2Router.gamma: 1.0
* transmitSpeed: 5M
* transmitRange: 80
* rngSeed:	1

# 25\_th Round - service 1
This experiment extends the experiment of the 25th round.
It started from scratch, but added intervals 1, 3 and transmission speed of 1M

* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	Prague1MetroTrue,FreiburgTrue,Helsinki1True (helsinki did not work)
* router:	ContactGraphRouter
* bufferSize: 	1000G
* msgTtl:	400
* Events1.size:	1M;5M
* warmup:	18000
* endTime:	28800
* interval:	5;3;1
* updateInterval: 0.1
* ProphetV2Router.beta: 0.6
* ProphetV2Router.gamma: 1.0
* transmitSpeed: 1M;5M
* transmitRange: 80
* rngSeed:	1

# 26th Round - service 1
Incomplete run

* Cities: Helsinki
* Group.router=ProphetV2Router;EpidemicRouter
* Group.bufferSize=1000G
* Group.msgTtl=200;400;600;800
* Events1.size=1M
* MovementModel.warmup=18000
* Scenario.endTime=28800;39600
* Events1.interval=1;3;5
* Scenario.updateInterval=0.1
* ProphetV2Router.beta=0.6
* ProphetV2Router.gamma=1.0
* btInterface.transmitSpeed=5M
* btInterface.transmitRange=80
* MovementModel.rngSeed=1;2;3

# Continuing 26: container1Atservice 1
* Cities PragueMetro, FreiburgTram, HelsinkiTram
* Os restos da simulacao de 26\_round (helsinki) ainda estao la
* Collected on 03.06
* Group.router=ProphetV2Router;EpidemicRouter
* Group.bufferSize=1000G
* Group.msgTtl=200;400;600
* Events1.size=1M;5M
* MovementModel.warmup=18000
* Scenario.endTime=28800
* Events1.interval=1;3;5
* Scenario.updateInterval=0.1
* ProphetV2Router.beta=0.9;0.6;0.5;0.3
* ProphetV2Router.gamma=0.999885791;1.0
* btInterface.transmitSpeed=1M;5M
* btInterface.transmitRange=80
* MovementModel.rngSeed=1


# 27 Round - service 2
Incomplete run
* PragueMetro, Freiburg, Helsinki
* Group.router=SprayAndWaitRouter
* Group.bufferSize=1000G
* Group.msgTtl=400
* Events1.size=1M;5M
* MovementModel.warmup=18000
* Scenario.endTime=28800
* Events1.interval=3;5
* Scenario.updateInterval=0.1
* ProphetV2Router.beta=0.6
* ProphetV2Router.gamma=1.0
* btInterface.transmitSpeed=5M
* btInterface.transmitRange=80
* MovementModel.rngSeed=1
* SprayAndWaitRouter.nrofCopies=1;10;30;50;70;90
* SprayAndWaitRouter.binaryMode=true;false

# 28 Round - container2Atservice 1
Collected on 03.06
Epidemic, but using FIFO as queueing policy
Group.Queue = 2 - direct in the configuration file cities.txt

* PragueMetro, Freiburg, Helsinki
* Group.router=ProphetV2Router;EpidemicRouter
* Group.bufferSize=1000G
* Group.msgTtl=400
* Events1.size=1M;5M
* MovementModel.warmup=18000
* Scenario.endTime=28800
* Events1.interval=1;3;5
* Scenario.updateInterval=0.1
* ProphetV2Router.beta=0.9;0.6;0.5;0.3
* ProphetV2Router.gamma=0.999885791;1.0
* btInterface.transmitSpeed=1M;5M
* btInterface.transmitRange=80
* MovementModel.rngSeed=1

# 30 Round - containerAtsimulant
* Maps:		automatically from OSM	
* Schedules:manually created
* Cities:	Prague1MetroTrue,FreiburgTrue,Helsinki1True 
* router:	MaxPropRouter
* bufferSize: 	1000G
* msgTtl:	400
* Events1.size:	1M;5M
* warmup:	18000
* endTime:	28800
* interval:	3;5
* updateInterval: 0.1
* transmitSpeed: 1M;5M
* transmitRange: 80
* rngSeed:	1
