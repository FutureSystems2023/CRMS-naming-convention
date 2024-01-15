# CRMS SQL Naming Convention
This is a guide on the naming convention for Competition Results Management System (CRMS)

<br/>

### Overall Case formatting:
<table>
    <thead>
        <tr>
            <th>Fields</th>
            <th>Case
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Database names</td>
            <td>Lower case</td>
        </tr>
        <tr>
            <td>Table names</td>
            <td>Pascal case + snake case</td>
        </tr>
        <tr>
            <td>Column names</td>
            <td>Lower case + snake case</td>
        </tr>
        <tr>
            <td>Keys and Indexes</td>
            <td>Prefix = uppercase</td>
        </tr>
    </tbody>
</table>

<br/>

### Definition of Case formatting:

Refer to the picture below to understand the different case formatting.

![case formatting definition](camel-case-snake-case-pascal-case.png "Case Formatting Definition")

<hr>

## Database
Database names will be **lowercase** (no numbers or special characters like "-/+=", only "_" underscores are allowed).

<hr>

## Tables
Table names will be in **lowercase** and **singular**. E.g. athlete, team, sport, etc. If table name has multiple words, concatenate them with an underscore "_". E.g. "Competition Geo Location"  --> competition_geo_location.

Naming convention will follow "Parent-Child" relationship. E.g. Athlete results will be named as athlete_result instead of result_athlete

### Many to Many Tables
For many to many tables, table names will be concatenated with 2 underscores '**__**'. E.g. competition__competition_category.

<hr>

## Columns
Column names will be **singular** and **lowercase** except for prefixes and suffixes. <u>All prefixes and suffixes</u> should be in **lowercase**. Column names with more than one word will be joined using underscores '**_**'

### Primary Key Column
Primary Keys will be prefixed with '**pk_**'

### Foreign Key Column
Foreign Keys will be prefixed with '**fk_**'

<hr>

## Constraints Naming

Constraints naming will be in the following format: {tablename}_{columnname(s)}_{suffix} (for primary key just {tablename}_{suffix} will suffice)

### Primary Keys
Primary Keys will be suffixed with '**_pkey**'

### Foreign Keys
Foreign Keys will be suffixed with '**_fkey**'

### Indexes
Indexes will be suffixed with '**_idx**'

### Unique Key Constraints
Unique Key constraints will be suffixed with '**_key**'

### Exclusion Constraints
Exclusion constraints will be suffixed with '**_excl**'

### Check Constraints
Exclusion constraints will be suffixed with '**_check**'

<hr>

## Sequence
Sequence will be suffixed with '**_seq**'

<hr>

## Data Types Format

### Date
Date fields will be in the format "**<i>YYYY-MM-DD</i>**"

### DateTime
Date fields will be in the format "**<i>YYYY-MM-DD HH:MM:SS</i>**"

### Time
Time fields will be in the format "**<i>HH:MM:SS</i>**"
