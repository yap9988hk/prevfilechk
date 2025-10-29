# Prevfilechk - Previous File Checking
Previous File (PF) checking is a logic that run to check all the previous file during underwriting process.
Current model is extracted to specifically demonstrate the PF checking.

### Rule #1  
HasExistingCover must be True  
Total Previous LOAD minus Total Current LOAD more than 50  
Daysapart less than or equal to 1095  
**-> Result : Decline**  

###  Rule #2  
HasExistingCover must be True  
Total Number of EMC in Previous minus Total Number of EMC in Current is more than 1  
Daysapart less than or equal to 1825  
**-> Result : Decline**

### Rule #3  
HasExistingCover must be True  
*Previous application has any LD1 code that current application doesn't have*  
Daysapart less than or equal to 1825  
**-> Result : Decline**

### Rule #4  
HasExistingCover must be True  
*Previous application has any LD1 code that current application doesn't have*  
Daysapart greater than 1825  
**-> Result : Modified Declaration**

### Rule #5  
HasExistingCover must be True  
Total Previous LOAD minus Total Current LOAD more than 50  
Daysapart greater than 1095  
**-> Result : Modified Declaration**

### Rule #6  
HasExistingCover must be True  
Total Number of EMC in Previous minus Total Number of EMC in Current is more than 1  
Daysapart greater than 1825  
**-> Result : Modified Declaration**

### Rule #7  
HasExistingCover must be True  
Total Number of EMC in Previous minus Total Number of EMC in Current equal to 1  
**-> Result : Modified Declaration**

### Rule #8  
HasExistingCover must be True  
*Previous application has any EMC code that current application doesn't have*  
**-> Result : Modified Declaration**

### Rule #9  
HasExistingCover must be True  
Total Previous LOAD minus Total Current LOAD is between 1 to 50  
**-> Result : Modified Declaration**

### Rule #10  
HasExistingCover must be True  
*Previous application has any LOAD code that current application doesn't have or have but with lesser loading amount*  
**-> Result : Modified Declaration**
