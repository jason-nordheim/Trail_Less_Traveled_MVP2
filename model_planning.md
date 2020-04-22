# Nouns 
---- 


## Location 
This the place of something 
### Attribtes (property)
- `Location.latitude`
  - variable_type: `float` 
  - required: y 
- `Location.longitude` 
  - variable_type: `float` 
  - required: y 
### Data Source 
----
## Trail (Hannah)
### Attributes 
- `Trail.traffic_level` 
  - description: describes the amount of traffic at a particular trail, at current time 
  - method_type: 
  - params: 
  - return: 
- `Trail.traffic_level_average` 
  - description: describes the amount of traffic at a trail over time 
  - method_type: 
  - params: 
  - return: 
- `Trail.traffic_over_day(day)` 
  - description: returns an array of traffic levels at every hour of the day (index:0=> 1:00am, index:2 => 2:00am)
  - method_type: 
  - params: 
  - return: 
- `Trail.type` 
  - description: defines what activities are at that trail instance 
  - method_type: 
  - params: 
  - return: 
- `Trail.length` 
  - description: defines how long the trail is in miles/kilometers 
  - method_type: 
  - params: 
  - return: 
- `Trail.shade_level` 
  - description: defines the relative amount of shade on a scale. 
- `Trail.pets_allowed` 
  - description: returns the types of pets allowed (`nil` if no pets allowed)
  - returns: Array[Pets]
### Methods 
--- 
## User (Lisa)
### Attributes (characteristics)
- `Class.username`
  - description: the users chosen name 
  - attribute_type:
- `Class.first_name`
  - description: the given name of a user
  - attribute_type:  
### Methods (verb)
- `Class.method`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
### Data Source 
  - where is the information coming from 
---- 
## Hike (Jason)
### Attributes (characteristics)
- `Hike.Name`
  - description: the short name used to describe a hike
  - attribute_type: string 
- `Hike.Trails` 
  - description: attribute of trails comprised in the hike (i.e. [blue_trail,red_trail, etc.])
  - attribute_type: Array<Trail>
- `Hike.Location` 
  - description: the starting point of the trail 
  - attribute_type: Location
- `Hike.shade_level` 
  - description: Averages shade rating for all `Trails` as part of the hike 
  - attribute_type: number 
- `Hike.pets_allowed`
  - description: defines what pets (if any) are permitted on **all** trails of the hike 
  - attribute_type: Array<string>
### Methods (verb)
- FUTURE - `Class.similar`
  - description: finds other hikes that are similar to the one provided 
  - method_type: instance
  - params: nil 
  - return: Array<Hike>   
### Data Source 
  - where is the information coming from 

  
---- 

 
-----
--> Down the line (v2)
---- 
## Mountain 
Represent a physical mountain 
### Attribtes (property)
- `Mountain.name` 
  - method_type: `instance`
- `Mountain.location` 
  - description: returns location 
  - method_type: `instance` 
  - return: `Location` 
- `Mountain.all`
  - description: returns all mountain records
  - method_type: `class` (self.all)
  - return: [Mountains]

### Methods (verb)
- `Mountain.findClosest()` 
  - class: `Mountain` 
  - description: finds the nearest mountain related to the object called upon
  - method_type: `instance` 
  - params: `nil`
  - return: `Array[Mountains]
### Data Source 
---- 
## Conditions 
---- 
## Equipment 
---- 
## Parking 
### Attributes
- `Parking.spots_available` 
### Methods (verb)
- `Class.attribute`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
---- 



> Template 
---- 
## Object_Name 
### Attributes (characteristics)
- `Class.attribute`
  - description: 
  - method_type:  
### Methods (verb)
- `Class.attribute`
  - description:" 
  - method_type: [instance/class] 
  - params: [name:string, age:integer]
  - return: name 
### Data Source 
  - where is the information coming from 
--- 



