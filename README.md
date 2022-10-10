# Production-Schedule

This production schedule is one of the larger projects that I have taken on in my time as a data analyst. It took me seven workdays while assisting with other projects to gather data from the ERP system, cleaning the data into a usable and legible format, and create the final schedule.

The process to create this document was to:

1.	Sort SKUs into categories by which component parts they use
2.	Give each work cell a group of categories based on like production techniques
3.	Pull data from ERP database using SQL into an updatable sheet on the document for:
    a.	Quantity of component per SKU assembly
    b.	Number of manufacturing processes per component
        i.	Labor time per process
        ii.	Machines viable for each process

This document takes in the number of finished products that sales wants by category and turns that into manufacturing information for the company including labor times, calculated employees for production, and organizing it into a vertically aligned pattern of production schedule to support sales goals.

The data was imported into the document using SQL coding and was previously attached to the ERP system to have the data refreshable. All fields that did not directly pull from the ERP system were calculated off the data in the reports from the SQL queries.

The FAB Import Sheet manipulates the data on the FAB SCHEDULE sheet into a format that is ready for import using a dexterity macro into our ERP system for use in schedule creation as well as production documentation tools using uploaded information.

This document uses the following excel functions to calculate the schedule:
Filter
Unique
Index
Sum
MRound
Index(Match)
Roundup
Nested Filter statements
