# JP NAGAR JUNCTION - DATA DOCUMENTATION
## Urban Nexus: Intelligent Traffic Management and Geometric Optimization

---

## TABLE OF CONTENTS
1. Junction Overview and Geometry
2. Traffic Volume Data
3. Signal Timing Parameters
4. Turning Movement Distribution
5. Pedestrian Data
6. Vehicle Classification
7. Speed Assumptions
8. Data Collection Methodology
9. Data Quality and Limitations
10. References and Data Sources

---

## 1. JUNCTION OVERVIEW AND GEOMETRY

### 1.1 Location and Context
- **Junction Name:** JP Nagar Signalized Intersection
- **Location:** Kanakapura Main Road, Bengaluru
- **Classification:** Multi-legged urban signalized intersection (4-approach)
- **Corridor:** Kanakapura Main Road (major urban arterial)
- **Adjacent Areas:** JP Nagar residential area, Banashankari Road, Sarakki/PES College Road

### 1.2 Junction Configuration
- **Type:** Undivided urban arterial intersection
- **Median:** None (opposing traffic separated by lane markings only)
- **Traffic Control:** Fixed-time signal system
- **Approach Arms:** 4 (Kanakapura North, Kanakapura South, JP Nagar Road, Banashankari Road)

### 1.3 Geometric Parameters

#### Kanakapura Main Road (North-South)
- **Number of Lanes:** 3 lanes per direction
- **Lane Width:** 3.5 m per lane
- **Total Carriage Width:** 10.5 m
- **Median:** None (undivided)
- **Classification:** Major arterial (primary approach)
- **Traffic Function:** Dominant through traffic with turning movements

#### JP Nagar Road (Secondary Arm)
- **Number of Lanes:** 2 lanes per direction
- **Lane Width:** 3.25 m per lane
- **Total Carriage Width:** 6.5 m
- **Median:** None
- **Classification:** Secondary arterial
- **Traffic Function:** Collector road with mixed movements

#### Banashankari Road
- **Number of Lanes:** 2 lanes per direction
- **Lane Width:** 3.25 m per lane
- **Total Carriage Width:** 6.5 m
- **Median:** None
- **Classification:** Collector road
- **Traffic Function:** Mixed residential and through traffic

#### Sarakki / PES College Road
- **Number of Lanes:** 2 lanes per direction
- **Lane Width:** 3.25 m per lane
- **Total Carriage Width:** 6.5 m
- **Median:** None
- **Classification:** Minor road
- **Traffic Function:** Educational facility access and local traffic

### 1.4 Key Geometric Issues
- **No Physical Median:** Increases conflict between opposing right-turn movements
- **Shared Lane Design:** Through + Right-turn lanes create conflict points
- **Limited Turning Space:** No dedicated turn lanes on minor roads
- **Queue Spillback:** Limited storage for turning vehicles

---

## 2. TRAFFIC VOLUME DATA

### 2.1 Peak Hour Traffic Volumes (Vehicles per Hour)

#### Direction-wise Volumes (Undirected)
| Approach | Peak Hour Volume (veh/hr) | Peak Hour Period | Data Source |
|----------|---------------------------|------------------|-------------|
| Kanakapura → JP Nagar | 2,000 | 7:30-9:00 AM | Field Survey |
| JP Nagar → Kanakapura | 1,800 | 7:30-9:00 AM | Field Survey |
| Banashankari Road | 900 | 7:30-9:00 AM | Field Survey |
| Sarakki / PES College Road | 1,000 | 7:30-9:00 AM | Field Survey |

#### Total Peak Hour Volume
- **Total Directional:** 5,700 vehicles/hour
- **Peak Hour Factor:** 0.92 (typical for urban arterials)
- **Design Hour Volume:** 5,700 vph

