========================================================================
                 OTO KLİP ALMA BOTU - KULLANIM KILAVUZU
========================================================================

Bu program, Kick.com üzerindeki canlı yayınlarınızı saniyesi saniyesine 
dinleyerek, belirlediğiniz sihirli kelimeleri (örn: "klip al") söylediğiniz 
anda sohbete otomatik olarak "!clip" komutunu gönderir.

NASIL KULLANILIR?
------------------------------------------------------------------------
1. AYARLARI YAPIN
Programı çalıştırmadan önce, klasördeki "config.json" dosyasına sağ 
tıklayıp "Birlikte Aç -> Not Defteri" diyerek açın. 

Aşağıdaki bilgileri kendinize göre düzenleyin:
- "streamer_username": Kendi Kick kanal adınızı yazın. (örn: "Kafamkinder")
- "bot_auth_token": Kendi Kick hesabınızın yetki token'ını yazın. 
  (Bunu girmezseniz bot chat'e mesaj gönderemez.)
   [!] TOKEN NASIL ALINIR? 
  1) Tarayıcıdan Kick.com'a girin ve hesabınıza giriş yapın.
  2) Klavyeden F12 tuşuna basarak (veya sağ tık -> İncele diyerek) Geliştirici Araçları'nı açın.
  3) Üstteki sekmelerden "Network" (Ağ) sekmesine tıklayın.
  4) Kick sohbetine (chat) herhangi bir deneme mesajı yazıp gönderin.
  5) F12 ekranında aşağıya yeni satırlar düşecek. Chate yazı yazdıktan sonra çıkan satıra tıklayın.
  6) Sağ tarafta açılan panelde "Headers" (Başlıklar) bölümünü aşağı kaydırın.
  7) "Authorization" isimli satırı bulun. Karşısında yazan ve "Bearer" ile başlayan upuzun şifreyi (Örn: Bearer 3386738592|XPNxN...) kopyalayıp config dosyasında ilgili yerdeki tırnak işaretinin içine yapıştırın.
  
- "cooldown_seconds": Üst üste klip almasını önlemek için bekleme süresi 
  (saniye cinsinden).
- "wake_words": Sistemin tetiklenmesini istediğiniz kelimeler. İstediğiniz 
  kadar kelime veya cümle ekleyebilirsiniz.

2. PROGRAMI ÇALIŞTIRIN
Ayarları kaydedip kapattıktan sonra "OtoKlip.exe" dosyasına çift tıklayın.

* İlk Açılış: Program ilk defa açıldığında yapay zeka ses tanıma motorunu 
  (yaklaşık 45 MB) bilgisayarınıza indirecektir. Bu işlem internet hızınıza 
  bağlı olarak 1-2 dakika sürebilir. Bu işlem sadece bir kere yapılır.
  
* Yayını Dinleme: Model yüklendikten sonra program canlı yayınınızı arka 
  planda dinlemeye başlar. Siz "klip al" dediğinizde program bunu algılar
  ve hemen sohbete "!clip" komutu yazar.

------------------------------------------------------------------------
ÖNEMLİ NOTLAR VE İPUÇLARI:
* Esnek Algılama: Hızlı konuşurken "klip al" yerine "flip al" veya "kılip al" 
  derseniz bile sistem bunu anlar ve klibi alır. (Esnek eşleştirme %85 benzerlik 
  üzerinden çalışır).
* Güvenlik: Kimseye "config.json" içindeki "bot_auth_token" bilginizi atmayın!
* Kapatmak: Programı kapatmak için siyah ekranın sağ üstündeki çarpıya (X) 
  basmanız yeterlidir.

İyi yayınlar! 🎮
