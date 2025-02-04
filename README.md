# Tableau_definitions
Definitions csv used to produce performance reports
We use the Tableau tabcmd tool to produce the performance reports automatically from the command promtp.
To produce the reports, type this into the command promtp:
      cd c:\temp
      tabcmd_sh24 -d -t {token_name} -p "{token_value}" definitions.csv

token_name and token_value are in 1Password.

That should start a progress bar in the command prompt.
Once each page is finished, type this, adapting the month to the end of the relevant reporting period:
      cd c:\temp
      merge_pdf_sh24 -o "Month 2023" merge_areas.txt

The last version of the definitions.csv and the merge_areas.txt should be stored in c:\temp for the process to work.
