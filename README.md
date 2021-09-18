# SQL_ODEV9
**Patika.dev sayfasındaki SQL eğitimi kapsamında yaptığım 9. ödev**
------------------------
1._city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız._
```sql
SELECT city, country FROM city
INNER JOIN country ON country.country_id =city.city_id ;
```
2._customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız._
```sql
SELECT  payment_id, first_name, last_name FROM customer
INNER JOIN payment ON payment.customer_id = customer.customer_id ;
```
3._customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız._
```sql
SELECT  rental_id, first_name, last_name FROM customer
INNER JOIN rental ON rental.customer_id = customer.customer_id ;
```
------------------------------------
**Sorgu senaryolarını [dvdrental.tar](https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip) isimli dosyayı indirerek gerçekleştirebilirsiniz.**
