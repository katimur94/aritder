# 🐝 ARITDER Sitesi — Kullanım Rehberi

## 🌐 SİTE CANLI YAYINDA!
- **Site adresi:** https://katimur94.github.io/aritder/
- **Kod deposu:** https://github.com/katimur94/aritder
- Güncelleme yapmak için: `index.html`'i düzenleyin → GitHub'daki repoya yükleyin (github.com/katimur94/aritder → "Add file" → "Upload files") → 1-2 dakika içinde site kendini günceller. Ya da Claude'a "siteyi güncelle" deyin, o halleder.

## Siteyi açmak
`index.html` dosyasına **çift tıklayın** — tarayıcıda açılır. Kurulum, program, internet sunucusu gerekmez; sitenin tamamı tek dosyadır.

## Kendinize göre ayarlamak
`index.html` dosyasını Not Defteri ile açın ve en alttaki **AYARLAR** bölümünü bulun:

```
const AYARLAR = {
  facebookSayfa: "ARIT74",          ← Facebook sayfanızın adı (facebook.com/XXXX)
  instagramKullanici: "aritder",    ← Instagram kullanıcı adınız (@ olmadan)
  senlikBaslangic: "2026-08-14T13:00:00+03:00",
  senlikBitis:     "2026-08-16T22:00:00+03:00",
  ...
};
```

- **Facebook akışı otomatiktir:** Sayfanızda yeni gönderi paylaştığınızda sitede kendiliğinden görünür (Facebook'un resmî "Sayfa Eklentisi" kullanılır, şifre/anahtar gerekmez). Şu an örnek olarak en büyük Arıt topluluk sayfası **ARIT74** bağlı — derneğin kendi sayfası açılınca sadece bu satırı değiştirin.
- **Instagram:** Instagram, profil akışını izinsiz gömmeye izin vermez; bu yüzden şık bir profil kartı ve konum etiketi bağlantısı kullanıldı. Kullanıcı adınızı AYARLAR'a yazmanız yeterli.
- **Geri sayım:** Şenlik tarihlerini her yıl AYARLAR'dan güncelleyin; sayaç otomatik olarak "şenlik sürüyor 🎉" ve "sona erdi 🍂" durumlarına da geçer.
- **İletişim bilgileri:** "İletişim" bölümündeki e-posta/telefon yer tutucularını kendi bilgilerinizle değiştirin.

## İnternete yayınlamak — TÜRKİYE İÇİN ÖNEMLİ ⚠️

**Vercel'in ücretsiz adresleri (xxx.vercel.app) Türkiye'de BTK tarafından engellendi** — Cloudflare Pages'in ücretsiz adresleri (pages.dev) de aynı durumda. Yani "Vercel'e yükle, ücretsiz linki paylaş" yöntemi Türkiye'deki ziyaretçiler için ÇALIŞMAZ. Çözümler:

### Yol 1 — En sağlam ve tavsiye edilen: Türk hosting + .org.tr alan adı 🇹🇷
1. **Alan adı alın:** `aritder.org.tr` gibi. 2022'den beri (TRABİS sistemi) org.tr için **belge gerekmiyor**, "ilk gelen alır". Natro, Turhost, İsimtescil, Hosting.com.tr gibi BTK yetkili firmalardan yıllık ~birkaç yüz TL'ye alınır.
2. **Basit bir hosting paketi alın** (aynı firmadan, en ucuz "web hosting" paketi yeter — site tek dosya!). `index.html`'i firmanın panelinden yükleyin, bitti.
3. **Artı:** Bu paketlerde `baskan@aritder.org.tr` gibi **e-posta kutuları ücretsiz dahildir** ve Türkiye'den erişim/hız sorunu yaşanmaz, Türkçe telefon desteği vardır.

### Yol 2 — Tamamen ücretsiz: GitHub Pages
- github.com'da hesap açın → depo oluşturun → `index.html`'i yükleyin → Settings → Pages → yayınla.
- `kullaniciadi.github.io/aritder` adresi Türkiye'den açılıyor. Sonradan kendi alan adınızı da bağlayabilirsiniz.

### Yol 3 — Vercel/Netlify + kendi alan adınız
- Engel yalnızca ücretsiz ortak uzantılara (vercel.app / pages.dev) uygulanıyor; **kendi alan adınızı bağlarsanız** (aritder.org.tr) site Türkiye'den açılır. Yine de Yol 1 daha dertsizdir.

## Dernek e-postası (baskan@aritder.org.tr gibi)
- **Hosting paketiyle geldiyse:** ekstra hiçbir şey gerekmez, panelden kutu açarsınız. ✅ En kolayı.
- **Ücretsiz istiyorsanız:** **Zoho Mail** — kendi alan adınızla **5 kullanıcıya kadar ücretsiz** (kutu başı 5 GB). Yandex'in eskiden ücretsiz olan kurumsal maili artık ücretli, Google Workspace da ücretli; ücretsiz sınıfta en iyisi Zoho.
- Kurulum: alan adını aldığınız panelde Zoho'nun verdiği MX kayıtlarını girmek (10 dk, adım adım anlatıyorlar).

## Sitede neler var?
- 🎪 Şenliğe canlı geri sayım (14–16 Ağustos, Tarık Yüksel & Tayfur Çalık konserleri, safari, off-road)
- 🌤️ Arıt'ın **gerçek zamanlı hava durumu** (Open-Meteo, ücretsiz, anahtarsız)
- 📜 1530 "Arıd Divanı"ndan bugüne zaman tüneli
- 🗺️ Gürcüoluk Mağarası, Küre Dağları, Amasra, lav sütunları tanıtımları
- 🎬 YouTube'dan Arıt şenlik ve Bartın drone videoları (gömülü)
- 🖼️ Wikimedia Commons'tan gerçek Arıt fotoğraflı, büyütmeli galeri
- 📘 Facebook canlı akışı + Instagram kartı
- 🗺️ OpenStreetMap üzerinde Arıt haritası
- 🌙 Gece/gündüz modu, uçan arı, bal damlası kaydırma çubuğu 🐝
