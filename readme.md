# Solver for Inventory Dynamics - integration into Digital Supply Chain Twin platforms

This exe was elaborated based on the modelling presented by Amanda G. Prosdocimi during her master thesis elaboration.

## Getting Started

Copy the main.exe and the 'spreadsheet' folder to a folder within your WIN machine

# Input File Structure
Input files should be positioned within:
/spreadsheet/input/
 
Modify the input xlsx files accordingly - they are located in /spreadsheet/input
!! Always preserve the name of columns and rows - do not change them!!
!! Do not change file names or sheet names !!

# Cost Coeficients 
set the cost coefficents in const_input.xlsx sheet - cost coefficients

# Arrhenius Constants
set the arrhenius equation constants in const_input.xlsx sheet - constants

# Initial Values 
set the initial value for single inventory in const_input.xlsx sheet - initial_values_single_inventory
set the initial value for multiple inventory in const_input.xlsx sheet - initial_values_mult_inventory

# Note!
The code will run single and mult inventories at the same. If input is left blank it will not run. Complete input even if you do not need an specific case. 

# Output File

Output file with calculations are placed in /spreadsheet/output/
file output_cost.xlsx has the costs calculations based on the benchmark (in this case the single inventory)
file output_inventory_levels - the results of the inventory dynamics and quality levels calculations

# Single Inventory Case
modify data.input.xlsx sheet - input_sheet_single_inventory applies to single inventory case
data.input.xlsx sheet - input_sheet_mult_inventory is ignored

# Multiple Inventory Case
data.input.xlsx sheet - input_sheet_single_inventory applies to inventory 1
data.input.xlsx sheet - input_sheet_mult_inventory applies to inventory 2

### Prerequisites

The executable should run without any specific dependencies - WIN only
