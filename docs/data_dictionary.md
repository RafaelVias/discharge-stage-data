# Data Dictionary

This document provides detailed descriptions of the variables in the discharge-stage measurement datasets.

## Variables

- `meas_nu`: Measurement number/identifier
  - Type: Character string
  - Description: A unique identifier for each measurement. 
  - Note on enumeration:
    - Iceland and Sweden: Original measurement numbers as provided by the institutions
    - USA: Measurements enumerated from 1 to n for each station, ordered by stage height (W)

- `station_number`: Station identifier
  - Type: Character string
  - Description: A unique identifier for each gauging station
  - Format varies by country

- `station_name`: Station name
  - Type: Character string
  - Description: The name of the gauging station location

- `date`: Measurement date
  - Type: Date (YYYY-MM-DD)
  - Description: The date when the measurement was taken

- `W`: Stage/water level
  - Type: Numeric
  - Unit: meters (m)
  - Description: The height of the water surface relative to a local datum (reference point)

- `Q`: Discharge
  - Type: Numeric
  - Unit: cubic meters per second (m³/s)
  - Description: The volume of water flowing through the river cross-section per unit time

- `country`: Country of location
  - Type: Character string
  - Values: "iceland", "sweden", "usa"
  - Description: Country where the gauging station is located