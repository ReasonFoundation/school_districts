# School_districts


## Problem: 
NCES has a total of 13 thousand school districts. The current ACFRs database has more than 9 thousand. However, school districts in ACFRs database do not a common identifier with the NCES, making it hard to know how many and which ones are collected. 

## Solution: 
1. acfrs_filenam_govname_ncesid.Rmd
This file is in acfrs_datachecking project

This is the first stop dealing with acfrs school district data. Using regular expression to match as much as possible the names in ACFRs and in NCES. 

--> Output: final_match.csv

2. dictionary_name_ncesID_acfrsID.qmd: 

Construct a dictionary that links entity name, acfrs id, nces id

-->  Out put
dictionary12345.RDS

Dictionary12345 how has 9493 entities that ncesID, id (internal acfrs id),  students number.

# Fields of data

- Category

Type of Government:General Purpose (e.g. a state, county, city, town, village or borough), School District, Special District, Community College District or Public Higher Education

- Net Pension Liability

The liability of employers and nonemployer contributing entities to employees for benefits provided through a defined benefit pension plan.

- Net Pension Assets

The excess of net position in a pension system to the total pension liability. It should be measured as the portion of the actuarial present value of projected payments that is attributable to past periods of employee service, net of the pension plan’s fiduciary net position.

- Net OPEB Liability

The net OPEB liability is measured as the portion of the actuarial present value of projected benefit payments that is attributed to past periods of employee service, net of the OPEB plan's fiduciary net position.

- Net OPEB Assets

The net OPEB Asset is computed as the difference between the actuarial present value of projected benefit payments attributed to past periods of employee service and the OPEB plan’s fiduciary net position.

- Total Liabilities

Liabilities are present obligations to sacrifice resources that the government has little or no discretion to avoid. 

- Current Liabilities

Current liabilities are amount of obligations for items that have entered into the operating cycle incurred in the acquisition of materials and supplies to be used in providing services; collections received in advance of the performance of services.

- Current Portion of Long-Term Liabilities

Noncurrent liabilities, due within one year, which are present obligations to sacrifice resources that the government has little or no discretion to avoid.

- Compensated Abseces

Compensated absences payable, classified as noncurrent. Compensated absences are compensated time off such as vacation and sick leave, which has been earned by employees and probable that the employer will compensate the employees through paid time off or some other means, such as cash payments at termination or retirement but not yet compensated by the employer.

- Bonds Outstanding

Amount of debt payments related to the general obligation bonds that are due in current and future reporting periods.

- Loans Outstanding

Aggregate carrying value as of the balance sheet date of loans payable.(Unlike bonds, loans are made directly by another organization such a bank or other unit of government.)

- Notes Outstanding

Amount of all notes owed by the local unit. Debit upon payment of such notes; credit for the face amounts of long-term notes.

(The primary difference between notes payable and bonds stems from securities laws. Bonds are always considered and regulated as securities, while notes payable are not necessarily considered securities. )

- Leases

Represent lease contracts payable in more than one year that convey control of the right to use another entity's nonfinancial asset (the underlying asset) as specified in the contract for a period of time in exchange or exchange-like transaction.

- Revenues

The sum of program revenues and general revenues.

- Expenses

Expenses, which includes an entity's outflows or expiration of assets or the incurrence of liabilities during a period from providing or producing goods, rendering services, or carrying out other activities.

- Charges for Services

Program revenues that arise from charges to customers, applicants, or others who purchase, use, or directly benefit from the goods, services, or privileges provided, or are otherwise directly affected by the services.

- Operating Grants and Contributions

Program revenues from operating grants and contributions. Program revenues are amounts derived directly from the program itself or from parties outside the reporting government's taxpayers or citizenry, as a whole. Program revenues reduce the net cost of the function to be financed from the government's general revenues.

- Capital Grants and Contributions

Program revenues from capital grants and contributions. Program revenues are amounts derived directly from the program itself or from parties outside the reporting government's taxpayers or citizenry, as a whole. Program revenues reduce the net cost of the function to be financed from the government's general revenues.

- General Revenue

The sum of all general revenues, which include taxes, investment income and fines.

- Change in Net Position

Changes in net position which is the difference in net position between the beginning and end of the reporting period.

- Component Unit of

If the entity is a separately reporting component unit, which entity's ACFR shows its financial results as a component