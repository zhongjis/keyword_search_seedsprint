# keyword_search_seedsprint
this is a simple keyword matching system for Seedsprint. 

## Set Ups:
### 1: MongoDB
- should have a db called **workdata_seedsprint** 
- should have a collection called **fullname_skills** 
### 2: Gradle
- this program is built using Gradle. if you need to install it. you can use brew:
> brew install Gradle <br>

### 2: Source File
- please put source file under ***/src/main/resources*** 
- due to the format limitation of .xlsx file, please convert it to xlsm. 
- current version only support **one file** and the file name must be ***worddata1.xlsm***  

### 3: Known Issues
- HashMap dict_skill_fullNames is not correctly generated. the fullNames list is never updated when key exists.

## Update:
### August 9th, 2019
- now the tfidf calculation should be working
### August 7th, 2019
- every parts are ready except tfidf calculation 
- cuz this is the first version, all parts are hard coded. 
- database is not used, ignore database error for now.
- Thank you for your patience:)
