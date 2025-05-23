
# DEPREM VERİLERİ

Kandilli Rasathanesi sitesinden deprem verileri alıp Excel dosyası olarak kaydetmektedir.

[http://www.koeri.boun.edu.tr/scripts/lst6.asp]


## Yükleme 

gerekli kütüphaneleri pip install ile  yükleyin

```bash 
  pip install pandas requests openpyxl
  
```

## Kullanım

```
python deprem.py
```

Python dosyasında 29.satırda bulunan :
```python
for line in lines[:250]:
```
250 rakamını değiştirerek alınması istenen deprem sayısını belirleyebilirsiniz.

## Özellikler

- Excel dosyası olarak kayıt yapar.
- Excel dosyasında Tarih, Saat, Enlem, Boylam, Derinlik, ML, Mw, Yer, Harita bilgileri yer almaktadır.
- Excel dosyasında Deprem Şiddeti 3-5 arasında olan yerler "SARI", 5 ve üstü yerler "KIRMIZI" dolgu ile belirtilmiştir.
- Harita sütununda ilgili yerin harita linki yer almaktadır.
- Harita linkleri için [https://www.openstreetmap.org/] kullanılmıştır.


## Ekran Görüntüleri

![Ekran Görüntüsü](https://github.com/mustafa-ozlu/DepremVerileri/blob/main/Screenshot.png)

