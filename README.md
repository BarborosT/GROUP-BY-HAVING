# GROUP-BY-HAVING

1.film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.

`Select * From film Group By rating `

2.film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

`Select replacement_cost ,COUNT(*) From film Group By replacement_cost Having COUNT(*)>50 Order By COUNT(*)`

3.customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir? 

`Select COUNT(*) store_id From Customer`

4. city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

`Select COUNT(*),country_id  From city Group By country_id Order By COUNT(*) DESC`
