# Synthetic-Data-Generation
For Telemedicine Research and Test Proposed Storage Architechture
Creates synthetic telemedicine consultation data for database testing. Generates 9 CSV tables with referential integrity: patients, doctors, healthcare facilities, consultations, tests, time slots, and geographic locations.

**Features:** Realistic Bangladeshi names, phone numbers, medical specializations, geographic coordinates

## Quick Start
```bash
pip install pandas numpy
python generate_data.py
```

## Generated Tables
- `fact_telemedicine.csv` - 1,000 consultation records
- `dim_patient.csv` - 500 patients
- `dim_doctor.csv` - 150 healthcare providers
- `dim_healthcare.csv` - 80 facilities
- `dim_consultation.csv` - 300 consultation types
- `dim_test.csv` - 200 diagnostic tests
- `dim_time.csv` - 70,176 time slots
- `dim_specialization.csv` - 15 medical specialties
- `LOCATION_RANGPUR.csv` - 58 geographic locations

## Schema
Star schema design with `FACT_TELEMEDICINE` as central table linked to 8 dimension tables via foreign keys.

**Total Records:** 72,479
