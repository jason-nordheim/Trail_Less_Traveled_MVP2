
# [The Hiking Project](https://www.hikingproject.com)

* Trail
  * PROPERTIES  
    * overview[text] - brief overview of the trail 
    * description[text] - a description of the trail 
    * need_to_know[text] - any special details about the trail (seasonal rules, best months, etc.)
    * trail_type 
      * narrow_trail (single_track)
      * wide_trail (double track)
      * paved_path 
    * route_type 
      * loop 
      * out_and_back
      * point_to_point 
    * distance[float] (out and back, miles or kilometers)
    * difficulty[integer]
      * easy
      * intermediate
      * difficult 
      * very_difficult 
    * camping
      * camp_fires_allowed[bool] 
    * elevation 
      * ascent[integer] (feet)
      * descent[integer] (feet)
      * high_altitude[integer] (feet)
      * low_altitude[integer] (feet) 
    * grade 
      * average_grade (% and degree) 
      * max_grade (% and degree) 
    * dogs_allowed[bool]
    * rating[integer] (1-5)
  * METHODS  
    * get_weather() - gets the weather forecast for the next few days 
    * get_current_conditions() - gets the most recent report of trail conditions 
    * get_conditions() - gets all conditions 

```json
  "trails": [
    {
      "id": 7011192,
      "name": "Boulder Skyline Traverse",
      "type": "Hike",
      "summary": "The classic long mountain route in Boulder.",
      "difficulty": "black",
      "stars": 4.7,
      "starVotes": 78,
      "location": "Superior, Colorado",
      "url": "https://www.hikingproject.com/trail/7011192/boulder-skyline-traverse",
      "imgSqSmall": "https://cdn-files.apstatic.com/hike/7048859_sqsmall_1555540136.jpg",
      "imgSmall": "https://cdn-files.apstatic.com/hike/7048859_small_1555540136.jpg",
      "imgSmallMed": "https://cdn-files.apstatic.com/hike/7048859_smallMed_1555540136.jpg",
      "imgMedium": "https://cdn-files.apstatic.com/hike/7048859_medium_1555540136.jpg",
      "length": 16.3,
      "ascent": 5409,
      "descent": -5492,
      "high": 8492,
      "low": 5417,
      "longitude": -105.2582,
      "latitude": 39.9388,
      "conditionStatus": "Minor Issues",
      "conditionDetails": "Dry, Snowy, Mostly Dry, Some Mud, Icy - Spikes n poles helpful but not required",
      "conditionDate": "2020-03-17 17:21:19"
    },
```



* TrailIssue 
  * Proerties 
    * issue_severity[integer]
      * low 
      * medium 
      * high 
    * comment[text] - description of why the trail's conditions have degraded. 
  * Methods 

* Member 
  * PROPERTIES 
    * first_name[string]
    * last_name[string] 
    * local_city[string]
    * local_state[string]
    * created_at[timestamp] (member since...)
    * favorite_trails[array<Trail>] - favorite trails stored by user 
    * checkins[array<Trail>] - trails checked into 
    * email[string]
  * METHODS  
    * checkin(trail) - checks the user into the trail passed as a parameter, and marking the visit as the current date. 
    * favorite(trail) - marks the trail provided as a parameter as a favorite trail for that user. 


# [The Trail Run Project](https://www.trailrunproject.com)
