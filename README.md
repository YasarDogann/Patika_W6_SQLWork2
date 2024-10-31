# Patika+ Week6 SQL ile 2. Ödev Uygulaması
Merhaba,
Bu proje SQL ile Patika+ 6.hafta SQL komutları pratik için yapılmış bir uygulamadır.

## 📚 Proje Hakkında
Bu proje, aşağıdaki konuları öğrenmeye yardımcı olmak için tasarlanmıştır:
- Temel SQL komutları
- WHERE kullanımı
- AND ve OR kullanımı
- BETWEEN kullanımı
- IN kullanımı


## İstenilen Görev
Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
   - film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız ( BETWEEN - AND yapısını kullanınız.)
   - .actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.)
   - film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)

## Kod 
```sql
/*
Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
  1. film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla 
  sıralayınız ( BETWEEN - AND yapısını kullanınız.)
  
  2. .actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması 
  koşuluyla sıralayınız. ( IN operatörünü kullanınız.)
  
  3. film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma 
  koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)
*/


-- 1.SORU
SELECT * FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99;

-- 2.SORU
SELECT first_name, last_name FROM actor
WHERE first_name IN ('Penelope','Nick','Ed');

-- 3.SORU
SELECT * FROM film
WHERE rental_rate IN (0.99,2.99,4.99) AND replacement_cost IN (12.99, 15.99, 28.99);
```





