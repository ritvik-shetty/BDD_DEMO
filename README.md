# BDD_DEMO!




# To generate the bdd Allure report we need to do the following steps -

(We need to downlad java jdk and set the env variables before doing this)

1) Install the module allure using command : pip install allure-behave 

2) Later run the testcases using command : behave

3) But to get the data for the report we run the command : 
behave -f allure_behave.formatter:AllureFormatter -o reports/allure_result (This creates the json data for the report in the folder allure result inside reports folder)

4) To generate the HTML report we use the command : 
allure generate reports/allure_result -o results/allure_report --clean (This creates a new folder called allure_report and creates the html report for the  json data present in the allure_result.)


For GET request the report is :
![GET Allure-Report](<Screenshot (11).png>)

For POST request the report is :
![POST Allure-Report](<Screenshot (12).png>)

For PUT request the report is :
![PUT Allure-Report](<Screenshot (13).png>)

For DELETE request the report is :
![DELETE Allure-Report](<Screenshot (14).png>)