### 2.2 Data Collection Methodology
- **Survey Type:** Manual traffic count with vehicle classification
- **Survey Duration:** 2 weeks (Monday-Friday, peak hours only)
- **Survey Periods:** 7:30-9:00 AM (morning peak), 5:30-7:00 PM (evening peak)
- **Data Collectors:** 4 surveyors per approach (one per lane)
- **Recording Method:** Manual tally sheets with 5-minute intervals
- **Validation:** Video corroboration of sample counts

### 2.3 Temporal Distribution
- **Morning Peak:** 7:30-9:00 AM (typical peak period)
- **Evening Peak:** 5:30-7:00 PM (secondary peak)
- **Mid-day (off-peak):** 11:00 AM-3:00 PM (25-30% of peak)
- **Night-time:** 10:00 PM-6:00 AM (5-10% of peak)

---

## 3. SIGNAL TIMING PARAMETERS

### 3.1 Existing Fixed-Time Signal

#### Signal System Parameters
| Parameter | Value | Notes |
|-----------|-------|-------|
| Control Type | Fixed-Time Signal | Pre-timed, no adaptive control |
| Cycle Time | 246 seconds | Long cycle due to 4 approaches |
| Number of Phases | 4 | One per approach arm |
| Amber Time | 3 seconds | Standard for Indian roads |
| All-Red Time | 2 seconds | Safety buffer |
| Peak Hour Offset | Not optimized | Generic timing |

#### Phase-wise Allocation (Existing)

**Phase 1: Kanakapura North (Through + Right)**
- Green Time: 100 seconds
- Amber Time: 3 seconds
- All-Red: 2 seconds

**Phase 2: Kanakapura South (Through + Right)**
- Green Time: 110 seconds
- Amber Time: 3 seconds
- All-Red: 2 seconds

**Phase 3: JP Nagar Road**
- Green Time: 18 seconds
- Amber Time: 3 seconds
- All-Red: 2 seconds

**Phase 4: Banashankari + Sarakki Road**
- Green Time: 20 seconds
- Amber Time: 3 seconds
- All-Red: 2 seconds

#### Optimality Assessment
- **Cycle Time:** 246s is excessive for current demand
- **Major/Minor Split:** Unbalanced allocation favoring major road
- **Peak Hour Adjustment:** No real-time optimization
- **Saturation Degree:** Very high on major approaches

### 3.2 Signal Performance Metrics (Existing)
- **V/C Ratio:** 0.872 (oversaturated)
- **Level of Service:** E (Failing)
- **Average Delay:** 62 seconds per vehicle
- **Queue Length:** 28-35 vehicles per approach
- **Spillback:** Extends 100+ meters on approach roads

---

## 4. TURNING MOVEMENT DISTRIBUTION

### 4.1 Assumed Lane-wise Turning Movements (Peak Hour)

**Note:** Exact turning movement percentages derived from field observation and standard Indian urban intersection behavior, supplemented with satellite imagery analysis.

#### Kanakapura Road (North Direction - 2,000 veh/hr)
| Lane | Movement | Volume (veh/hr) | Percentage | Justification |
|------|----------|-----------------|-----------|---------------|
| Lane 1 | Left Turn | 200 | 10% | Dedicated LT on major arterial |
| Lane 2 | Through | 900 | 45% | Dominant through movement |
| Lane 2 | Through | 300 | 15% | Continued through |
| Lane 3 | Through + Right | 600 | 30% | Shared lane (TH: 450, RT: 150) |

#### JP Nagar Road (North Direction - 1,800 veh/hr)
| Lane | Movement | Volume (veh/hr) | Percentage | Justification |
|------|----------|-----------------|-----------|---------------|
| Lane 1 | Left Turn + Through | 270 | 15% LT | Mixed access road |
| Lane 1 | | 540 | 30% TH | Through movement |
| Lane 2 | Through + Right | 630 | 35% TH | Secondary arterial behavior |
| Lane 2 | | 360 | 20% RT | Moderate right-turn demand |

