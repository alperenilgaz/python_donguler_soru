# python_donguler_soru
--------------------------
## Problem 1 :
----------------
Kullanıcıdan aldığınız bir sayının mükemmel olup olmadığını bulmaya çalışın.

Bir sayının kendi hariç bölenlerinin toplamı kendine eşitse bu sayıya "mükemmel sayı" denir. Örnek olarak, 6 mükemmel bir sayıdır. (1 + 2 + 3 = 6)
cevap :
--------
sayı=int(input("bir sayı giriniz :"))
i=1
toplam=0
while(i<sayı):

    if(sayı%i==0):
        toplam+=i
        i += 1

    elif(sayı==toplam) :
        print("girdiğiniz sayı mükemmel sayıdır.")
        break

    else :
        print("giridiğiniz sayı mükemmel sayı değildir.")
        break
------------------------------------------------------------------------------------------------------------------------------------------------------
## Problem 2 :
-------------
Kullanıcıdan aldığınız bir sayının "Armstrong" sayısı olup olmadığını bulmaya çalışın.

Örnek olarak, Bir sayı eğer 4 basamaklı ise ve oluşturan rakamlardan herbirinin 4. kuvvetinin toplamı( 3 basamaklı sayılar için 3.kuvveti ) o sayıya eşitse bu sayıya "Armstrong" sayısı denir.

Örnek olarak : 1634 = 1^4 + 6^4 + 3^4 + 4^4
cevap :
--------
sayı = input("Sayı:")
basamak_sayisi = len(sayı)
sayı = int(sayı)
basamak = 0
toplam = 0

gecici_sayı = sayı

while (gecici_sayı > 0):
    basamak = gecici_sayı % 10

    toplam += basamak ** basamak_sayisi

    gecici_sayı //= 10

if (toplam == sayı):
    print(sayı, "bir armstrong sayısıdır.")
else:
    print(sayı, "bir armstrong sayısı değildir.")

SORULACAK BEN ÇÖZMEDİM.............................
----------------------------------------------------------------------------------------------------------------------------------------------------

## Problem 3 :
-------------
1'den 10'kadar olan sayılarla ekrana çarpım tablosu bastırmaya çalışın.

İpucu: İç içe 2 tane for döngüsü kullanın. Aynı zamanda sayıları range() fonksiyonunu kullanarak elde edin.

cevap :
--------
for i in range(1,11) :
    print("*************************************************************")
    for j in  range (1,11):
        print("{}x{}={}".format(i,j,i*j))
----------------------------------------------------------------------------------------------------------------------------------------------------
## Problem 4 :
-------------
Her bir while döngüsünde kullanıcıdan bir sayı alın ve kullanıcının girdiği sayıları "toplam" isimli bir değişkene ekleyin. Kullanıcı "q" tuşuna bastığı zaman döngüyü sonlandırın ve ekrana "toplam değişkenini" bastırın.

İpucu : while döngüsünü sonsuz koşulla başlatın ve kullanıcı q'ya basarsa döngüyü break ile sonlandırın.

cevap :
--------
toplam=0
while True:
    sayı=input("bir sayı giriniz :")
    if(sayı=="q"):
        break

    sayı=int(sayı)
    toplam+=sayı
print("girdiğiniz değerlerin toplamı :",toplam)

---------------------------------------------------------------------------------------------------------------------------------------------------

## Problem 5 :
-------------
1'den 100'e kadar olan sayılardan sadece 3'e bölünen sayıları ekrana bastırın. Bu işlemi continue ile yapmaya çalışın.

cevap :
--------

for i in range(1,101):
    if(i%3!=0) :
        continue
    
     print(i)

----------------------------------------------------------------------------------------------------------------------------------------------------
## Problem 6 :
-------------
Buradaki problemin çözümünü derslerimizde özellikle öğrenmedik. Burada mantık yürüterek ve list comprehension kullanarak 1'den 100'e kadar olan sayılardan sadece çift sayıları bir listeye atmayı yapmayı çalışın.

Not: Programlamada her detayı öğrenemeyiz. Bunun için bazı yerlerde deneme yanılma yoluyla da öğrendiğimiz şeyler olur. Bu problemde deneme yanılma yoluyla list comprehension'ın koşullu durumlarla kullanımını öğreneceksiniz.

İpucu: Basit düşünmeye çalışın.

cevap :
--------
liste=[i for i in range(1,101) if i%2==0]
print(liste)











