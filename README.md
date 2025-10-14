# FDA-drugs 

<img src="https://imgs.search.brave.com/MkngS6eksTucRa-f6JVOHziuWe5SWDFnVdWWKPn-CbE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly93d3cu/cG5nbWFydC5jb20v/ZmlsZXMvMjMvRmRh/LUxvZ28tUE5HLVBo/b3Rvcy5wbmc" height=300>

dataset of FDA approved drugs including molecular formulas


## data sources

- MAIN PAGE - https://www.accessdata.fda.gov/scripts/cder/daf/index.cfm
- DrugBank  - https://go.drugbank.com/

## abreviations

- NDA = new drug application  
- Biological License application (BLA) 
- Abbreviated New Drug Application (ANDA)
- PBT `molecular_formula` is Protein Based Therapy (meaning there is no molecular formula available)
- OTC over the counter 


all NDA numeric values can be for either NDA | BLA | ANDA

## drug names

- short name (ex: `anisotropine methylbromide` --> `anisotropine`)
- drug name --> active ingredient. not all drug names return data but active ingredient does (ex: anhydron --> cyclothiazide)
- drug names searched using the API were the `active ingredient` 

## data categories

| column            | meaning                    |
|-------------------|----------------------------|
| drug_name         | shortened name of the drug |
| NDA_id            | `integer` id for drug      |
| company           | pharmaceutical company     |
| dosage_form       | physical form drug comes in |
| route             | how the drug is delivered  |
| therapy           | what the drug is used for  |
| status            | Prescribed/ Discontinued/ OTC |
| molecular_formula | empirical formula of drug   |


