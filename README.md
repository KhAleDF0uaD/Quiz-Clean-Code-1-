# Quiz-Clean-Code-1-c.21-l.1-
Clean
Define

    Select all nondescriptive and misspelled column headers (ApplicationP, AboutC, RequiredQual, JobRequirment) and replace them with full words (ApplicationProcedure, AboutCompany, RequiredQualifications, JobRequirement)
    Select all records in the StartDate column that have "As soon as possible", "Immediately", etc. and replace the text in those cells with "ASAP"

Code

df_clean = df.copy()

    Select all nondescriptive and misspelled column headers (ApplicationP, AboutC, RequiredQual, JobRequirment) and replace them with full words (ApplicationProcedure, AboutCompany, RequiredQualifications, JobRequirement)

df_clean = df_clean.rename(columns={'oldName1': 'newName1',

                                    'oldName2': 'newName2'})
