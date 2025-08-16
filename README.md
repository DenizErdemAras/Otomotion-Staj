# Otomotion-Staj

Stajda süresince yazdığım, elimde bulunan çalışır haldeki bitmiş projeler.

Kodların çalıştırılabilmesi için TwinCAT 3 programı gerekli. Ama sadece kodları görmek için, proje dosyaları içinde bulunan POUs klasöründeki dosyalara bakabilirsiniz. (TC2_ServoPiano hariç. Bu bir TwinCAT 2 projesi ve kodlar programsız görüntülenemiyor.)

## Rampa Bloğu (Rampa Blogu)
İstenen hedef değere belirtilen artış ve azalış sürelerinde ulaşan fonksiyon bloğu.

Bu örnek bir motorun dönme hızını RPM cinsinden kontrol ediyormuş gibi hazırlandı.

rTarget değeri değişince, eğer değer artacaksa rAccelerationTime, azalacaksa rDecelerationTime kadar bir sürede hedef değere sinüsoidal bir eğri ile rRPM değerini rTarget'a ulaştırıyor.

![demo](https://github.com/DenizErdemAras/Otomotion-Staj/blob/a6707ab1886404050e4b50c0cfa450286d6df82f/Gif/rampa_blogu.gif)


## Çember İçinde Dönen Çember (TwinCAT Project2 Visualisation Test)
Büyük çemberin içinde ona değerek dönen küçük çember.

![demo](https://github.com/DenizErdemAras/Otomotion-Staj/blob/a001bf171f01b19173778c35d86e45ada6a33280/Gif/visualisation_test.gif)


## Lineer Aktüatör Konum Hesabı (lineer aktüatör hesap)
Bir ucu çembere bağlı, diğer ucu yatay doğrusal hareket yapabilen çubuğun; çemberin boyutuna göre hareket edebileceği alanı ve çemberin açısına göre konumunu hesaplayıp görselleştiren program.

![demo](https://github.com/DenizErdemAras/Otomotion-Staj/blob/a001bf171f01b19173778c35d86e45ada6a33280/Gif/lineer_aktutator_hesap.gif)


## PID Konrol (PID Control)
Fonksiyon bloklarıyla hazırlanmış bir gerilim kontrol sistemi simülasyonu.

Simülasyon dancer roll (balerin rulosu), dancer'den çıkan malzemeyi kontrol eden bir motor ve PID kontrolcüden oluşuyor.

Dancer, içine giren ve çıkan malzeme hızı farkı yüzünden biriken malzemeyi bir yüzdelik değere dönüştürüyor. Giren malzeme hızını basit bir fonksiyonla sürekli değişecek şekilde ayarladım.

Görseldeki sarı renkli çizgi hedef yüzde değerini gösteriyor. Kahverengi olan ise gerçek yüzdeyi.

Hedef değer şu ankinden farklı olunca PID sistemi motor hızını değiştiriyor. Bu dancer'den çıkan malzemeyi (r_out_material) etkiliyor.

Gerçek değer hedefe ulaşınca sistem r_in_material ve r_out_material'i eşit tutup bu değeri korumaya çalışıyor.

![demo](https://github.com/DenizErdemAras/Otomotion-Staj/blob/a001bf171f01b19173778c35d86e45ada6a33280/Gif/PID_dancer_visu.gif)


## Servo Piyano (Servo Piyano) (TC2_ServoPiano)
(Bu programı başka bir bilgisayarda TwinCAT 2 kullanarak yazdım. Daha sonra kodu bende de dursun diye bir kısmını kendi bilgisayarıma taşımaya çalıştım. Grafik arayüz kısmı olmadığı için TwinCAT 3 için olan versiyonu çalışmaz halde.)

(TwinCAT 2 dosyası da mevcut (TC2_ServoPiano) ama kodlar dosyadan kolayca görüntülenemiyor. Sadece TwinCAT 2 programıyla görüntülenebiliyor.)

Bir servo motoru farklı hızda döndürerek basılan piyano tuşunun sesini çıkaran veya müzik çalabilen program.

Ses de gerekli olduğu için buna gif değil, video koydum.

https://drive.google.com/file/d/11DFyeIzoYNQO2H27AdMxx5bk8NdaiOdF/view
