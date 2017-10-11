Apriori Algorithm and Example with Association Rule

This repository shows you about using Apriori Algorithm for dataset ("Makanan in Bahasa Indonesia" or Food Collection that consumed by me everyday).
1. I have an dataset which create from mysql file, and i choose for my data in id_user = 3
.sql file included in this project. 
2. I query to get my data with this query : SELECT * from tbl_makan INNER join tbl_makan_makanan on tbl_makan.id_makan = tbl_makan_makanan.id_makan WHERE tbl_makan.id_user=3 order by tbl_makan.tanggal, tbl_makan.waktu_makan
3. Then i export to csv file for Excel.
4. I write the number code of each food that already in the database. I do it with Main.java file
 5. Then I create ther formater tool (Format.java) and the result can be assign to the main Apriori Program format, then make makanan.dat file.
 6. Create Apriori.java file that contain Apriori Algorithm with Association Rules.
 7. Compile the Apriori.java : javac Apriori.java and then execute main command : java Apriori makanan.dat 0.2 0.3 where the 0.2 refers to support and the 0.3 refers to the confidence
  
Credit to :
1. Anugrah Dwiatmaja Putra that make a little software to record the food
2. Convert text to String array. http://textmechanic.com/text-tools/basic-text-tools/add-prefixsuffix-into-line/
3. Main Apriori Algorithm Program by Engineer-RC and monperrus : https://gist.github.com/ENGINEER-RC/34bdc63161befad19ce33564a473fc58