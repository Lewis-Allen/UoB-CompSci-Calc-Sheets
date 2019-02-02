# University of Brighton - Degree Calc
Grade calculating spreadsheets. Find out your current grade to help you set aims to achieve the degree classification you want.

## Prerequisites 
Basic Excel knowledge will be required for any personalizations to be made.

These sheets are designed for third-year students in the year 2018/2019. This consisted of twenty credits of optional modules in the second year, and forty credits of optional modules in the third year. Placement Learning grades are not included in these spreadsheets because no-one seems to have concrete evidence on how this particular module contributes towards the degree mark. (Please let me know if you find some :-) ).

## Different Sheets and Optional Modules
The forty credits can be spread across two-to-four modules in the final year. Three spreadsheets have been provided for different module configurations. (One twenty credit module and two ten credit modules etc).

### List of sheets

| Spreadsheet Name            | Description                                                                    |
|-----------------------------|--------------------------------------------------------------------------------|
| Two Twenty Credit Optionals | 40 credits consisting of two twenty credit modules.                            |
| One Twenty Credit Optional  | 40 credits consisting of two twenty credit modules and two ten credit modules. |
| Four Ten Credit Optionals   | 40 credits consisting of four ten credit modules.                              |

## Personalizing 
There are two sheets in each spreadsheet, one for calculating grades by module mark, and one that allows you to specify marks at an assignment level. Some personalizations will likely be required when using the *by assignment* sheet.

These sheets by default assume each optional module has two assignments worth 50% each. This will unlikely be perfect for all cases and will need to be changed to suit any personal requirements.

### Removing an Assignment Row
In the case of a ten credit module only having a single assignment/exam worth the entire module, you would have to change:

| Module                        | Assignment/Exam | Percentage of Module | Potential Percent of Year | Mark | Percent Earned | Final Degree Contribution |
|-------------------------------|-----------------|----------------------|---------------------------|------|----------------|---------------------------|
| Optional 10 Credit Module Two | Assignment One  | 50.00%               | 4.17                      |      | 0.00           | 0.00                      |
|                               | Assignment Two  | 50.00%               | 4.17                      |      | 0.00           | 0.00                      |

into this:

| Module                        | Assignment/Exam | Percentage of Module | Potential Percent of Year | Mark | Percent Earned | Final Degree Contribution |
|-------------------------------|-----------------|----------------------|---------------------------|------|----------------|---------------------------|
| Optional 10 Credit Module Two | Assignment One  | 100.00%              | 4.17                      |      | 0.00           | 0.00                      |

A row has been deleted, percentage worth changed. The rest will auto calculate.

### Adding an Assignment Row
Adding an extra assignment row is slightly trickier. There are a couple of extra steps.

- Add a new assignment row. (Copy a current row)
- Modify the percentages based on what each assignment is worth. Total for the module should be 100%.
- Ensure the formula in the *Potential Percent of Year* column is pointing to the correct module in the modules grid to the side if you are using the *by Assignment* sheet.
- Ensure the final total is including your new assignment.

e.g.

| Module                        | Assignment/Exam | Percentage of Module | Potential Percent of Year | Mark | Percent Earned | Final Degree Contribution |
|-------------------------------|-----------------|----------------------|---------------------------|------|----------------|---------------------------|
| Optional 20 Credit Module Two | Assignment One  | 50.00%               | 8.33                      |      | 0.00           | 0.00                      |
|                               | Assignment Two  | 50.00%               | 8.33                      |      | 0.00           | 0.00                      |

becomes:

| Module                        | Assignment/Exam   | Percentage of Module | Potential Percent of Year | Mark | Percent Earned | Final Degree Contribution |
|-------------------------------|-------------------|----------------------|---------------------------|------|----------------|---------------------------|
| Optional 20 Credit Module Two | Assignment One    | 50.00%               | 8.33                      |      | 0.00           | 0.00                      |
|                               | Assignment Two    | 25.00%               | 4.17                      |      | 0.00           | 0.00                      |
|                               | Assignment Three  | 25.00%               | 4.17                      |      | 0.00           | 0.00                      |

## Future Work
- Automatic calculation of what average you need in the rest of your assignments to achieve a first/higher second. (You can work this out yourself by putting in dummy values into the other assignments and seeing what the total becomes).
- Using this as a base for a fully-fledged web application, making it easier for users to make their personalizations.