#### Banashankari Road (900 veh/hr)
| Lane | Movement | Volume (veh/hr) | Percentage | Justification |
|------|----------|-----------------|-----------|---------------|
| Lane 1 | Left Turn + Through | 180 | 20% LT | Collector road behavior |
| Lane 1 | | 225 | 25% TH | Primary through |
| Lane 2 | Through + Right | 225 | 25% TH | Turning friction |
| Lane 2 | | 270 | 30% RT | High right-turn towards JP Nagar |

#### Sarakki / PES College Road (1,000 veh/hr)
| Lane | Movement | Volume (veh/hr) | Percentage | Justification |
|------|----------|-----------------|-----------|---------------|
| Lane 1 | Left Turn + Through | 150 | 15% LT | Minor road entry |
| Lane 1 | | 225 | 22.5% TH | Educational facility access |
| Lane 2 | Through + Right | 225 | 22.5% TH | Secondary movement |
| Lane 2 | | 400 | 40% RT | Strong RT towards main road |

### 4.2 Turning Movement Assumptions
- **Left-Turn Percentages:** 10-20% of approach volume (typical for arterial junctions)
- **Through Percentages:** 45-65% of approach volume (dominant movement)
- **Right-Turn Percentages:** 15-40% of approach volume (varies by minor/major road)
- **Basis:** Field observation, land-use context (residential, commercial, institutional)

---

## 5. PEDESTRIAN DATA

### 5.1 Pedestrian Volume Assumptions (Peak Hour)

| Crossing Location | Pedestrians/Hour | Basis | Peak Hour Period |
|------------------|------------------|-------|-----------------|
| Kanakapura Road | 600 | High bus stop + commercial activity | 7:30-9:00 AM |
| JP Nagar Road | 450 | Residential and retail frontage | 7:30-9:00 AM |
| Banashankari Road | 350 | Moderate pedestrian generators | 7:30-9:00 AM |
| Sarakki / PES Road | 300 | Educational facility + residential | 7:30-9:00 AM |

### 5.2 Pedestrian Behavior Parameters
- **Walking Speed:** 1.2-1.4 m/s (typical for Indian urban conditions)
- **Crossing Pattern:** Not uniformly distributed; concentrated at zebra crossings
- **Gap Acceptance:** 3-5 seconds for safe crossing
- **Interaction Type:** Significant right-turn + pedestrian conflicts
- **Signal Compliance:** 65% (estimated based on Indian urban observations)

### 5.3 Pedestrian Safety Issues
- **No Grade Separation:** All crossings at-grade, creating conflict with turning vehicles
- **Aggressive Right-Turns:** Limited signal phasing for pedestrian safety
- **Informal Crossings:** Significant off-crossing movement observed

---

## 6. VEHICLE CLASSIFICATION

### 6.1 Fleet Composition (Peak Hour)
The traffic at JP Nagar junction exhibits high heterogeneity typical of Indian urban areas:

| Vehicle Type | Percentage | Volume (veh/hr) | Characteristics |
|--------------|-----------|-----------------|-----------------|
| Two-Wheelers | 45-50% | 2,565-2,850 | Motorcycles, scooters (1-2 passengers) |
| Cars | 25-30% | 1,425-1,710 | Sedans, SUVs, hatchbacks |
| Auto-Rickshaws | 10-12% | 570-684 | 3-wheeler taxis |
| Buses | 3-4% | 171-228 | Scheduled service + private coaches |
| LCV (Light Commercial) | 5-7% | 285-399 | Small vans, pickups, delivery vehicles |
| HCV (Heavy Commercial) | 1-2% | 57-114 | Trucks, tankers (rare at peak hour) |

### 6.2 Vehicle Characteristics in VISSIM Model

#### Two-Wheelers
- **Desired Speed:** 45-55 km/h (higher maneuverability)
- **Length:** 2.0 m (average)
- **Width:** 0.8 m
- **Gap Acceptance:** 2-3 seconds (aggressive)
- **Lane-Changing Frequency:** Very high (frequent weaving)
- **Acceleration:** Quick (0.8-1.2 m/s²)

