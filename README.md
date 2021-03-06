# Machine-Bias-Mitigation

HOME MORTGAGE DISCLOSURE ACT (HMDA)
README
Record Count (main table): 11,875,464 <br>
**Uploaded data is sampled data because the original one which I used for analysis is over 300MB. 
<br> Plus, it has some confidential issues to share the real data.**

The Home Mortgage Disclosure Act (HMDA) requires all banks, savings and loans, savings banks and credit unions with assets of more than $33 million and offices in metropolitan areas to report mortgage applications. This act was enacted by Congress in 1975 and is implemented by the Federal Reserve Board's Regulation C with the goal of:

*	Helping the public determine whether financial institutions are serving the housing needs of their communities;
*	Informing public officials in distributing public-sector investments so as to attract private investment to areas where it is needed;
*	Identifying possible discriminatory lending patterns.

This regulation applies to certain financial institutions, including banks, savings associations, credit unions, and other mortgage lending institutions. Banks, savings and loan associations, credit unions, and mortgage and consumer finance companies are required to report HMDA data if they meet the law's criteria for coverage.

There were 11.7 million loan records for calendar year (CY) 2014 reported by 7,062 financial institutions. These records include applications for home purchase, for home improvement, and for refinancing (see the field "PURPOSE" in the main HMDA table). The total record count is down 30 percent from CY 2013, although home purchases are up by four percent. 

Data generated by HMDA provides information on lending practices. The main data set is the Loan Application Register (LAR), called HMDA on the download provided by NICAR. It contains demographic information about loan applicants, including race, gender and income; the purpose of the loan (i.e. home purchase or improvement); whether the buyer intends to live in the home; the type of loan (i.e. conventional, FHA insured, etc.); the field "Rate_Spread," showing the difference between Treasury security interest rate and the loan's interest rate; and the outcome of the loan application (i.e. approved or declined). The lenders are given the opportunity to note reasons for denial in three fields, but those are seldom used.

The LAR data also includes geographical information on applicants, such as Census tract, MA (metropolitan area), state and county. 2010 Census information, such as total population and percentage of minority population by Census tract, is included as well.  

The names and addresses of lending institutions are stored in the Transmittal Sheet (TS.csv) and can be joined to the LARs data (HMDA tables) by using the RESP_ID and AGENCY fields in each table. You must use both RESP_ID and AGENCY. 

If you have any questions regarding the data, please contact the HMDA assistance line (202) 452-2016. The Federal Financial Institutions Examination Council's website also has several helpful resources on their website, including: 

