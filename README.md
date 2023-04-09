1#SORU - film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?

1#CEVAP - SELECT ROUND (AVG (rental_rate),2) FROM film;

1#<img width="960" alt="1" src="https://user-images.githubusercontent.com/129968939/230771982-1ae4c95a-2306-461b-8de0-7c1bd4535858.png">

2#SORU - film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?

2#CEVAP - SELECT COUNT (title) FROM film
WHERE title LIKE 'C%';

2#<img width="960" alt="2" src="https://user-images.githubusercontent.com/129968939/230772341-d7ba96ef-b3d5-46fc-83c6-7b34520e4ae9.png">

3#SORU - film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?

3#CEVAP - SELECT MAX (length) FROM film
WHERE rental_rate = 0.99;

3#<img width="960" alt="3" src="https://user-images.githubusercontent.com/129968939/230772450-8a4b060e-f959-4ba3-a1de-910790edd4db.png">

4#SORU - film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?

4#CEVAP - SELECT COUNT (DISTINCT replacement_cost) FROM film
WHERE length > 150;

4#<img width="960" alt="4" src="https://user-images.githubusercontent.com/129968939/230772595-fab385f4-30f3-4a36-80f9-0f41725ddab5.png">