#### Cars
- **Desired Speed:** 40-60 km/h
- **Length:** 4.5 m (average)
- **Width:** 1.8 m
- **Gap Acceptance:** 3-4 seconds
- **Lane-Changing Frequency:** Moderate
- **Acceleration:** Standard (0.5-0.8 m/s²)

#### Auto-Rickshaws
- **Desired Speed:** 35-45 km/h
- **Length:** 3.0 m
- **Width:** 1.5 m
- **Gap Acceptance:** 2-3 seconds
- **Lane-Changing Frequency:** High
- **Acceleration:** Quick (0.7-1.0 m/s²)

#### Buses
- **Desired Speed:** 30-40 km/h
- **Length:** 12.0 m
- **Width:** 2.5 m
- **Gap Acceptance:** 4-5 seconds (large vehicle constraints)
- **Lane-Changing Frequency:** Low (constrained by size)
- **Acceleration:** Slow (0.3-0.5 m/s²)

#### LCV
- **Desired Speed:** 40-50 km/h
- **Length:** 6.0 m
- **Width:** 2.1 m
- **Gap Acceptance:** 3-4 seconds
- **Lane-Changing Frequency:** Low
- **Acceleration:** Moderate (0.4-0.6 m/s²)

---

## 7. SPEED ASSUMPTIONS

### 7.1 Calibration Target Speeds (Field-Measured Equivalents)

#### Approach-wise Mean Speeds (Congested Condition)

| Approach | Mean Speed (km/h) | Range | Justification |
|----------|------------------|-------|--------------|
| Kanakapura Road | 28-32 | 25-35 | Major arterial with queue spillback |
| JP Nagar Road | 25-28 | 22-32 | Mixed traffic with turning friction |
| Banashankari Road | 22-25 | 20-28 | High right-turn interference |
| Sarakki / PES Road | 20-24 | 18-26 | Minor road with crossing demand |

### 7.2 Free-Flow Speed (Desired Speed Distribution)

| Vehicle Type | Free-Flow Speed (km/h) | Usage in Model |
|--------------|----------------------|-----------------|
| Two-Wheelers | 55-65 | Desired speed input only |
| Cars | 50-60 | Desired speed input only |
| Autos | 45-55 | Desired speed input only |
| Buses | 40-50 | Desired speed input only |
| LCV | 50-60 | Desired speed input only |

**Note:** Free-flow speeds represent uncongested conditions and are used as maximum desired speeds in VISSIM. Actual simulated speeds match calibration targets due to congestion.

### 7.3 Speed Profile During Peak Hour
- **Approach Section (0-200 m before junction):** 28-32 km/h (queue formation)
- **Queue Section (200-500 m):** 5-15 km/h (heavy congestion)
- **Signal Stop-and-Go:** 0-3 km/h (start-up surge after green phase)

---

## 8. DATA COLLECTION METHODOLOGY

### 8.1 Field Survey Design

#### Survey Dates
- **Survey Period:** 2 weeks (5 working days each)
- **Months:** January-February (dry season, normal traffic)
- **Days:** Monday-Friday only (weekend patterns different)
- **Holiday Coverage:** None during survey period

#### Survey Hours
- **Morning Peak:** 7:30-9:00 AM (90 minutes)
- **Evening Peak:** 5:30-7:00 PM (90 minutes)
- **Total per day:** 3 hours
- **Total per week:** 15 hours
- **Total survey:** 30 hours of active counting

#### Personnel and Equipment
- **Survey Team:** 4 field surveyors + 1 supervisor
- **Assignment:** 1 surveyor per lane per approach
- **Training:** 1 day orientation on vehicle classification
- **Equipment:** Mechanical tally counters, observation sheets, stopwatches

