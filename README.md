# CRMS SQL Naming Convention
This is a guide on the naming convention for Central Results Management System (CRMS)

<hr>

## Database
Database names will be **lowercase** (no numbers or special characters lie "_" or "-").

<hr>

## Tables
Table names will be in **PascalCasing** (camelCasing with the first letter also capitalized) and **singular**. E.g. AthleteTeam.

### Many to Many Tables
For many to many tables, table names will be concatenated with underscore '**_**'. E.g. Competition_CompetitionCategory.

<hr>

## Columns
Column names will be **singular** and **lowercase** except for prefixes and suffixes. <u>All prefixes and suffixes</u> should be in **uppercase**.

<hr>

## Keys and Indexes

### Primary Keys
Primary Keys will be prefixed with '**PK_**'

### Foreign Keys
Foreign Keys will be prefixed with '**FK_**'

### Indexes
Indexes will be prefixed with '**IDX_**'

<hr>

## Fields
Field Names with more than one word will be joined using underscores '**_**'

### Date fields
Date fields will be in the format "**<i>YYYY-MM-DD</i>**"

### DateTime fields
Date fields will be in the format "**<i>YYYY-MM-DD HH:MM:SS</i>**"