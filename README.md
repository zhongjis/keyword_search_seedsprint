# keyword_search_seedsprint
this is a simple keyword matching system for Seedsprint. 

## Set Ups:
### 1: MongoDB
- should have a db called **workdata_seedsprint** 
- should have a collection called **fullname_skills** 

### 2: Gradle
- this program is built using Gradle. if you need to install it. you can use brew:
> brew install Gradle <br>
- if you want to run the program, please navigate to the project folder and run:
> gradle init && gradle run

### 3: Source File
- please put source file under ***/src/main/resources*** 
- due to the format limitation of .xlsx file, please convert it to xlsm. 

## Example Output
- all skills will be printed in the console like

> [INFO] term: Big Six Non-O157 STEC Panels: tfidf 6.054439346269371 <br>
> [INFO] term: Six Sigma: tfidf 6.054439346269371 <br>
> [INFO] term: Project Management: tfidf 4.2626798770413155 <br>
> [INFO] term: Strategy: tfidf 4.2626798770413155 <br>
> [INFO] term: Mobile Devices: tfidf 6.054439346269371 <br>
> [INFO] term: Deal Structuring: tfidf 6.054439346269371 <br>
> [INFO] term: food safety modernization act: tfidf 6.054439346269371 <br>
> [INFO] term: Chemietechnik: tfidf 6.054439346269371 <br>

**bigger the tfidf is, means the skill is rarer**. I will add a ranking program later to rank all the term/skills.

## Known Issues
1. due to the layout differences among all workdata files. the skill and names extraction feature is not functioning correctly.

## Update:
### August 14th, 2019
- now the program will find all .xslm files under resources folder.
- now you will see more prompts and know what's going on in the program. this also helps debugging.

### August 9th, 2019
- now the tfidf calculation should be working
- Known Issue: HashMap dict_skill_fullNames is not correctly generated. the fullNames list is never updated when key exists. (Solved)

### August 7th, 2019
- every parts are ready except tfidf calculation 
- cuz this is the first version, all parts are hard coded. 
- database is not used, ignore database error for now.
- Thank you for your patience:)
