# APRIORI ALGORİTMASI İLE MARKET SEPETİ ANALİZİ #

Bu proje, Apriori Algoritması kullanarak market alışveriş verilerinden ürünler arasındaki gizli ilişkileri bulmayı amaçlamaktadır. Algoritma, sıkça birlikte satın alınan ürün kümelerini belirler ve bu bilgiler, pazarlama stratejileri geliştirmek veya müşterilere öneriler sunmak için kullanılabilir.

# **Proje Özeti** 

+ Veri Seti: Market alışverişlerinden elde edilen işlem (transaction) verileri.
+ Apriori Algoritması: En sık ürün kümelerini ve bu kümeler arasındaki birliktelik kurallarını (support, confidence, lift) çıkarır.
+ Görselleştirme: Ürünler arasındaki ilişkiler ve birliktelik kuralları çeşitli grafiklerle görselleştirilmiştir (bar grafikleri, ağ grafiği, ısı haritası).
+ Ürün Öneri Sistemi: Belirli bir ürünü satın alan müşterilere önerilecek diğer ürünleri sunan bir sistem geliştirilmiştir.

# Adım Adım Uygulama 

1. Veri Hazırlama:

+ Veriler NaN değerlerinden arındırılmış ve one-hot encoding ile işlenmiştir.

2. Sık Ürün Kümeleri:

+ Apriori algoritmasıyla minimum %5 destek eşiğine sahip sık ürün kümeleri bulunmuştur.

3. Birliktelik Kuralları:

+  Ürünler arasındaki ilişkiler, lift ve confidence gibi metriklerle analiz edilmiştir.
Görselleştirme:

+ En sık ürün kümeleri: Destek oranlarına göre bar grafikleri.
+ Ürün ilişkileri ağı: NetworkX ile ürünler arasındaki ilişkiler görselleştirilmiştir.
+ Isı haritası: Ürünler arası güven oranları ısı haritasıyla sunulmuştur.
+ Kelime bulutu: En popüler ürün kümeleri kelime bulutu ile görselleştirilmiştir.

5. Öneri Sistemi:

+ Satın alınan bir ürüne göre, kullanıcıya önerilecek ürünleri listeleyen bir fonksiyon.


# Gereksinimler
+ Python 3.x
+ Pandas
+ Mlxtend
+ Matplotlib
+ Seaborn
+ NetworkX
+ WordCloud
