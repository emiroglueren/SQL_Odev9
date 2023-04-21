# ODEV 9

Merhabalar,


Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

    city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
    customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
    customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.


Kolay Gelsin.

# CEVAPLAR:

## 1.Soru:

SELECT city.city, country.country FROM city
INNER JOIN country ON city.country_id = country.country_id;

## 2.Soru:

SELECT payment.payment_id, customer.first_name, customer.last_name FROM customer
INNER JOIN payment ON customer.customer_id = payment.customer_id;

## 3.Soru:

SELECT rental.rental_id, customer.first_name, customer.last_name FROM customer
INNER JOIN rental ON customer.customer_id = rental.customer_id;