*	A more detailed history of HMDA (http://www.ffiec.gov/hmda/history2.htm)
*	A glossary of useful terms (http://www.ffiec.gov/hmda/glossary.htm)
* 	FAQs: (http://www.ffiec.gov/hmda/faq.htm)
* 	Additional aggregate reports: (http://www.ffiec.gov/reports.htm)

Also, a good resource for background information and documents: http://www.stlouisfed.org/hmdaregcamendments/default.html

****The following tables should appear when you download or order the national dataset****

hmda14a.csv - The 4.2 million records of the Loan Application Register (LAR) for loan applications from the first 14 states (Alabama through Illinois, including DC). 

hmda14b.csv - The next 3.6 million records of the Loan Application Register (LAR) for loan applications from the last 21 states (Indiana through North Dakota).

hmda14c.csv - The next 4.1 million records of the Loan Application Register (LAR) for loan applications from the last 28 states (Ohio through Wyoming) as well as Puerto Rico and the 'NA' category.

In each of the above tables, you'll find information on persons seeking loans, as well as a respondent identification (RESP_ID) number that refers to the lending institution.

****Other files that should appear****

FIPS.TXT - This is the look-up table for state and county FIPS codes.

TS.csv - This is the lookup table of lending institutions. It also includes the respondent identification (RESP_ID). Please note: The RESP_ID is a unique identifier for each institution. Some RESP_IDs will appear multiple times. In this situation, you can use the AGENCY field to differentiate institutions.

RP.csv - The reporter panel is the universe of all institutions that reported under HMDA; it includes additional information on lending institutions. Please note: The RESP_ID is a unique identifier for each institution. Some RESP_IDs will appear multiple times. In this situation, you can use the AGENCY_CODE field to differentiate institutions.

MSA.csv - This is the Metropolitan Area lookup table.

MSAOFF.csv -  MSA/MDs with home or branch office


In the Layouts folder: 

REGIONAL.TXT - The different regional/district offices for each federal regulator and the states they are responsible for overseeing.

hmda_layout.txt - a record layout for the main hmda table

rp_layout.txt - a record layout for the reporter's panel

ts_layout.txt - a record layout for the transmittal sheet

msaoff_layout.txt - a record layout for the MSA office lookup table

layouts.xls - an Excel file containing all the above record layouts


In the Code_Sheets folder:

[YEAR]HMDALARRecordFormat.PDF - The FFIEC's record layout for the table HMDA.csv, not including NICAR-created fields

[YEAR]HMDACodeSheet.PDF - Code sheet for the latest edition.

[YEAR]HMDAInstitutionRecordFormat.PDF - Record layout for the lending institutions lookup table (TS.DBF).

[YEAR]HMDAReporterPanel.pdf - explanation and record layout of the RP table.

[YEAR]HMDAMSAOfficeFormat.pdf - FFIEC'S record layout of the table MSA.DBF


In the Agency_Documentation Folder:

TRANSITIONRULES.PDF - Transition rules provide lenders with guidance on collecting and reporting applications received before January 1, 2004 on which final action is taken in 2004.

REGULATIONC2004.PDF - The Federal Reserve Board's Regulation C for the Home Mortgage Disclosure Act (HMDA). The Official Staff Commentary contains Federal Reserve staff interpretations of Regulation C.

REGC_STAFF2004.PDF - Official Staff Commentary on Regulation C

HMDA_HELP_2006.PDF - Frequently asked questions about the new HMDA data

RE_APP-A-UPDATE.PDF - Standards for Maintaining, Collecting, and Presenting Federal Data on Race and Ethnicity

SPEC2010.PDF - Describes the required electronic format in which all institutions must submit their data. The file specifications are a required format and must be followed in order for the data to be processed.

Report_Guide_2013.pdf - The 2013 edition reflects the transfer of authority over Regulation C from the Federal Reserve Board to the Consumer Financial Protection Bureau. 

*******************************************************
* HMDA STORIES FROM THE IRE RESOURCE CENTER *
*******************************************************
To order copies of one or more of following stories call the IRE RESOURCE CENTER at 
573-884-3364 and give the the FILE NUMBER. The cost is 15 cents per page for IRE
members and 25 cents per page for non-members. There is also a $10 user fee for 
non-members.

FILE NUMBER: 23297
In 2007, The Morning Call of Allentown, Pa., utilized HMDA data, foreclosure reports and experts to explain how a wave of unstable mortgage loans were causing increasing numbers of uninformed borrowers to lose their homes. The investigation illustrated the problems faced by many people who, being unfamiliar with buying a home, ended up accepting very harsh terms on their loans and mortgages. Experts predict that this situation will lead to a rise in foreclosures in the area.

FILE NUMBER: 22110
This three-day series in the Charlotte Observer looked at many facets of home lending. The reporters used mortgage
loan data from 25 top lenders to show that blacks who bought homes in communities across America in 2004 were four
times as likely as whites to get high interest rates for mortgage loans. The interest rate disparities occurred even
when blacks had substantially higher incomes.
                                             
FILE NUMBER: 15381
Banks and mortgage companies still did relatively little business among minorities and 
in minority neighborhoods, the Kansas City Star reported in 1999. That even applies to the biggest banks, which under law must serve the entire area where they take deposits. Lenders still rejected minority mortgage applicants far more frequently than whites. Even high-income minorities were rejected more frequently than whites with lower incomes. These patterns didn't prove illegal discrimination. But taken with interviews with dozens of loan applicants, bankers, 
community activists, regulators and researchers, they show that barriers to minority homeownership still stand.               

TIPSHEETS FROM THE IRE RESOURCE CENTER

FILE NUMBER: 3296:
David Donald (Center for Public Integrity) and John Dunbar (Investigative Reporting Workshop) give pointers on tracking the bailout money funds. Included are links to Web sites and datasets to help inform stories on the bailout. Links provided include information on: subprime lenders; bailout cash/TARP funds; banking data; and enforcement actions.

FILE NUMBER: 3042
Tisha Thompson of WTTG-TV (Washington, D.C.) describes how to use the federal Home Mortgage Disclosure Act (HMDA) database in order to investigate subprime lending in your community. She explains what fields in the database will reveal subprime lending, and how to use an "update function" to count the subprime loans and apply a demographic element. The tipsheet ends with a list of helpful sources, such as the Consumer Federation of America and the State Licensing Board. 

FILE NUMBER: 3090
John Maines of the South Florida Sun-Sentinal discusses how to find data reported under the Home Mortgage Disclosure Act and query it to find information about high-interest loans. Maines also discusses how to tie the database results into a story about foreclosures in your area.

FILE NUMBER: 2626
Ted Mellnik of the Charlotte Observer writes about a series of stories he worked on involving high-interest mortgage loans and their typical ending: foreclosure. A 2003 story found rapidly increasing mortgage fraud, and a 2005 series described broad growth in high-interest mortgages -- both linked to foreclosure. His tipsheet looks at the role of the Federal Housing Administration and high-rate lenders in mortgage lending and how the affects forclosures. 

FILE NUMBER: 1774
From the 2003 computer-assisted reporting conference, a run down on what you need to have to do HMDA data based stories and what pitfalls to watch out for in said data. A list of recent changes to the HMDA data is also included.

IRE members can search and download tipsheets from www.ire.org/resourcenter.

Please call the NICAR office at (573) 884-7711 if you have any questions.

National Institute of Computer-Assisted Reporting
138 Neff Annex
Columbia, MO 65211
