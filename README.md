# Floating target
Python script to calculate floating target

## Installation
This is using python 3.10.X\
pip install required libraries i.e "pip install -r requirements.txt"

## Settings
set the fy value to the financial year (int)\
set the curr_mon to the current month (int)\
Set the db settings at the top to correspond to the server settings in use

## Usage
Run python hfr_targets_facility_level.py\
The script will generate a Targets-Achieved.csv with floating targets\
When the curr_mon is 4 or below the calculation starts from month 1\
When the curr_mon is > 4 the reference month to reference the starting point for the floating targets will be existing data in DB hence will fail if no data.\

## Notes
Assumes all partners data up to month of reference is in the target table.\
Script for target table is provided in facility_floating_target.sql
