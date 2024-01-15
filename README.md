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

### Many to Many Tables
For many to many tables, table names will be concatenated with 2 underscores '**__**'. E.g. competition_competitioncategory.

<hr>

## Columns
Column names will be **singular** and **lowercase** except for prefixes and suffixes. <u>All prefixes and suffixes</u> should be in **lowercase**. Column names with more than one word will be joined using underscores '**_**'

<hr>

## Keys and Indexes

### Primary Keys
Primary Keys will be prefixed with '**PK_**'

### Foreign Keys
Foreign Keys will be prefixed with '**FK_**'

### Indexes
Indexes will be prefixed with '**IDX_**'

### Unique Key Constraints
Unique Key constraints will be prefixed with '**UQ_**'

<hr>

## Data Types Format

### Date
Date fields will be in the format "**<i>YYYY-MM-DD</i>**"

### DateTime
Date fields will be in the format "**<i>YYYY-MM-DD HH:MM:SS</i>**"

### Time
Time fields will be in the format "**<i>HH:MM:SS</i>**"
