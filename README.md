# Custom Marlin Configuration Ender 3 Pro SKR Mini E3 2 + CR Touch + Sprite Extruder Pro
Este es un firmware personalizado de Marlin 2.1.2.1 para adaptar el Sprite Extruder Pro con CRTouch a la Ender 3 Pro.
## Upgrades Ender 3 Pro
* BIGTREETECH SKR Mini E3 V2.0 Motherboard
* BIGTREETEHCH TFT35 E3 V3.0.1
* Creality CR Touch
* Creality Sprite Extruder Pro
* Dual Z axis

#define EXTRUDE_MAXLENGTH 500
#define DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 400, 424.9 }
#define DEFAULT_MAX_FEEDRATE
#define DEFAULT_TRAVEL_ACCELERATION    500
#define USE_PROBE_FOR_Z_HOMING
#define Z_MIN_PROBE_PIN PC14
#define BLTOUCH
#define NOZZLE_TO_PROBE_OFFSET { -46.4, -60, -1.29 }
#define PROBING_MARGIN 10
#define XY_PROBE_FEEDRATE (150*60)
#define Z_PROBE_FEEDRATE_FAST (20*60)
#define Z_CLEARANCE_BETWEEN_PROBES  3 
#define Z_CLEARANCE_MULTI_PROBE     3 
#define Z_MIN_PROBE_REPEATABILITY_TEST
#define Z_HOMING_HEIGHT  20
#define X_BED_SIZE 225
#define Y_BED_SIZE 225 
#define Z_MAX_POS 200
//  #define MIN_SOFTWARE_ENDSTOP_Z //Custom Elboby - disabled 2024
#define SOFT_ENDSTOPS_MENU_ITEM  
#define AUTO_BED_LEVELING_BILINEAR
#define ENABLE_LEVELING_AFTER_G28
#define G26_MESH_VALIDATION
#define GRID_MAX_POINTS_X 5
#define ABL_BILINEAR_SUBDIVISION
#define Z_SAFE_HOMING
#define HOMING_FEEDRATE_MM_M { (150*60), (150*60), (10*60) }
#define NOZZLE_PARK_POINT { (X_MIN_POS + 10), (Y_MAX_POS - 10), 20 }