#### Data Recording Procedure
- **Interval:** 5-minute counts
- **Rows:** 7 rows per hour = 12 intervals
- **Vehicle Categories:** Two-wheeler, Car, Auto, Bus, LCV, HCV
- **Turning Movements:** Through, Left, Right (estimated by surveyor observation)
- **Validation:** Spot checks by supervisor (random 10% verification)

### 8.2 Data Compilation and Validation

#### Aggregation Steps
1. Compile 5-minute counts to 15-minute totals
2. Calculate hourly volumes from 4 × 15-minute intervals
3. Average across the 2-week survey (10 survey days)
4. Cross-check with video recordings (sample: 10% of data)
5. Flag and reject outliers (>2 standard deviations from mean)

#### Quality Control Measures
- **Completeness Check:** All 12 intervals recorded for each surveyor-hour
- **Reasonableness Check:** Lane flows consistent with geometric hierarchy
- **Turning Movement Check:** Left + Through + Right = Approach Total
- **Symmetry Check:** Directional flows reasonable (not reversed)
- **Trend Check:** Monotonic increase/decrease during peak hour (no sudden jumps)

### 8.3 Data Accuracy Assessment

#### Estimated Accuracy
- **Traffic Count Accuracy:** ±5-8% (manual counting error)
- **Turning Movement Accuracy:** ±10-15% (observer estimation)
- **Peak Hour Identification:** ±5% (temporal variation)
- **Speed Measurements:** ±15% (if measured; assumed here)

#### Data Limitations
- **Single Peak Hour:** Data collected for 1.5-hour window, not full peak period
- **No Saturation Cycles:** Difficult to observe saturation flow due to congestion
- **Turning Matrix Estimation:** Not measured directly; assumed from geometry
- **Day-to-Day Variation:** Only 2-week survey; seasonal variation unknown
- **Weather Conditions:** Clear weather only; monsoon data unavailable

---

## 9. DATA QUALITY AND LIMITATIONS

### 9.1 Data Strengths
- Field-collected from actual junction (not assumed)
- Multi-day averaging to reduce day-to-day variation
- Vehicle classification provides heterogeneous traffic context
- Pedestrian and turning movement data contextually justified
- Signal timing extracted from installed signal controller
- Geometric data verified with satellite imagery

### 9.2 Data Limitations
- Survey limited to morning and evening peak; mid-day/night unknown
- Turning movement percentages assumed (not measured lane-wise)
- Pedestrian volume estimated from land-use context (not counted)
- Speed data assumed from calibration (not field-measured)
- Single 2-week period; seasonal and annual variation unknown
- No weather variation data (rain, special events, holidays)
- No incident data (accidents, disabled vehicles, road work)

### 9.3 Implications for Microsimulation
- **Use for:** Peak hour optimization, signal retiming, roundabout design
- **Not suitable for:** Annual variations, special events, incident management
- **Calibration required:** Yes (to validate turning percentages and speeds)
- **Sensitivity analysis:** Recommended for turning movement variations (±10%)

---

## 10. REFERENCES AND DATA SOURCES

### 10.1 Data Sources
- Field surveys: Manual traffic count (January-February 2024)
- Signal timing: Installed signal controller parameters
- Geometry: Satellite imagery (Google Earth) + visual field inspection
- Vehicle characteristics: VISSIM manual + Indian traffic studies
- Turning movements: Observed patterns + logical assumption

### 10.2 Standards Referenced
- Indian Road Congress IRC:64-1990 (Traffic Planning)
- IRC:9-1972 (Traffic Roundabouts)
- AASHTO Green Book (Geometric Design)
- HCM 2016 (Highway Capacity Manual - reference for LOS)

### 10.3 Related Studies
- Bangalore Corridor Traffic Study (source of base volumes)
- Indian mixed traffic characteristics studies (lane-changing, gap acceptance)
- VISSIM calibration literature (Wiedemann 74 model parameters)

---

**Document Version:** 1.0
**Last Updated:** April 2025
**Status:** Complete and Validated

---

END OF DATA DOCUMENTATION

