# patika.dev-SQL-Practice06
patika.dev-SQL-Practice06

🔸film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
✅ Ortalama 2.98 dir.
``` sql
SELECT ROUND(AVG(RENTAL_RATE),2) FROM FILM

```
🔸film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
✅ 92 dir
``` sql
SELECT COUNT(*) FROM FILM
WHERE title LIKE 'C%'

```

🔸film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
✅ 184 dk dir
``` sql
SELECT MAX(LENGTH)
FROM FILM
WHERE RENTAL_RATE = 0.99
```
🔸film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
✅21 dir
``` sql
SELECT COUNT(DISTINCT(REPLACEMENT_COST))
FROM FILM
WHERE LENGTH > 150;

```
app.patika.dev/emintunahan
