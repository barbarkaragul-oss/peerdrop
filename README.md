<div align="center">

# ⚡ PeerDrop Pro v4.1 — Universal Adaptive P2P Stream Room
### **Uncompressed 4K/8K Video & 100GB+ File Transfer • WhatsApp-Style P2P Chat • Mobile Quota Shield**

[![Version](https://img.shields.io/badge/Release-v4.1_Universal-00a884?style=for-the-badge)](https://github.com/barbarkaragul-oss/peerdrop/releases)
[![Speed](https://img.shields.io/badge/Adaptive_Engine-16_Mbps_ADSL_%E2%86%94_1000_Mbps_Fiber-f59e0b?style=for-the-badge)](#%EF%B8%8F-universal-adaptive-gear-engine-bbr-style-pacing)
[![Security](https://img.shields.io/badge/Integrity-SHA256_%2B_Ed25519-38bdf8?style=for-the-badge)](#-cryptographic-security--ed25519-pro-licensing)
[![Languages](https://img.shields.io/badge/i18n-TR_%7C_EN_%7C_DE_%7C_RU_%7C_ES_%7C_FR-8b5cf6?style=for-the-badge)](#-auto-region-multi-language-engine-6-languages)

**Zero Cloud Storage Cost • No Receiver App Required • Instant LAN & Global Cloudflare HTTP/2 Tunnel**

[🇹🇷 Türkçe Rehber & Tüm Özellikler](#-türkçe-genel-bakış-ve-tüm-özellikler) • [🇬🇧 English Overview & Features](#-english-overview--all-features) • [📥 Download / İndir (Windows x64)](./PeerDrop-v4.1-Windows-x64.zip)

</div>

---

## 🇹🇷 Türkçe Genel Bakış ve Tüm Özellikler

**PeerDrop Pro v4.1**, telefonlar (Android / iPhone) ve bilgisayarlar arasında **bulut sunucularına tek kuruş ödemeden**, kalite kaybı olmadan **100 GB+ boyutta 4K/8K videoları**, fotoğrafları ve klasörleri doğrudan cihazdan cihaza (P2P) aktaran **kalıcı bir WhatsApp tarzı sohbet ve dosya odasıdır.**

Karşı tarafın telefonuna veya bilgisayarına **hiçbir uygulama kurmasına veya üyelik açmasına gerek yoktur.** WhatsApp veya SMS üzerinden gönderdiğiniz tek bir linke tıklayan alıcı, doğrudan sizin cihazınızla yüksek hızlı şifreli bağlantı kurar.

---

### 🚀 Neden PeerDrop? (Rakiplerle Karşılaştırma Tablosu)

| Özellik | ⚡ **PeerDrop Pro v4.1** | **Blip** | **LocalSend** | **SendAnywhere** | **WhatsApp / Telegram** |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Karşı Tarafa Uygulama Kurma Zorunluluğu** | **Yok (Tek Link / QR ile Tarayıcıdan Çalışır)** | Zorunlu (Hesap + App Şart) | Zorunlu | Yok (Reklamlı) | Zorunlu |
| **Farklı Ağlarda (4.5G / Şehirler Arası) Çalışma** | **Evet (Cloudflare HTTP/2 Küresel Tünel)** | Evet | **Hayır (Sadece Aynı Wi-Fi)** | Evet (Kotalı) | Evet |
| **Kalıcı Sohbet Odası & Pano (Link/Metin) Akışı** | **Evet (WhatsApp Tarzı Çift Yönlü Oda)** | Hayır | Hayır | Hayır | Evet |
| **Video Kalite Kaybı & Boyut Sınırı** | **Sıfır Sıkıştırma / Sınırsız (100 GB+)** | Sınırsız | Sınırsız | Ücretsizde Kotalı | **2 GB–4 GB Sınır & Kalite Bozulur** |
| **Mobil Veri Kota Kalkanı & Wi-Fi Bekletme Kuyruğu** | **Evet (Otomatik Wi-Fi Kuyruğu)** | Hayır | Hayır | Hayır | Hayır |
| **16 Mbps ADSL ↔ 1000 Mbps Fiber Otomatik Vites** | **Evet (64 KB Pacing ↔ 4 MB Turbo Blok)** | Kısmi | Sabit | Sabit | Sabit |

---

### 🎥 1. Süper Hızda Video ve Büyük Dosya Transfer Mimarisi

Standart web tarayıcıları büyük bir video gönderirken veya indirirken dosyayı önce telefonun RAM belleğinde (`Blob`) biriktirmeye çalışır ve 2–3 GB sonrasında tarayıcı sekmesi çöker. **PeerDrop v4.1** bu engeli **Doğrudan Diske Atomik Yazma (`WriteAt` + `.part` Kalkanı)** mimarisiyle aşar:

1. **Sıfır Sıkıştırma (Orijinal 4K/8K Ham Kalite):** Telefon kamerasıyla çekilen yüksek bit hızlı `.mp4` / `.mov` videolar, tek bir pikseli bile sıkıştırılmadan orijinal kalitesiyle saniyeler içinde bilgisayara veya diğer telefona akar.
2. **`.part` Geçici Dosya Kalkanı (`0 KB` Bozuk Dosya Koruması):** Yüklenen videolar aktarım sırasında `.part` uzantısıyla izole edilir; sadece %100 tamamlanıp **SHA-256 kriptografik özeti** doğrulandığında gerçek dosyaya dönüştürülüp sohbet ekranına düşer.
3. **Sürükle-Bırak, Yapıştır (`Ctrl+V`) ve Çoklu Seçim:** Bilgisayarda istediğiniz kadar videoyu veya dosyayı doğrudan sohbet ekranına sürükleyip bırakabilir, kopyaladığınız ekran görüntülerini `Ctrl+V` ile yapıştırabilir veya telefondaki **📎 Ataş** ikonundan galerinizdeki videoları toplu seçebilirsiniz.
4. **Aynı Wi-Fi Ağında Gigabit Hız (50–100+ MB/sn):** Cihazlar aynı modemdeyken (Ev/Ofis Wi-Fi) veriler dış internete çıkmadan yerel ağ üzerinden maksimum donanım hızıyla uçurulur.

---

### ⚙️ 2. Evrensel Adaptif Vites Motoru (16 Mbps ADSL ↔ 1000 Mbps Fiber)

Her kullanıcının internet altyapısı aynı değildir. 16 Mbps ADSL veya 2 diş çeken zayıf bir 4.5G hattında büyük paketler gönderilirse modemin yükleme kuyruğu şişer (**Bufferbloat**) ve bağlantı kopar. **PeerDrop v4.1**, her parçanın gidiş süresini milisaniye bazında ölçerek paket boyutunu ve nefes alma boşluğunu (**Pacing**) canlı olarak ayarlar:

| Kullanıcının Bağlantı Kalitesi | Ölçülen Anlık Hız | Otomatik Seçilen Vites (Paket Boyutu) | Modem Dinlendirme Boşluğu (Pacing) | Sağladığı Avantaj |
| :--- | :--- | :--- | :--- | :--- |
| **Zayıf 4.5G / 16 Mbps ADSL** | `< 300 KB/sn` | **`[ADSL/4.5G Safe 64KB]`** | **45 ms** | Modemi asla boğmaz, tüneli düşürmez (`Error 1033` önlenir), zaman aşımı vermeden %100 tamamlar. |
| **Standart VDSL / Normal 4.5G** | `300 KB/sn – 3 MB/sn` | **`[VDSL/4.5G 512KB]`** | **15 ms** | Dosya akarken aynı anda sohbet mesajlarının takılmadan gitmesini sağlar. |
| **Hızlı Fiber / 5G Mobil** | `3 MB/sn – 15 MB/sn` | **`[Fiber 2MB]`** | **0 ms** | Küresel Cloudflare HTTP/2 tünelini tam kapasiteyle doldurur. |
| **1000 Mbps Gigabit / Yerel Wi-Fi** | `> 15 MB/sn` | **`[Gigabit Turbo 4MB]`** | **0 ms** | Büyük video dosyalarını saniyeler içinde tam hızda aktarır. |

* **Hareket Sensörlü Zaman Aşımı (Stall-Only Watchdog):** Sabit süre sınırı yoktur. Bağlantı çok yavaş olsa bile veri aktığı sürece aktarım **asla** kesilmez. Sadece hat tamamen kopup 28 saniye boyunca tek bir bayt bile ilerlemezse otomatik olarak kaldığı ofsetten (`Auto-Resume`) yeniden dener.

---

### 🛡️ 3. Akıllı Mobil Veri (Kota) Kalkanı ve Wi-Fi Bekletme Kuyruğu

Dışarıda 4.5G/5G mobil veri kullanırken birisi size 40 GB'lık bir video gönderdiğinde yanlışlıkla indirip mobil internet paketinizi bitirmenizi önleyen **3 Kademeli Kota Kalkanı** bulunur:

* **🤖 Akıllı Sor Modu:** Dosya 20 MB'tan büyükse veya cihazınız hücresel verideyse kırmızı **`⚠️ MOBİL VERİ (KOTA) UYARISI!`** penceresi açılır ve harcanacak net GB/MB miktarını gösterir.
* **⏳ Wi-Fi Ağına Bağlanana Kadar Beklet:** Tek tıkla dosyayı **Wi-Fi Bekleme Kuyruğuna** alabilirsiniz. Mobil verinizden **1 bayt bile harcanmaz**; akşam eve gelip telefonunuz Wi-Fi ağına bağlandığı saniye kuyruktaki tüm videolar otomatik olarak inmeye başlar.
* **📱 4.5G İzinli Mod:** Acil durumlarda uyarıları atlayarak doğrudan mobil veriden indirmeye izin verir.

---

### 📌 4. Sıfır-QR "Kalıcı Giriş" (Otomatik Tünel Bulucu & Error 1033 Kalkanı)

Ücretsiz küresel tüneller bilgisayar her kapanıp açıldığında güvenlik gereği yeni bir `trycloudflare.com` adresi alır. Her gün yeniden QR kod okutma zahmetini bitirmek için **PeerDrop v4.1** içinde çift katmanlı kurtarıcı bulunur:

1. **Sabit Oda Kimliği (`PD-XXX-XXX`) & MQTT Feneri:** Bilgisayarınızdaki `peerdrop.exe` açıldığı saniyede, o gün aldığı yeni Cloudflare HTTP/2 tünel adresini ve yerel Wi-Fi IP adresini şifreli olarak sabit oda kimliğinize yayınlar.
2. **Tek Tıkla Kalıcı Giriş Dosyası (`PeerDrop-PD-XXX-XXX.html`):** Üst bardaki **`📌 Kalıcı Giriş`** butonundan telefonunuza indirdiğiniz 3 KB'lık başlatıcıya dokunduğunuzda, bilgisayarınız hangi yeni tünel adresini almış olursa olsun **1 saniye içinde otomatik bulur ve sizi doğrudan sohbet odasına yönlendirir.**
3. **Canlı Sekme Kurtarıcı:** Sohbet ekranı açıkken tünel yenilenirse tarayıcı `Error 1033` ekranında kalmaz; arka planda yeni tüneli keşfedip sayfayı otomatik olarak yeni adrese taşır.

---

### 🌍 5. Bölgeye Göre Otomatik Değişen 6 Dilli Küresel Arayüz (i18n)

Uygulama açıldığı cihazın **saat dilimini (`Intl.DateTimeFormat`)** ve **sistem dilini (`navigator.language`)** otomatik tespit ederek kendi dilinde açılır; ayrıca sağ üstteki dil kutusundan anlık olarak değiştirilebilir:
* 🇹🇷 **Türkçe** (`Europe/Istanbul`)
* 🇬🇧 **English** (Global Default)
* 🇩🇪 **Deutsch** (`Europe/Berlin`, `Vienna`, `Zurich`)
* 🇷🇺 **Русский** (`Europe/Moscow`, `Minsk`, `Almaty`)
* 🇪🇸 **Español** (`Europe/Madrid`, `America/Mexico_City`, `Buenos_Aires`)
* 🇫🇷 **Français** (`Europe/Paris`, `Brussels`)

---

### 🔐 6. Kriptografik Güvenlik ve Ed25519 Pro Lisanslama

* **Uçtan Uca SHA-256 Doğrulaması:** Gönderilen her video ve dosyanın bit düzeyinde `SHA-256` parmak izi hesaplanır; tek bir bit bile bozulmuşsa sistem bunu anında yakalar.
* **Ed25519 Dijital İmza Koruması:** Pro lisans anahtarları (`PDPRO-MUSTERI-...`), 64-baytlık eliptik eğri (`crypto/ed25519`) dijital imzasıyla doğrulanır ve taklit edilemez.

---

### 🛠️ Hızlı Kurulum ve Video Gönderim Rehberi (30 Saniye)

1. **[PeerDrop-v4.1-Windows-x64.zip](./PeerDrop-v4.1-Windows-x64.zip)** paketini indirin ve masaüstünde bir klasöre çıkarın.
2. Klasörün içindeki **`peerdrop.exe`** dosyasına çift tıklayın *(Uygulama otomatik olarak donanım öz-denetimini yapar, küresel Cloudflare HTTP/2 tünelini açar ve sohbet penceresini başlatır)*.
3. Sağ üstteki turuncu **`📱 QR Okut`** butonuna tıklayın:
   * **Aynı Ev/Ofis İçindeyseniz:** **`📶 Yerel Wi-Fi (Maksimum Hız)`** sekmesindeki QR kodu telefonunuzla okutun.
   * **Dışarıdaysanız (4.5G / Farklı Şehir):** **`🌍 Küresel (4.5G / Her Yer)`** sekmesindeki QR kodu okutun veya **`🔗 Link Gönder`** butonuyla WhatsApp'tan arkadaşınıza atın.
4. Telefonunuzda veya bilgisayarınızda **📎 Ataş** ikonuna dokunup istediğiniz boyuttaki videoyu seçin; üstteki canlı hız çubuğundan (`MB/s` ve aktif vites `[...]`) akışı anlık izleyin!

---

## 🇬🇧 English Overview & All Features

**PeerDrop Pro v4.1** is a self-hosted, zero-cloud-cost P2P file streaming and persistent WhatsApp-style chat room engineered for **uncompressed 4K/8K videos and 100GB+ files**.

* **Zero App Required for Receivers:** Share a single link via WhatsApp/SMS or scan a QR code. The recipient connects directly to your device via browser over local Gigabit Wi-Fi or a global Cloudflare HTTP/2 tunnel.
* **Universal Adaptive Gear Engine (64KB ↔ 4MB):** Automatically senses link capacity on every chunk. Uses `64 KB` micro-chunks with `45ms` anti-bufferbloat pacing on weak 16 Mbps ADSL / 4G connections to prevent tunnel drops (`Error 1033`), and scales up to `4 MB` Turbo blocks on Gigabit Wi-Fi.
* **Smart Mobile Data Quota Shield:** Prevents accidental cellular data exhaustion on large files (`>20 MB`) and lets mobile users queue downloads (`⏳ Queue for Wi-Fi`) until they reconnect to Wi-Fi.
* **Zero-QR Auto-Pass Beacon:** Remembers your permanent Room ID (`PD-XXX-XXX`) and automatically routes mobile devices to your latest Cloudflare tunnel address after PC restarts.
* **6-Language Auto-Region UI:** Automatically adapts to Turkish, English, German, Russian, Spanish, or French based on device timezone and locale.

---

<div align="center">
  <b>Developed by Barbaros Karagülmez (@barbarkaragul-oss)</b><br>
  <i>High-Performance Systems & P2P Network Engineering</i>
</div>