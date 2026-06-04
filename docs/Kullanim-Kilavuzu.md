# 📘 TUS Master Pro — Kullanım Kılavuzu

TUS hazırlığı için yapay zekâ destekli masaüstü çalışma uygulaması. Bu kılavuz tüm özellikleri adım adım anlatır. Kısa cevaplar için **[SSS](SSS.md)**'ye bakabilirsin.

## İçindekiler
1. [TusMaster nedir?](#1-tusmaster-nedir)
2. [Kurulum (mac & Windows)](#2-kurulum)
3. [İlk açılış sihirbazı](#3-i̇lk-açılış-sihirbazı)
4. [Ekranı tanıyalım](#4-ekranı-tanıyalım)
5. [Soru çözme](#5-soru-çözme)
6. [🧠 Kalıcı Hafıza (SRS)](#6--kalıcı-hafıza-srs)
7. [Bugünün Planı](#7-bugünün-planı)
8. [TUS Simülatörü](#8-tus-simülatörü)
9. [İlaç Kartları](#9-i̇laç-kartları)
10. [Analiz](#10-analiz)
11. [Tekrar](#11-tekrar)
12. [Yapay zekâ araçları](#12-yapay-zekâ-araçları)
13. [Kendi denemeni ekleme](#13-kendi-denemeni-ekleme)
14. [API anahtarı & kota yönetimi](#14-api-anahtarı--kota-yönetimi)
15. [Yedekler, verilerin ve gizlilik](#15-yedekler-verilerin-ve-gizlilik)
16. [Tema, sayaç ve küçük ayarlar](#16-tema-sayaç-ve-küçük-ayarlar)
17. [Çalışma ipuçları](#17-çalışma-i̇puçları)
18. [Sorun giderme](#18-sorun-giderme)
19. [⚠️ Tıbbi sorumluluk](#19-️-tıbbi-sorumluluk)

---

## 1. TusMaster nedir?
- **2.400'ü aşkın telifsiz çalışma sorusu** hazır gelir — bunlar gerçek ÖSYM soruları değil, yapay zekâ ile üretilmiş, aynı tarzda **varyant** sorulardır (telif nedeniyle gerçek çıkmışlar gelmez; kendi denemeni ekleyebilirsin — bkz. [bölüm 13](#13-kendi-denemeni-ekleme)).
- Her soruyu çözünce yapay zekâ **her şıkkın** ayrıntılı analizini verir.
- **Kalıcı hafıza** (spaced repetition) sistemiyle öğrendiğini unutmadan tutmanı sağlar.
- İlaç kartları, performans analizi, TUS simülatörü, yeni nesil soru üretimi ve daha fazlası.
- Tüm verin senin bilgisayarında kalır; yapay zekâ senin **ücretsiz** anahtarınla çalışır.

## 2. Kurulum

### 🍎 macOS
1. İndirdiğin `.dmg` dosyasına çift tıkla.
2. Açılan pencerede **TusMaster** simgesini **Applications** klasörüne sürükle-bırak.
3. İlk açılışta: Applications'ta TusMaster'a **sağ tık → "Aç" → tekrar "Aç"**. (Apple noter onayı henüz yapılmadığı için bu uyarı normaldir; yalnızca ilk seferde.)

### 🪟 Windows
1. İndirdiğin `.zip` dosyasını bir klasöre çıkar (sağ tık → *"Tümünü ayıkla"*).
2. Klasördeki **`TusMaster.exe`** dosyasına çift tıkla.
3. *"Windows bilgisayarınızı korudu"* çıkarsa: **Ek bilgi → Yine de çalıştır**.
4. `TusMaster.exe` ile **`_internal`** klasörünü aynı yerde tut, ayırma/silme.

> İlk açılış birkaç saniye sürebilir (uygulama veritabanını hazırlıyor). Uygulama kendi penceresinde açılır.

## 3. İlk açılış sihirbazı
İlk açılışta 2 adımlık karşılama ekranı gelir:

**Adım 1 — Sözleşme:** Kullanım koşullarını oku ve kabul et.

**Adım 2 — Ücretsiz Gemini anahtarı:**
- https://aistudio.google.com/apikey adresinden Google hesabınla ücretsiz anahtar al (*Create API key*).
- Anahtarı kutuya yapıştır → **"Kaydet ve Başla"**.

Bu ekranda şu uyarılar çıkar (hepsini okumanı öneririz):
- 🚫💳 **Kredi kartı girme** — Gemini ücretsizdir; kart/ödeme isteyen bir sayfa çıkarsa doldurma, kapat.
- 💡 **Kotanı katla** — farklı Google hesaplarından birkaç anahtar alıp her satıra bir tane yapıştırabilirsin (biri dolunca otomatik diğerine geçer).
- 🔋 **Ücretsiz API kotalıdır** — yoğun kullanımda yapay zekâ kısa süre durabilir; arıza değildir.
- 📝 **Çıkmış sorular hazır gelmez** — kendi sorularını sen eklersin ([bölüm 13](#13-kendi-denemeni-ekleme)).

## 4. Ekranı tanıyalım
Sol taraftaki menüden bölümlere geçersin:
- **Soru Bankası** — tüm soruları gez/filtrele.
- **Soru Çöz** — çözme ekranı (rastgele karışım da buradan açılır).
- **Bugünün Planı** — günlük tekrar + zayıf konu karışımı (yanında 🧠 kaç tekrar olduğunu gösteren rozet çıkar).
- **Yıldızlı Sorular**, **İlaç Kartları**.
- **ANALİZ:** Performans, Zayıf Analiz, Sınav Karnem.
- **TEKRAR:** Hata Havuzu, Notlarım.
- **İçerik & Kaynak**, **Ders Havuzu**, **TUS Simülatörü**, **Yeni Nesil Sorular**, **AI Araçları** (açılır bölümler).
- Sağ üstte: 🌙/☀️ gece/gündüz düğmesi.

## 5. Soru çözme
1. Bir soruda şıklardan birine tıkla.
2. Doğru/yanlış anında belli olur; yapay zekâ **"Çözüm & Analiz"** ile her şıkkın neden doğru/yanlış olduğunu açıklar.
3. Şık üstüne gelince (hover) o şıkka özel kısa açıklama çıkar.
4. Soru altında ek araçlar:
   - 🧠 **Hafıza butonları** (Yine / Zor / İyi / Kolay) → bkz. [bölüm 6](#6--kalıcı-hafıza-srs).
   - 👍/👎 **geri bildirim** — soru hatalıysa işaretle (çok 👎 alan soru otomatik gizlenir).
   - 📝 **Not** — soruya kişisel not ekle.
   - ⭐ **Yıldızla** — sonra kolay bulmak için.
5. Üstteki *"Soru X/Y"* yanındaki arama kutusuna numara yazıp istediğin soruya atlayabilirsin (uzun denemelerde pratik).
6. Çözerken yan panelden **Analiz / Textbook (konu anlatımı) / İlgili Makaleler** açabilirsin (aynı anda biri görünür).

## 6. 🧠 Kalıcı Hafıza (SRS)
En değerli özellik. *"Spaced repetition"* (aralıklı tekrar), bilimsel olarak en güçlü kalıcı-öğrenme yöntemidir.

**Nasıl çalışır:**
- Bir soruyu çözdükten sonra çıkan *"Bunu ne kadar iyi hatırladın?"* kutusundan birini seç:
  - **Yine** → bilemedim/yanlış → yarın tekrar gelir.
  - **Zor** → zor hatırladım → kısa aralıkla gelir.
  - **İyi** → hatırladım → aralık büyür (1→3→8 gün…).
  - **Kolay** → çok kolaydı → aralık daha hızlı büyür.
- Her butonun üstünde *"kaç gün sonra döner"* önizlemesi yazar.
- Soru, seçtiğin zorluğa göre tam unutmaya yakın tekrar karşına çıkar → **kalıcı öğrenme**.

**Nerede görürüm:**
- Performans sayfasında **🧠 Tekrar Takvimi** kartı: bugün kaç kart vadesi geldi + önümüzdeki 7 gün + *"▶ N kartı tekrar et"*.
- Sol menüde Bugünün Planı yanında **🧠 N tekrar** rozeti.

> 💡 İpucu: Her gün önce "vadesi gelen tekrarları" bitir, sonra yeni soru çöz. Günlük 15–20 dakikalık tekrar, maraton çalışmadan kalıcıdır.

## 7. Bugünün Planı
O gün için akıllı bir karışım hazırlar: tekrar zamanı gelen sorular + geçmişte yanlış yaptıkların + birkaç yeni keşif. *"Bugün ne çalışayım?"* derken buradan başla.

## 8. TUS Simülatörü
Gerçek TUS formatında tam deneme: **Temel Bilimler** ve **Klinik Bilimler** olarak ders dağılımına uygun soru seçer, kronometre çalışır, bitince karneye işlenir. Sınav provası için idealdir.

## 9. İlaç Kartları
Her ilaç için: sınıf, mekanizma, **endikasyon** (yeşil), **kontrendikasyon** (kırmızı uyarı), yan etkiler, TUS tuzağı.
- Karta tıklayınca **🔬 Detaylı Analiz**'i açabilirsin → yapay zekâ derin monograf üretir (farmakokinetik, etkileşimler, özel popülasyonlar, TUS incileri). İlk üretim birkaç saniye sürer, sonra kayıtlı gelir.

## 10. Analiz
- **Performans** — özet kartlar (çözülen, başarı, süre), ders bazlı başarı grafiği, zaman serisi, Tekrar Takvimi ve en zayıf konular.
- **Zayıf Analiz** — en düşük başarılı konuların sıralı listesi; *"🚀 Zayıflarımı Çöz"* ile hepsinden odaklı tekrar seti başlatır.
- **Sınav Karnem** — çözdüğün denemelerin geçmişi (tarih, doğru/yanlış/boş, süre).

> Not: Bu ekranlardaki sayılar **soru sayısıdır** (kaç soru çözdüğün/denediğin).

## 11. Tekrar
- **Hata Havuzu** — yanlış yaptığın sorular; *"bu sefer tutuyor musun?"* diye tekrar dene.
- **Notlarım** — soruya eklediğin kişisel notların tek listede.
- **Yıldızlı Sorular** — yıldızladıkların.

## 12. Yapay zekâ araçları
- **Yeni Nesil Sorular** — istediğin konu/zorlukta yapay zekânın ürettiği taze sorular.
- **Vaka Simülatörü** — yapay zekâ gerçekçi bir klinik vaka sunar, sen karar verirsin, AI değerlendirip bir sonraki aşamayı açar.
- **İlgili Makaleler** — sorunun konusuyla ilgili tıbbi kaynak/araştırma bağlantıları (*bu özellik kota harcamaz*).
- **Textbook** — sorunun konusunun kısa, odaklı anlatımı.

> Bu araçların çoğu Gemini kotanı kullanır; *"İlgili Makaleler"* kullanmaz.

## 13. Kendi denemeni ekleme
Gerçek çıkmış sorular telif nedeniyle gelmez; kendi PDF'lerini ekleyebilirsin:
1. **İçerik & Kaynak** bölümünden deneme/soru PDF'ini yükle.
2. Uygulama metni tarar, soruları ayıklar, derslere yerleştirir.
3. Reklam/boş sayfa görselleri otomatik elenir (örn. dershane reklamları soru görseli sanılmaz).
4. Tarama mükemmel değildir — eklenen soruları gözden geçir; eksik/yanlış varsa düzeltebilir veya çıkarabilirsin.

## 14. API anahtarı & kota yönetimi
- Yapay zekâ senin **ücretsiz** Gemini anahtarınla çalışır; anahtar yalnızca bu bilgisayarda saklanır.
- **Kota:** Ücretsiz anahtarın dakikalık/günlük sınırı vardır. Dolunca yapay zekâ özellikleri kısa süre *"kota doldu"* der (sorular/çözmeye devam edebilirsin; sadece AI üretimi bekler).
- **Çoklu anahtar:** Birden fazla anahtar girersen (farklı Google hesapları) biri dolunca uygulama otomatik diğerine geçer → kotanı çok katlarsın.
- **Asla kredi kartı girme** — ücretsiz katman yeterli.

## 15. Yedekler, verilerin ve gizlilik
- İlerleyişin, notların, eklediğin sorular ve tekrar takvimin bilgisayarındaki **yerel** veritabanında tutulur.
- Uygulama otomatik **günlük yedek** alır; bir sorun olursa eski hâle dönülebilir.
- **Gizlilik:** Soruların ve verilerin senin bilgisayarından dışarı gönderilmez. Yalnızca yapay zekâ analizinde, ilgili sorunun metni senin anahtarınla doğrudan Google Gemini'ye gider. Anahtarın kimseyle paylaşılmaz.

## 16. Tema, sayaç ve küçük ayarlar
- Sağ üstten gece/gündüz modunu değiştir (gündüz ☀️ güneş, gece 🌙 ay).
- Rastgele deneme/Günün Havuzu modunda *"Sınavı Bitir"*in yanında kronometre çalışır; bitirince süre karneye işlenir.

## 17. Çalışma ipuçları
- Her gün **önce tekrarları bitir** (Tekrar Takvimi/Bugünün Planı), sonra yeni soru çöz. Tutarlılık > maraton.
- Hafıza butonlarını **dürüst** kullan — *"Kolay"* dediğin soru uzun süre gelmez; emin değilsen *"Zor"/"Yine"* de ki sık sık karşına çıksın.
- **Yanlışlarını sahiplen** — Hata Havuzu + Zayıf Analiz, en çok puan kazandıracağın yer.
- AI analizini **anladığından emin ol**; sadece okuyup geçme — aktif hatırlama kalıcılığı artırır.

## 18. Sorun giderme
- **mac "açılamıyor" diyor** → Applications'ta sağ tık → "Aç" → "Aç".
- **Windows açılmıyor** → `TusMaster.exe` ile `_internal` klasörü aynı yerde mi? ZIP'i tam çıkardın mı? SmartScreen'de "Yine de çalıştır" dedin mi?
- **Yapay zekâ cevap vermiyor / "kota doldu"** → biraz bekle ya da ikinci bir ücretsiz anahtar ekle. İnternet bağlantını kontrol et.
- **Çözülemeyen sorun** → 🐞 Sorun Bildir ya da myny061955@gmail.com.

## 19. ⚠️ Tıbbi sorumluluk
TusMaster bir çalışma/öğrenme aracıdır. Yapay zekâ ara sıra hatalı veya eksik bilgi üretebilir (halüsinasyon). Tüm bilgileri güncel ve güvenilir tıbbi kaynaklarla doğrula. Buradaki hiçbir içerik tıbbi tanı, tedavi veya hasta bakımı tavsiyesi değildir; gerçek klinik kararlar için resmi kaynaklara ve uzman görüşüne başvur.

**Başarılar! 🎯**
