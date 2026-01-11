## Dependency
Install dependency before running the code.

```bash
pip install ortools
```
---

## Hyper Parameters

Initial conditions to play around with.


```python

# Panelty for having extra vehicle
ALPHA_VEHICLE_PENALTY = 200

PHYSICAL_FLEET_SPECS = {
    # Max weight capacity of each truck
    'weight': 2000,  
    # Max volume capacity of each truck
    'volume': 1000   
}

# Buffer time for vehicle to return. 
# larger : looser time constraint
# smaller: more strict time constraint
BUFFER_RETURN_TIME = 200 

# Extra vehicles to add beyond theoretical minimum
ROUTING_BUFFER = 5

```


## Result for day1


Running Vehicle Routing Problem Solver (MIP Objective: Minimize Vehicles, then Time)...

**--- Initialization Report ---**

Total Weight: 1877 | Max Truck W: 2000 -> Min Trucks: 1

Total Volume: 898 | Max Truck V: 1000 -> Min Trucks: 1

Latest Deadline found: 360

Setting Fleet Size to: 6 (Theoretical Min: 1)

OR-Tools Objective (Time Cost + Penalties): 1090

MIP Objective (Alpha*Vehicles + Total Time): 1090 (3 
vehicles * 200 + 490)   
  
    
/

/

**--- SOLUTION ---**

- Route for vehicle 0 (Depot: 0):

    - 0 -> Time(0) 16 -> Time(20) 11 -> Time(35) 5 -> Time(47) 56 -> Time(57) 54 -> Time(68) 58 -> Time(79) 57 -> Time(93) 59 -> Time(101) 15 -> Time(109) 76 -> Time(119) 77 -> Time(128) 78 -> Time(140) 72 -> Time(150) 69 -> Time(166) 68 -> Time(186) 64 -> Time(193) 13 -> Time(203) 67 -> Time(210) 66 -> Time(215) 65 -> Time(220) 63 -> Time(225) 9 -> Time(233) 3 -> Time(239) 8 -> Time(248) 1 -> Time(255) 10 -> Time(264) 0 -> Time(289)

    Route Distance: 345
    Route End Time: 289


- Route for vehicle 1 (Depot: 0):
    - 0 -> Time(0) 2 -> Time(18) 4 -> Time(32) 26 -> Time(41) 28 -> Time(62) 53 -> Time(79) 52 -> Time(93) 23 -> Time(106) 19 -> Time(114) 55 -> Time(121) 20 -> Time(139) 29 -> Time(156) 30 -> Time(161) 32 -> Time(171) 31 -> Time(176) 24 -> Time(193) 27 -> Time(205) 40 -> Time(227) 39 -> Time(233) 38 -> Time(239) 37 -> Time(246) 36 -> Time(255) 34 -> Time(269) 33 -> Time(279) 0 -> Time(316)

    Route Distance: 348
    Route End Time: 316

- Route for vehicle 3 (Depot: 0):
    - 0 -> Time(0) 6 -> Time(21) 7 -> Time(44) 14 -> Time(73) 17 -> Time(87) 12 -> Time(95) 18 -> Time(106) 25 -> Time(135) 51 -> Time(146) 35 -> Time(159) 22 -> Time(166) 50 -> Time(174) 21 -> Time(181) 49 -> Time(190) 48 -> Time(199) 47 -> Time(205) 45 -> Time(214) 44 -> Time(224) 46 -> Time(234) 42 -> Time(242) 43 -> Time(251) 41 -> Time(261) 60 -> Time(277) 75 -> Time(285) 62 -> Time(294) 61 -> Time(306) 74 -> Time(315) 73 -> Time(325) 70 -> Time(339) 71 -> Time(349) 0 -> Time(381)

    Route Distance: 397
    Route End Time: 381

**Total distance of all used routes: 1090**

**Max route end time: 381**

**Total travel time cost: 490 (The minimized sum component)**

    SUCCESS: All nodes were served.