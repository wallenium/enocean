# Supported profiles
All profiles (should) correspond to the official [EEP](http://www.enocean-alliance.org/eep/) by EnOcean.

### RPS Telegram (0xF6)
##### RORG 0xF6 - FUNC 0x01 - TYPE 0x01 - Push Button

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PB      |Status of the push button                         |enum    |0 - Released                                                          |
|        |                                                  |        |1 - Pressed                                                           |



##### RORG 0xF6 - FUNC 0x02 - TYPE 0x01 - Light and Blind Control - Application Style 1

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|R1      |Rocker 1st action                                 |enum    |0 - Button AI                                                         |
|        |                                                  |        |1 - Button AO                                                         |
|        |                                                  |        |2 - Button BI                                                         |
|        |                                                  |        |3 - Button BO                                                         |
|EB      |Energy bow                                        |enum    |0 - released                                                          |
|        |                                                  |        |1 - pressed                                                           |
|R2      |Rocker 2nd action                                 |enum    |0 - Button AI                                                         |
|        |                                                  |        |1 - Button AO                                                         |
|        |                                                  |        |2 - Button BI                                                         |
|        |                                                  |        |3 - Button BO                                                         |
|SA      |2nd action                                        |enum    |0 - No 2nd action                                                     |
|        |                                                  |        |1 - 2nd action valid                                                  |
|T21     |T21                                               |status  |                                                                      |
|NU      |NU                                                |status  |                                                                      |


##### RORG 0xF6 - FUNC 0x02 - TYPE 0x02 - Light and Blind Control - Application Style 2

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|R1      |Rocker 1st action                                 |enum    |0 - Button AI                                                         |
|        |                                                  |        |1 - Button AO                                                         |
|        |                                                  |        |2 - Button BI                                                         |
|        |                                                  |        |3 - Button BO                                                         |
|EB      |Energy bow                                        |enum    |0 - released                                                          |
|        |                                                  |        |1 - pressed                                                           |
|R2      |Rocker 2nd action                                 |enum    |0 - Button AI                                                         |
|        |                                                  |        |1 - Button AO                                                         |
|        |                                                  |        |2 - Button BI                                                         |
|        |                                                  |        |3 - Button BO                                                         |
|SA      |2nd action                                        |enum    |0 - No 2nd action                                                     |
|        |                                                  |        |1 - 2nd action valid                                                  |
|T21     |T21                                               |status  |                                                                      |
|NU      |NU                                                |status  |                                                                      |



##### RORG 0xF6 - FUNC 0x05 - TYPE 0x01 - Liquid Leakage Sensor (mechanic harvester)

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|WAS     |Water Sensor                                      |enum    |0-16 - not specified                                                  |
|        |                                                  |        |17 - Water detected                                                   |
|        |                                                  |        |18-255 - not specified                                                |
|T21     |T21                                               |status  |                                                                      |
|NU      |NU                                                |status  |                                                                      |


##### RORG 0xF6 - FUNC 0x05 - TYPE 0x02 - Smoke Detector

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SMO     |Status of detection and battery                   |enum    |0 - Smoke Alarm OFF                                                   |
|        |                                                  |        |16 - Smoke Alarm ON                                                   |
|        |                                                  |        |48 - Energy LOW                                                       |



##### RORG 0xF6 - FUNC 0x10 - TYPE 0x00 - Window Handle

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|WIN     |Window handle                                     |enum    |0 - Moved from up to vertical                                         |
|        |                                                  |        |1 - Moved from vertical to up                                         |
|        |                                                  |        |2 - Moved from down to vertical                                       |
|        |                                                  |        |3 - Moved from vertical to down                                       |
|T21     |T21                                               |status  |                                                                      |
|NU      |NU                                                |status  |                                                                      |



### 1BS Telegram (0xD5)
##### RORG 0xD5 - FUNC 0x00 - TYPE 0x01 - Single Input Contact

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CO      |Contact                                           |enum    |0 - open                                                              |
|        |                                                  |        |1 - closed                                                            |



### 4BS Telegram (0xA5)
##### RORG 0xA5 - FUNC 0x02 - TYPE 0x01 - Temperature Sensor Range -40°C to 0°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -40.0-0.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x02 - Temperature Sensor Range -30°C to +10°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -30.0-10.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x03 - Temperature Sensor Range -20°C to +20°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -20.0-20.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x04 - Temperature Sensor Range -10°C to +30°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -10.0-30.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x05 - Temperature Sensor Range 0°C to +40°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-40.0 °C                                               |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x06 - Temperature Sensor Range +10°C to +50°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 10.0-50.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x07 - Temperature Sensor Range +20°C to +60°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 20.0-60.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x08 - Temperature Sensor Range +30°C to +70°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 30.0-70.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x09 - Temperature Sensor Range +40°C to +80°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 40.0-80.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x0A - Temperature Sensor Range +50°C to +90°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 50.0-90.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x0B - Temperature Sensor Range +60°C to +100°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 60.0-100.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x10 - Temperature Sensor Range -60°C to +20°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -60.0-20.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x11 - Temperature Sensor Range -50°C to +30°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -50.0-30.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x12 - Temperature Sensor Range -40°C to +40°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -40.0-40.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x13 - Temperature Sensor Range -30°C to +50°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -30.0-50.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x14 - Temperature Sensor Range -20°C to +60°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -20.0-60.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x15 - Temperature Sensor Range -10°C to +70°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ -10.0-70.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x16 - Temperature Sensor Range 0°C to +80°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-80.0 °C                                               |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x17 - Temperature Sensor Range +10°C to +90°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 10.0-90.0 °C                                              |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x18 - Temperature Sensor Range +20°C to +100°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 20.0-100.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x19 - Temperature Sensor Range +30°C to +110°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 30.0-110.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x1A - Temperature Sensor Range +40°C to +120°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 40.0-120.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x1B - Temperature Sensor Range +50°C to +130°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 50.0-130.0 °C                                             |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x20 - 10 Bit Temperature Sensor Range -10°C to +41.2°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |1023.0-0.0 ↔ -10.0-41.2 °C                                            |


##### RORG 0xA5 - FUNC 0x02 - TYPE 0x30 - 10 Bit Temperature Sensor Range -40°C to +62.3°C

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |1023.0-0.0 ↔ -40.0-62.3 °C                                            |



##### RORG 0xA5 - FUNC 0x04 - TYPE 0x01 - Range 0°C to +40°C and 0% to 100%

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-250.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-250.0 ↔ 0.0-40.0 °C                                               |
|TSN     |Availability of the Temperature Sensor            |enum    |0 - not available                                                     |
|        |                                                  |        |1 - available                                                         |


##### RORG 0xA5 - FUNC 0x04 - TYPE 0x02 - Range -20°C to +60°C and 0% to 100%

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-250.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-250.0 ↔ -20.0-60.0 °C                                             |
|TSN     |Availability of the Temperature Sensor            |enum    |0 - not available                                                     |
|        |                                                  |        |1 - available                                                         |


##### RORG 0xA5 - FUNC 0x04 - TYPE 0x03 - Range -20°C to +60°C 10bit-measurement and 0% to 100%

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-255.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-1023.0 ↔ -20.0-60.0 °C                                            |
|TTP     |Telegram Type                                     |enum    |0 - Heartbeat                                                         |
|        |                                                  |        |1 - Event triggered                                                   |


##### RORG 0xA5 - FUNC 0x04 - TYPE 0x04 - Range -40°C to +120°C 12bit-measurement and 0% to 100%

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-199.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-1599.0 ↔ -40.0-120.0 °C                                           |



##### RORG 0xA5 - FUNC 0x06 - TYPE 0x01 - Range 300lx to 60.000lx

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (linear)                           |value   |0.0-255.0 ↔ 0.0-5.1 V                                                 |
|ILL2    |Illumination 2 (linear)                           |value   |0.0-255.0 ↔ 300.0-30000.0 lx                                          |
|ILL1    |Illumination 1 (linear)                           |value   |0.0-255.0 ↔ 600.0-60000.0 lx                                          |
|RS      |Range select                                      |enum    |0 - Range acc. to DB_1 (ILL1)                                         |
|        |                                                  |        |1 - Range acc. to DB_2 (ILL2)                                         |


##### RORG 0xA5 - FUNC 0x06 - TYPE 0x02 - Range 0lx to 1.020lx

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (linear)                           |value   |0.0-255.0 ↔ 0.0-5.1 V                                                 |
|ILL2    |Illumination 2 (linear)                           |value   |0.0-255.0 ↔ 0.0-510.0 lx                                              |
|ILL1    |Illumination 1 (linear)                           |value   |0.0-255.0 ↔ 0.0-1020.0 lx                                             |
|RS      |Range select                                      |enum    |0 - Range acc. to DB_1 (ILL1)                                         |
|        |                                                  |        |1 - Range acc. to DB_2 (ILL2)                                         |



##### RORG 0xA5 - FUNC 0x07 - TYPE 0x01 - Occupancy with Supply voltage monitor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (OPTIONAL)                         |value   |0.0-250.0 ↔ 0.0-5.0 V                                                 |
|PIRS    |PIR Status                                        |enum    |0 - PIR off                                                           |
|        |                                                  |        |1 - PIR on                                                            |
|SVA     |Supply voltage availability                       |enum    |0 - Supply voltage is not supported                                   |
|        |                                                  |        |1 - Supply voltage is supported                                       |


##### RORG 0xA5 - FUNC 0x07 - TYPE 0x02 - Occupancy with Supply voltage monitor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (REQUIRED)                         |value   |0.0-250.0 ↔ 0.0-5.0 V                                                 |
|PIRS    |PIR Status                                        |enum    |0 - Uncertain of occupancy status                                     |
|        |                                                  |        |1 - Motion detected                                                   |


##### RORG 0xA5 - FUNC 0x07 - TYPE 0x03 - Occupancy with Supply voltage monitor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (REQUIRED)                         |value   |0.0-250.0 ↔ 0.0-5.0 V                                                 |
|ILL     |Illumination                                      |value   |0.0-1000.0 ↔ 0.0-1000.0 lx                                            |
|PIRS    |PIR Status                                        |enum    |0 - Uncertain of occupancy status                                     |
|        |                                                  |        |1 - Motion detected                                                   |



##### RORG 0xA5 - FUNC 0x08 - TYPE 0x01 - Range 0lx to 510lx, 0°C to +51°C and Occupancy Button

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage (linear)                           |value   |0.0-255.0 ↔ 0.0-5.1 V                                                 |
|ILL     |Illumination (linear)                             |value   |0.0-255.0 ↔ 0.0-510.0 lx                                              |
|TMP     |Temperature (linear)                              |value   |0.0-255.0 ↔ 0.0-51.0 °C                                               |
|PIRS    |PIR Status                                        |enum    |0 - PIR on                                                            |
|        |                                                  |        |1 - PIR off                                                           |
|OCC     |Occupancy Button                                  |enum    |0 - Button pressed                                                    |
|        |                                                  |        |1 - Button released                                                   |



##### RORG 0xA5 - FUNC 0x09 - TYPE 0x04 - CO2 Sensor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-200.0 ↔ 0.0-100.0 %                                               |
|Conc    |Concentration (linear)                            |value   |0.0-255.0 ↔ 0.0-2550.0 ppm                                            |
|TMP     |Temperature (linear)                              |value   |0.0-255.0 ↔ 0.0-51.0 °C                                               |


##### RORG 0xA5 - FUNC 0x09 - TYPE 0x05 - VOC Sensor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|Conc    |VOC Concentration                                 |value   |0.0-65535.0 ↔ 0.0-65535.0 ppb                                         |
|VOC_ID  |VOC Identification                                |enum    |0 - VOCT (total)                                                      |
|        |                                                  |        |1 - Formaldehyde                                                      |
|        |                                                  |        |2 - Benzene                                                           |
|        |                                                  |        |3 - Styrene                                                           |
|        |                                                  |        |4 - Toluene                                                           |
|        |                                                  |        |5 - Tetrachloroethylene                                               |
|        |                                                  |        |6 - Xylene                                                            |
|        |                                                  |        |7 - n-Hexane                                                          |
|        |                                                  |        |8 - n-Octane                                                          |
|        |                                                  |        |9 - Cyclopentane                                                      |
|        |                                                  |        |10 - Methanol                                                         |
|        |                                                  |        |11 - Ethanol                                                          |
|        |                                                  |        |12 - 1-Pentanol                                                       |
|        |                                                  |        |13 - Acetone                                                          |
|        |                                                  |        |14 - ethylene Oxide                                                   |
|        |                                                  |        |15 - Acetaldehyde ue                                                  |
|        |                                                  |        |16 - Acetic Acid                                                      |
|        |                                                  |        |17 - Propionice Acid                                                  |
|        |                                                  |        |18 - ValericAcid                                                      |
|        |                                                  |        |19 - ButyricAcid                                                      |
|        |                                                  |        |20 - Ammoniac                                                         |
|        |                                                  |        |22 - Hydrogen Sulfide                                                 |
|        |                                                  |        |23 - Dimethylsulfide                                                  |
|        |                                                  |        |24 - 2-Butanol (butyl Alcohol)                                        |
|        |                                                  |        |25 - 2-Methylpropanol                                                 |
|        |                                                  |        |26 - Diethyl ether                                                    |
|        |                                                  |        |255 - ozone                                                           |



##### RORG 0xA5 - FUNC 0x10 - TYPE 0x03 - Temperature Sensor and Set Point

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Set Point (linear)                                |value   |0.0-255.0 ↔ 0.0-255.0 %                                               |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-40.0 °C                                               |


##### RORG 0xA5 - FUNC 0x10 - TYPE 0x05 - Temperature Sensor, Set Point and Occupancy Control

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Set Point (linear)                                |value   |0.0-255.0 ↔ 0.0-255.0 %                                               |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-40.0 °C                                               |
|OCC     |Occupancy Button                                  |enum    |0 - Button pressed                                                    |
|        |                                                  |        |1 - Button released                                                   |


##### RORG 0xA5 - FUNC 0x10 - TYPE 0x06 - Temperature Sensor, Set Point and Day/Night Control

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Set Point (linear)                                |value   |0.0-255.0 ↔ 0.0-255.0 %                                               |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-40.0 °C                                               |
|SLSW    |Slide switch                                      |enum    |0 - Position I / Night / Off                                          |
|        |                                                  |        |1 - Position O / Day / On                                             |


##### RORG 0xA5 - FUNC 0x10 - TYPE 0x10 - Temperature and Humidity Sensor, Set Point and Occupancy Control

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Set Point (linear)                                |value   |0.0-255.0 ↔ 0.0-255.0                                                 |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-250.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-250.0 ↔ 0.0-40.0 °C                                               |
|OCC     |Occupancy Button                                  |enum    |0 - Button pressed                                                    |
|        |                                                  |        |1 - Button released                                                   |


##### RORG 0xA5 - FUNC 0x10 - TYPE 0x12 - Temperature and Humidity Sensor and Set Point

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Set Point (linear)                                |value   |0.0-255.0 ↔ 0.0-255.0                                                 |
|HUM     |Rel. Humidity (linear)                            |value   |0.0-250.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature (linear)                              |value   |0.0-250.0 ↔ 0.0-40.0 °C                                               |



##### RORG 0xA5 - FUNC 0x11 - TYPE 0x02 - Temperature Controller Output

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CVAR    |Actual value of controller                        |value   |0.0-255.0 ↔ 0.0-100.0 %                                               |
|FAN     |Actual value of fan                               |enum    |0 - State 0 Manual                                                    |
|        |                                                  |        |1 - State 1 Manual                                                    |
|        |                                                  |        |2 - State 2 Manual                                                    |
|        |                                                  |        |3 - State 3 Manual                                                    |
|        |                                                  |        |16 - State 0 Automatic                                                |
|        |                                                  |        |17 - State 1 Automatic                                                |
|        |                                                  |        |18 - State 2 Automatic                                                |
|        |                                                  |        |19 - State 3 Automatic                                                |
|        |                                                  |        |255 - Not Available                                                   |
|ASP     |Actual Setpoint                                   |value   |0.0-255.0 ↔ 0.0-51.2 C                                                |
|ALR     |Alarm                                             |enum    |0 - No alarm                                                          |
|        |                                                  |        |1 - Alarm                                                             |
|CTM     |Controller mode                                   |enum    |1 - Heating                                                           |
|        |                                                  |        |2 - Cooling                                                           |
|        |                                                  |        |3 - Off                                                               |
|CTS     |Controller state                                  |enum    |0 - Automatic                                                         |
|        |                                                  |        |1 - Override                                                          |
|ERH     |Energy hold-off                                   |enum    |0 - Normal                                                            |
|        |                                                  |        |1 - Energy hold-off / Dew point                                       |
|RO      |Room occupancy                                    |enum    |0 - Occupied                                                          |
|        |                                                  |        |1 - Unoccupied                                                        |
|        |                                                  |        |2 - StandBy                                                           |
|        |                                                  |        |3 - Frost                                                             |


##### RORG 0xA5 - FUNC 0x11 - TYPE 0x03 - Blind Status

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|BSP     |Blind/shutter position                            |value   |0.0-100.0 ↔ 0.0-100.0 %                                               |
|AS      |Angle sign                                        |enum    |0 - Positive sign                                                     |
|        |                                                  |        |1 - Negative sign                                                     |
|AN      |Angle in 2 degrees steps                          |value   |0.0-90.0 ↔ 0.0-180.0 degrees                                          |
|PVF     |Position value flag                               |enum    |0 - No position value available                                       |
|        |                                                  |        |1 - Position value available                                          |
|AVF     |Angle value flag                                  |enum    |0 - No Angle value available                                          |
|        |                                                  |        |1 - Angle value available                                             |
|ES      |Error state                                       |enum    |0 - No error present                                                  |
|        |                                                  |        |1 - End-positions are not configured                                  |
|        |                                                  |        |2 - Internal failure                                                  |
|        |                                                  |        |3 - Not used                                                          |
|EP      |End position                                      |enum    |0 - No End-position available                                         |
|        |                                                  |        |1 - No End-position reached                                           |
|        |                                                  |        |2 - Blind fully open                                                  |
|        |                                                  |        |3 - Blind fully closed                                                |
|ST      |Status                                            |enum    |0 - No status available                                               |
|        |                                                  |        |1 - Blind is stopped                                                  |
|        |                                                  |        |2 - Blind opens                                                       |
|        |                                                  |        |3 - Blind closes                                                      |
|SM      |Service mode                                      |enum    |0 - Normal mode                                                       |
|        |                                                  |        |1 - Service mode activated                                            |
|MOTP    |Mode of the position                              |enum    |0 - Normal mode                                                       |
|        |                                                  |        |1 - Inverse ode                                                       |



##### RORG 0xA5 - FUNC 0x12 - TYPE 0x00 - Counter

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|MR      |Current value in or cumulative counter value      |value   |0.0-16777215.0 ↔ 0.0-16777215.0                                       |
|CH      |Measurement channel                               |value   |0.0-15.0 ↔ 0.0-15.0                                                   |
|DT      |Current value or cumulative counter value         |enum    |0 - Cumulative value                                                  |
|        |                                                  |        |1 - Current value                                                     |
|DIV     |Divisor for value                                 |enum    |0 - x/1                                                               |
|        |                                                  |        |1 - x/10                                                              |
|        |                                                  |        |2 - x/100                                                             |
|        |                                                  |        |3 - x/1000                                                            |


##### RORG 0xA5 - FUNC 0x12 - TYPE 0x01 - Electricity

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|MR      |current value in W or cumulative value in kWh     |value   |0.0-16777215.0 ↔ 0.0-16777215.0                                       |
|TI      |Tariff info                                       |value   |0.0-15.0 ↔ 0.0-15.0                                                   |
|DT      |Current value or cumulative value                 |enum    |0 - kWh                                                               |
|        |                                                  |        |1 - W                                                                 |
|DIV     |Divisor for value                                 |enum    |0 - x/1                                                               |
|        |                                                  |        |1 - x/10                                                              |
|        |                                                  |        |2 - x/100                                                             |
|        |                                                  |        |3 - x/1000                                                            |



##### RORG 0xA5 - FUNC 0x13 - TYPE 0x01 - Weather Station

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|DWS     |Dawn sensor                                       |value   |0.0-255.0 ↔ 0.0-999.0 lx                                              |
|TMP     |Temperature                                       |value   |0.0-255.0 ↔ -40.0-80.0 °C                                             |
|WND     |Wind speed                                        |value   |0.0-255.0 ↔ 0.0-70.0 m/s                                              |
|ID      |Identifier                                        |enum    |0-15 - Identifier {value}                                             |
|DN      |Day / Night                                       |enum    |0 - Day                                                               |
|        |                                                  |        |1 - Night                                                             |
|RAN     |Rain Indication                                   |enum    |0 - No Rain                                                           |
|        |                                                  |        |1 - Rain                                                              |



##### RORG 0xA5 - FUNC 0x14 - TYPE 0x01 - Single Input Contact (Window/Door), Supply voltage monitor

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SVC     |Supply voltage / super cap. (linear); 251 - 255 reserved for error code|value   |0.0-250.0 ↔ 0.0-5.0 V                                                 |
|CT      |Contact                                           |enum    |1 - open                                                              |
|        |                                                  |        |0 - closed                                                            |



##### RORG 0xA5 - FUNC 0x20 - TYPE 0x01 - Battery Powered Actuator (BI-DIR)

###### direction: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CV      |Current Value                                     |value   |0.0-100.0 ↔ 0.0-100.0 %                                               |
|SO      |Service On                                        |enum    |0 - off                                                               |
|        |                                                  |        |1 - on                                                                |
|ENIE    |Energy input enabled                              |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|ES      |Energy storage sufficiently charged               |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|BCAP    |Battery capacity; change battery next days        |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|CCO     |Contact, cover open                               |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|FTS     |Failure Temperature sensor, out of range          |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|DWO     |Detection, window open                            |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|ACO     |Actuator obstructed                               |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|TMP     |Temperature (linear)                              |value   |0.0-255.0 ↔ 0.0-40.0 °C                                               |

###### direction: 2
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|SP      |Valve Position or Temperature Setpoint            |value   |0.0-100.0 ↔ 0.0-100.0 %                                               |
|TMP     |Temperature from RCU                              |value   |0.0-255.0 ↔ 0.0-40.0 °C                                               |
|RIN     |Run init sequence                                 |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|LFS     |Lift set                                          |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|VO      |Valve open / maintenance                          |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|VC      |Valve closed                                      |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|SB      |Summer bit, Reduction of energy consumption       |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|SPS     |Set point selection                               |enum    |0 - Valve position                                                    |
|        |                                                  |        |1 - Temperature set point                                             |
|SPN     |Set point inverse                                 |enum    |0 - false                                                             |
|        |                                                  |        |1 - true                                                              |
|RCU     |Select function                                   |enum    |0 - RCU                                                               |
|        |                                                  |        |1 - service on                                                        |



##### RORG 0xA5 - FUNC 0x30 - TYPE 0x03 - Digital Inputs, Wake and Temperature

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|TMP     |Temperature (linear)                              |value   |255.0-0.0 ↔ 0.0-40.0 °C                                               |
|WA0     |Value of wake signal                              |enum    |0 - Low                                                               |
|        |                                                  |        |1 - High                                                              |
|DI3     |Digital Input 3                                   |enum    |0 - Low                                                               |
|        |                                                  |        |1 - High                                                              |
|DI2     |Digital Input 2                                   |enum    |0 - Low                                                               |
|        |                                                  |        |1 - High                                                              |
|DI1     |Digital Input 1                                   |enum    |0 - Low                                                               |
|        |                                                  |        |1 - High                                                              |
|DI0     |Digital Input 0                                   |enum    |0 - Low                                                               |
|        |                                                  |        |1 - High                                                              |



##### RORG 0xA5 - FUNC 0x38 - TYPE 0x08 - Gateway

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|COM     |Command ID                                        |enum    |0-13 - Command ID {value}                                             |
|TIM     |Time in 1/10 seconds. 0 = no time specifed        |value   |1.0-65535.0 ↔ 0.1-6553.5 s                                            |
|LCK     |Lock for duration time if time >0, unlimited time of no time specified. Locking may be cleared with "unlock". During lock phase no other commands will be accepted or executed|enum    |0 - Unlock                                                            |
|        |                                                  |        |1 - Lock                                                              |
|DEL     |Delay or duration (if Time > 0); 0 = Duration (Execute switching command immediately and switch back after duration) 1 = Delay (Execute switching command after delay)|enum    |0 - Duration                                                          |
|        |                                                  |        |1 - Delay                                                             |
|SW      |Switching command ON/OFF                          |enum    |0 - Off                                                               |
|        |                                                  |        |1 - On                                                                |

###### command: 2
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|COM     |Command ID                                        |enum    |0-13 - Command ID {value}                                             |
|EDIM    |Dimming value (absolute [0...255] or relative [0...100])|value   |0.0-255.0 ↔ 0.0-255.0 %                                               |
|RMP     |Ramping time in seconds, 0 = no ramping, 1...255 = seconds to 100%|value   |0.0-255.0 ↔ 0.0-255.0 s                                               |
|EDIMR   |Dimming Range                                     |enum    |0 - Absolute value                                                    |
|        |                                                  |        |1 - Relative value                                                    |
|STR     |Store final value                                 |enum    |0 - No                                                                |
|        |                                                  |        |1 - Yes                                                               |
|SW      |Switching command                                 |enum    |0 - Off                                                               |
|        |                                                  |        |1 - On                                                                |



### VLD Telegram (0xD2)
##### RORG 0xD2 - FUNC 0x01 - TYPE 0x01 - Electronic switch with Local Control

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PF      |Power Failure                                     |enum    |0 - Power Failure Detection disabled/not supported                    |
|        |                                                  |        |1 - Power Failure Detection enabled                                   |
|PFD     |Power Failure Detection                           |enum    |0 - Power Failure Detection not detected/not supported/disabled       |
|        |                                                  |        |1 - Power Failure Detection Detected                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|OC      |Over current switch off                           |enum    |0 - Over current switch off: ready / not supported                    |
|        |                                                  |        |1 - Over current switch off: executed                                 |
|EL      |Error level                                       |enum    |0 - Error level 0: hardware OK                                        |
|        |                                                  |        |1 - Error level 1: hardware warning                                   |
|        |                                                  |        |2 - Error level 2: hardware failure                                   |
|        |                                                  |        |3 - Error level not supported                                         |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|LC      |Local control                                     |enum    |0 - Local control disabled / not supported                            |
|        |                                                  |        |1 - Local control enabled                                             |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|DV      |Dim value                                         |enum    |0 - Switch to new output value                                        |
|        |                                                  |        |1 - Dim to new output level - dim timer 1                             |
|        |                                                  |        |2 - Dim to new output level - dim timer 2                             |
|        |                                                  |        |3 - Dim to new output level - dim timer 3                             |
|        |                                                  |        |4 - Stop dimming                                                      |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |


##### RORG 0xD2 - FUNC 0x01 - TYPE 0x0B - Smart Plug module with Energy Measurement

###### command: 6
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|qu      |Query                                             |enum    |0 - Query energy                                                      |
|        |                                                  |        |1 - Query power                                                       |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 7
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|UN      |Unit                                              |enum    |0 - Energy [Ws]                                                       |
|        |                                                  |        |1 - Energy [Wh]                                                       |
|        |                                                  |        |2 - Energy [KWh]                                                      |
|        |                                                  |        |3 - Power [W]                                                         |
|        |                                                  |        |4 - Power [KW]                                                        |
|        |                                                  |        |5-7 - Not used                                                        |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|MV      |Measurement value                                 |enum    |0-4294967295 - Measurement value {value}                              |

###### command: 3
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PF      |Power Failure                                     |enum    |0 - Power Failure Detection disabled/not supported                    |
|        |                                                  |        |1 - Power Failure Detection enabled                                   |
|PFD     |Power Failure Detection                           |enum    |0 - Power Failure Detection not detected/not supported/disabled       |
|        |                                                  |        |1 - Power Failure Detection Detected                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|OC      |Over current switch off                           |enum    |0 - Over current switch off: ready / not supported                    |
|        |                                                  |        |1 - Over current switch off: executed                                 |
|EL      |Error level                                       |enum    |0 - Error level 0: hardware OK                                        |
|        |                                                  |        |1 - Error level 1: hardware warning                                   |
|        |                                                  |        |2 - Error level 2: hardware failure                                   |
|        |                                                  |        |3 - Error level not supported                                         |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|LC      |Local control                                     |enum    |0 - Local control disabled / not supported                            |
|        |                                                  |        |1 - Local control enabled                                             |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|DV      |Dim value                                         |enum    |0 - Switch to new output value                                        |
|        |                                                  |        |1 - Dim to new output level - dim timer 1                             |
|        |                                                  |        |2 - Dim to new output level - dim timer 2                             |
|        |                                                  |        |3 - Dim to new output level - dim timer 3                             |
|        |                                                  |        |4 - Stop dimming                                                      |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 5
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|RM      |Report measurement                                |enum    |0 - Query only                                                        |
|        |                                                  |        |1 - Query / auto                                                      |
|RE      |Reset measurement                                 |enum    |0 - Not active                                                        |
|        |                                                  |        |1 - Trigger signal                                                    |
|ep      |Measurement mode                                  |enum    |0 - Energy                                                            |
|        |                                                  |        |1 - Power                                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|MD_LSB  |Measurement delta LSB                             |enum    |0-15 - Measurement delta LSB {value}                                  |
|UN      |Unit                                              |enum    |0 - Energy [Ws]                                                       |
|        |                                                  |        |1 - Energy [Wh]                                                       |
|        |                                                  |        |2 - Energy [KWh]                                                      |
|        |                                                  |        |3 - Power [W]                                                         |
|        |                                                  |        |4 - Power [KW]                                                        |
|        |                                                  |        |5-7 - Not used                                                        |
|MD_MSB  |Measurement delta MSB                             |enum    |0-255 - Measurement delta MSB {value}                                 |
|MAT     |Max message time                                  |enum    |0 - Reserved                                                          |
|        |                                                  |        |1-255 - Max message time {value}                                      |
|MIT     |Min message time                                  |enum    |0 - Reserved                                                          |
|        |                                                  |        |1-255 - Min message time {value}                                      |


##### RORG 0xD2 - FUNC 0x01 - TYPE 0x0C - Heating module with Pilotwire command and Energy Measurement

###### command: 8
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|PM      |Pilotwire mode                                    |enum    |0 - Off                                                               |
|        |                                                  |        |1 - Comfort                                                           |
|        |                                                  |        |2 - Eco                                                               |
|        |                                                  |        |3 - Anti-freeze                                                       |
|        |                                                  |        |4 - Comfort-1                                                         |
|        |                                                  |        |5 - Comfort-2                                                         |

###### command: 10
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|PM      |Pilotwire mode                                    |enum    |0 - Off                                                               |
|        |                                                  |        |1 - Comfort                                                           |
|        |                                                  |        |2 - Eco                                                               |
|        |                                                  |        |3 - Anti-freeze                                                       |
|        |                                                  |        |4 - Comfort-1                                                         |
|        |                                                  |        |5 - Comfort-2                                                         |

###### command: 9
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |

###### command: 6
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|qu      |Query                                             |enum    |0 - Query energy                                                      |
|        |                                                  |        |1 - Query power                                                       |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 7
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|UN      |Unit                                              |enum    |0 - Energy [Ws]                                                       |
|        |                                                  |        |1 - Energy [Wh]                                                       |
|        |                                                  |        |2 - Energy [KWh]                                                      |
|        |                                                  |        |3 - Power [W]                                                         |
|        |                                                  |        |4 - Power [KW]                                                        |
|        |                                                  |        |5-7 - Not used                                                        |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|MV      |Measurement value                                 |enum    |0-4294967295 - Measurement value {value}                              |

###### command: 3
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PF      |Power Failure                                     |enum    |0 - Power Failure Detection disabled/not supported                    |
|        |                                                  |        |1 - Power Failure Detection enabled                                   |
|PFD     |Power Failure Detection                           |enum    |0 - Power Failure Detection not detected/not supported/disabled       |
|        |                                                  |        |1 - Power Failure Detection Detected                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|OC      |Over current switch off                           |enum    |0 - Over current switch off: ready / not supported                    |
|        |                                                  |        |1 - Over current switch off: executed                                 |
|EL      |Error level                                       |enum    |0 - Error level 0: hardware OK                                        |
|        |                                                  |        |1 - Error level 1: hardware warning                                   |
|        |                                                  |        |2 - Error level 2: hardware failure                                   |
|        |                                                  |        |3 - Error level not supported                                         |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|LC      |Local control                                     |enum    |0 - Local control disabled / not supported                            |
|        |                                                  |        |1 - Local control enabled                                             |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|DV      |Dim value                                         |enum    |0 - Switch to new output value                                        |
|        |                                                  |        |1 - Dim to new output level - dim timer 1                             |
|        |                                                  |        |2 - Dim to new output level - dim timer 2                             |
|        |                                                  |        |3 - Dim to new output level - dim timer 3                             |
|        |                                                  |        |4 - Stop dimming                                                      |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 5
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|RM      |Report measurement                                |enum    |0 - Query only                                                        |
|        |                                                  |        |1 - Query / auto                                                      |
|RE      |Reset measurement                                 |enum    |0 - Not active                                                        |
|        |                                                  |        |1 - Trigger signal                                                    |
|ep      |Measurement mode                                  |enum    |0 - Energy                                                            |
|        |                                                  |        |1 - Power                                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|MD_LSB  |Measurement delta LSB                             |enum    |0-15 - Measurement delta LSB {value}                                  |
|UN      |Unit                                              |enum    |0 - Energy [Ws]                                                       |
|        |                                                  |        |1 - Energy [Wh]                                                       |
|        |                                                  |        |2 - Energy [KWh]                                                      |
|        |                                                  |        |3 - Power [W]                                                         |
|        |                                                  |        |4 - Power [KW]                                                        |
|        |                                                  |        |5-7 - Not used                                                        |
|MD_MSB  |Measurement delta MSB                             |enum    |0-255 - Measurement delta MSB {value}                                 |
|MAT     |Max message time                                  |enum    |0 - Reserved                                                          |
|        |                                                  |        |1-255 - Max message time {value}                                      |
|MIT     |Min message time                                  |enum    |0 - Reserved                                                          |
|        |                                                  |        |1-255 - Min message time {value}                                      |


##### RORG 0xD2 - FUNC 0x01 - TYPE 0x0F - Slot-in Module with 1 channel and no metering capabilities

###### command: 3
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PF      |Power Failure                                     |enum    |0 - Power Failure Detection disabled/not supported                    |
|        |                                                  |        |1 - Power Failure Detection enabled                                   |
|PFD     |Power Failure Detection                           |enum    |0 - Power Failure Detection not detected/not supported/disabled       |
|        |                                                  |        |1 - Power Failure Detection Detected                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|OC      |Over current switch off                           |enum    |0 - Over current switch off: ready / not supported                    |
|        |                                                  |        |1 - Over current switch off: executed                                 |
|EL      |Error level                                       |enum    |0 - Error level 0: hardware OK                                        |
|        |                                                  |        |1 - Error level 1: hardware warning                                   |
|        |                                                  |        |2 - Error level 2: hardware failure                                   |
|        |                                                  |        |3 - Error level not supported                                         |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|LC      |Local control                                     |enum    |0 - Local control disabled / not supported                            |
|        |                                                  |        |1 - Local control enabled                                             |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|DV      |Dim value                                         |enum    |0 - Switch to new output value                                        |
|        |                                                  |        |1 - Dim to new output level - dim timer 1                             |
|        |                                                  |        |2 - Dim to new output level - dim timer 2                             |
|        |                                                  |        |3 - Dim to new output level - dim timer 3                             |
|        |                                                  |        |4 - Stop dimming                                                      |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |


##### RORG 0xD2 - FUNC 0x01 - TYPE 0x12 - Slot-in Module with 2 channels and no metering capabilities

###### command: 3
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|PF      |Power Failure                                     |enum    |0 - Power Failure Detection disabled/not supported                    |
|        |                                                  |        |1 - Power Failure Detection enabled                                   |
|PFD     |Power Failure Detection                           |enum    |0 - Power Failure Detection not detected/not supported/disabled       |
|        |                                                  |        |1 - Power Failure Detection Detected                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|OC      |Over current switch off                           |enum    |0 - Over current switch off: ready / not supported                    |
|        |                                                  |        |1 - Over current switch off: executed                                 |
|EL      |Error level                                       |enum    |0 - Error level 0: hardware OK                                        |
|        |                                                  |        |1 - Error level 1: hardware warning                                   |
|        |                                                  |        |2 - Error level 2: hardware failure                                   |
|        |                                                  |        |3 - Error level not supported                                         |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - Not applicable, do not use                                       |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|LC      |Local control                                     |enum    |0 - Local control disabled / not supported                            |
|        |                                                  |        |1 - Local control enabled                                             |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CMD     |Command identifier                                |enum    |0-13 - Command ID {value}                                             |
|DV      |Dim value                                         |enum    |0 - Switch to new output value                                        |
|        |                                                  |        |1 - Dim to new output level - dim timer 1                             |
|        |                                                  |        |2 - Dim to new output level - dim timer 2                             |
|        |                                                  |        |3 - Dim to new output level - dim timer 3                             |
|        |                                                  |        |4 - Stop dimming                                                      |
|IO      |I/O channel                                       |enum    |0-29 - Output channel {value} (to load)                               |
|        |                                                  |        |30 - All output channels supported by the device                      |
|        |                                                  |        |31 - Input channel (from mains supply)                                |
|OV      |Output value                                      |enum    |0 - Output value 0% or OFF                                            |
|        |                                                  |        |1-100 - Output value {value}% or ON                                   |
|        |                                                  |        |101-126 - Not used                                                    |
|        |                                                  |        |127 - output value not valid / not set                                |



##### RORG 0xD2 - FUNC 0x03 - TYPE 0x0A - Push Button – Single Button

|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|BATT    |Battery Autonomy                                  |value   |1.0-100.0 ↔ 1.0-100.0 %                                               |
|BA      |Button Action                                     |enum    |0 - Reserved                                                          |
|        |                                                  |        |1 - Simple press                                                      |
|        |                                                  |        |2 - Double press                                                      |
|        |                                                  |        |3 - Long press                                                        |
|        |                                                  |        |4 - Long press released                                               |
|        |                                                  |        |5-255 - Reserved                                                      |



##### RORG 0xD2 - FUNC 0x05 - TYPE 0x00 - Type 0x00

###### command: 1
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|POS     |Vertical position                                 |enum    |0-100 - Output position {value}%                                      |
|        |                                                  |        |127 - Do not change                                                   |
|ANG     |Rotation angle                                    |enum    |0-100 - Output angle {value}%                                         |
|        |                                                  |        |127 - Do not change                                                   |
|REPO    |Repositioning                                     |enum    |0 - Go directly to POS/ANG                                            |
|        |                                                  |        |1 - Go up (0%), then to POS/ANG                                       |
|        |                                                  |        |2 - Go down (100%), then to POS/ANG                                   |
|        |                                                  |        |3 - Reserved                                                          |
|LOCK    |Locking modes                                     |enum    |0 - Do not change                                                     |
|        |                                                  |        |1 - Set blockage mode                                                 |
|        |                                                  |        |2 - Set alarm mode                                                    |
|        |                                                  |        |3 - Reserved                                                          |
|        |                                                  |        |4 - Reserved                                                          |
|        |                                                  |        |5 - Reserved                                                          |
|        |                                                  |        |6 - Reserved                                                          |
|        |                                                  |        |7 - Deblockage                                                        |
|CHN     |Channel                                           |enum    |0 - Channel 1                                                         |
|CMD     |Command Id                                        |enum    |0-5 - Command ID {value}                                              |

###### command: 2
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CHN     |Channel                                           |enum    |0 - Channel 1                                                         |
|CMD     |Command Id                                        |enum    |0-5 - Command ID {value}                                              |

###### command: 3
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|CHN     |Channel                                           |enum    |0 - Channel 1                                                         |
|CMD     |Command Id                                        |enum    |0-5 - Command ID {value}                                              |

###### command: 4
|shortcut|description                                       |type    |values                                                                |
|--------|--------------------------------------------------|--------|----                                                                  |
|POS     |Current vertical position                         |enum    |0-100 - Output position {value}%                                      |
|        |                                                  |        |127 - Position unknown, will be known after the next goto cmd         |
|ANG     |Current rotation angle                            |enum    |0-100 - Output angle {value}%                                         |
|        |                                                  |        |127 - Angle unknown, will be known after the next goto cmd            |
|LOCK    |Current locking mode                              |enum    |0 - Normal (no lock)                                                  |
|        |                                                  |        |1 - Blockage mode                                                     |
|        |                                                  |        |2 - Alarm mode                                                        |
|        |                                                  |        |3 - Reserved                                                          |
|        |                                                  |        |4 - Reserved                                                          |
|        |                                                  |        |5 - Reserved                                                          |
|        |                                                  |        |6 - Reserved                                                          |
|        |                                                  |        |7 - Reserved                                                          |
|CHN     |Channel                                           |enum    |0 - Channel 1                                                         |
|        |                                                  |        |1 - Channel 2                                                         |
|        |                                                  |        |2 - Channel 3                                                         |
|        |                                                  |        |3 - Channel 4                                                         |
|CMD     |Command Id                                        |enum    |0-5 - Command ID {value}                                              |



