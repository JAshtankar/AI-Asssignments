//***********PROMPT**********************
Instructions
- Generate a excel formulas for fetching data from excel2 to excel1 having FI_document_number and respective AMOUNT common filed 
- Fetch amount value from file2 to filed1 agains FI_document number
- Compare amount valued form file2 to file1 and if value is matching add new column STATUS and add 0 in front of fetching row 

Context
Act like a Account manager

Example 1:
File1: FI_document_number=FI_Doc_002, AMOUNT=2000
File2: FI_document_number=FI_Doc_002, AMOUNT=2000
NEW_ROW: FI_document_number=FI_Doc_002, AMOUNT=2000, AMOUNT2=2000 STATUS=0

Example 2:
File1: FI_document_number=FI_Doc_002, AMOUNT=2500
File2: FI_document_number=FI_Doc_002, AMOUNT=2000
NEW_ROW: FI_document_number=FI_Doc_002, AMOUNT=2500, AMOUNT2=2000 STATUS=BLANK

Tone:
[STRICTLY] ACCURACY 

Output:
Downloadable updated EXCEL having new STATUS column in it

Persona
Act as a Account manager to generate and reviewed excel with ACCURACY
//**************Response*************************************
I’ll give you accurate, production-ready Excel formulas exactly how an Accounts Manager would implement reconciliation.

Since I cannot directly attach/download a file here, I’ll give you:

Exact column structure
Precise formulas
Steps to generate your final Excel
✅ ASSUMPTION (Structure)
File1 (Main file – where you want results)
A	B
FI_document_number	AMOUNT
File2 (Source file)
A	B
FI_document_number	AMOUNT
✅ STEP 1: ADD NEW COLUMNS IN FILE1

Add 2 new columns:

C	D
AMOUNT2	STATUS