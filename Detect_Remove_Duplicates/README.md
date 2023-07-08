# Detecting and Remove Duplicates
* Used CTE and ROW_NUMBER()
* Microsoft SQL Server Management

## Explanation
* Used a SQL Query to choose columns and also use ROW_NUMBER to give a corresponding number role and use the partition clause by CustomerID to see how many duplicates within the dataset we have
* Now that we have detected the duplicates by assigining numbers to each row and using partition to essentially group the duplicates together we want to focus on removing the duplicates by using C.T.E also known as Common Table Expression
* Using CTE and putting the query within the paranatheses we remove duplicates by only selecting the rows where the id is equal to 1.
* For an example in the first image we have ALFKI with a total of 6 ID's or 6 duplicates, then we have ANATR with 4 ID's or 4 dupliactes. A way for us to remove those duplicates is to only choose the first ID for each CustomerID as seen in the second image.

Image 1:
![](https://github.com/Nwiradiradja/DataCleaning-SQL/blob/main/Detect_Remove_Duplicates/Detect1.png?raw=true)

Image 2:
![](https://github.com/Nwiradiradja/DataCleaning-SQL/blob/main/Detect_Remove_Duplicates/Detect2.png?raw=true)

