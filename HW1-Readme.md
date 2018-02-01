This data is sorted by the order identifier (order_id), quantity-the number ordered for this particular item,
item_name-the name of the dish, choice_description-constituents of this particular dish, 
price-price for the order on this line. 
Rows represent orders (one order can be many lines depending on the variety of items that were bought) 

head chipotle.tsv
tail chipotle.tsv #This shows that the last order_id is 1834

cat chipotle.tsv |wc -l #Gives 4623 lines in the data

grep -r "Steak Burrito" chipotle.tsv |wc -l #Finds 368 Steak Burritos

grep -r "Chicken Burrito" chipotle.tsv |wc -l #Finds 553 Chicken Burritos

grep -r "Chicken Burrito" chipotle.tsv |grep -r "Black Beans" | wc -l #Finds 282  Burritos with Black Beans

grep -r "Chicken Burrito" chipotle.tsv |grep -r "Black Beans" | wc -l #Finds 105 Burritos with Pinto Beans

#Hence there are 166 Chicken Burritos without any Beans

find . | grep tsv # Gives two data sets sms.tsv and chipotle.tsv

find . | grep csv | wc -l # finds 28 csv files

grep -r "dictionary" * |wc -l #finds 72 occurences of the word dictionary


