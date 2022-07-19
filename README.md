# SQL9
patika.dev linkim: https://app.patika.dev/cmilakonur <br />

Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz. <br />

1-city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız. <br />
SELECT city,country <br />
FROM city <br />
INNER JOIN country ON city.country_id = country.country_id; <br />

2-customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name <br />
isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız. <br />
SELECT customer.first_name,customer.last_name,payment.customer_id,payment.payment_id,payment.amount <br />
FROM customer <br />
INNER JOIN payment ON customer.customer_id = payment.customer_id; <br />

3-customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name <br />
isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız. <br />
SELECT customer.first_name,customer.last_name,rental.rental_id <br />
FROM customer <br />
INNER JOIN rental ON rental.customer_id = customer.customer_id; <br />
