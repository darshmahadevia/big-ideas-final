# The (412) Index


## Team Information
- Team Name: The Yinzer Index
- Team Members:
  - Darsh ([darsh_email@pitt.edu])
  - [Partner Name] ([partner_email@pitt.edu])
- Canvas Group Number: [Add Group Number Here]

## Project Overview
This project answers the question "What is the best neighborhood in Pittsburgh?" by combining nightlife, safety, and affordability into one score for young adults moving to the city.

## Our Metric: Young Adult Bestness Score
We combine 3 sub-metrics using weighted scoring:

- Nightlife (30%): More food facilities/restaurants = better
- Safety (40%): Fewer arrests = better
- Affordability (30%): Lower property values = better

Formula:

Bestness = (Nightlife x 0.30) + (Safety x 0.40) + (Affordability x 0.30)

All sub-metrics are min-max normalized to a 0 to 1 scale.
Safety and affordability are inverted so that lower raw values become higher scores.

## Datasets Used (WPRDC)
1. Allegheny County Restaurant/Food Facility Inspections
   - Resource used: Food Facility/Restaurant Locations CSV
   - Local file: food_facilities.csv
   - Link: https://data.wprdc.org/dataset/allegheny-county-restaurant-food-facility-inspection-violations

2. Pittsburgh Police Arrest Data (Archived)
   - Resource used: Arrests CSV
   - Local file: arrest_data.csv
   - Link: https://data.wprdc.org/dataset/arrest-data

3. Allegheny County Property Assessments
   - Resource used: Property Assessments Parcel Data (for downloads) CSV
   - Local file: property_assessments.csv
   - Link: https://data.wprdc.org/dataset/property-assessments

## Notebook Ownership
| Notebook | Team Member |
|---|---|
| nightlife_darsh.ipynb | Darsh |
| crime_darsh.ipynb | Darsh |
| cost_of_living_nick.ipynb | Nick Ocampo |
| final_report.ipynb | Group (Darsh + Nick Ocampo) |

## How to Run the Project
1. Put all CSV files and notebooks in the same folder.
2. Run nightlife_darsh.ipynb completely to generate nightlife_scores.csv.
3. Run crime_darsh.ipynb completely to generate safety_scores.csv.
4. Run cost_of_living_partner.ipynb completely to generate affordability_scores.csv.
5. Run final_report.ipynb to merge all scores and find the final winner.

## Output Files Generated
- nightlife_scores.csv
- safety_scores.csv
- affordability_scores.csv

These score files are used by final_report.ipynb to compute the final Young Adult Bestness Score ranking.
