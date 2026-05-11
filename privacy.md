# Lumoo Gizlilik Politikası

**Son güncelleme: 11 Mayıs 2026**

Bu gizlilik politikası, Lumoo uygulamasının ("Lumoo", "biz") topladığı verileri, nasıl kullandığını ve haklarını açıklar.

## Topladığımız veriler

### Hesap bilgileri
- **E-posta adresi**: kayıt ve giriş için. Sunucumuzda kullanıcı kimliğine bağlı şekilde saklanır.
- **Şifre**: bcrypt ile geri döndürülemez şekilde hash'lenir. Düz metin saklanmaz.

### Sağlık ve bebek bilgileri
- Bebeğin adı, doğum tarihi, cinsiyeti, doğum kilosu, anne adı, mascot tercihi
- Beslenme oturumları (süre, taraf, miktar, kategori)
- Sağılan süt kayıtları ve son kullanma tarihleri
- Pompa oturumları ve cluster pump fazları
- Büyüme ölçümleri (boy, kilo, baş çevresi)
- Bebek check-up notları

Bu veriler cihazında **AES-256-GCM** ile şifrelenerek saklanır. Sunucumuza giden bebek profili alanları da ayrıca AES-256-GCM ile şifrelenir.

### Kullanıcı içeriği (Lumoo'ya Sor — AI sohbet)
"Lumoo'ya Sor" sekmesinde yazdığın mesajların metni, sunucumuza gönderilir ve oradan AI yanıtı üretilmesi için **Anthropic, PBC** (Claude API) servisine iletilir.

**Gönderilen:** Yalnızca yazdığın mesajın metni.

**Gönderilmeyen:** Adın, e-posta adresin, bebek profili (ad, doğum tarihi, kilo vb.), beslenme/pompa kayıtların, cihaz tanımlayıcı (IDFA/IDFV), konum.

**Onay:** Bu özelliği ilk kez kullandığında uygulama içinde bir izin ekranı görürsün. Kabul etmeden hiçbir mesaj gönderilmez. Reddedersen sadece bu özellik devre dışı kalır; uygulamanın diğer bölümleri çalışır.

**Veri yaşam döngüsü:** Anthropic, API üzerinden gelen veriyi varsayılan olarak model eğitiminde kullanmaz ve 30 gün içinde siler.

### Reklamlar (yalnızca ücretsiz katmanda)
Lumoo, reklam gösterimi için **cihaz tanımlayıcısı (IDFA) kullanmaz**. Tüm AdMob reklam talepleri **kişiselleştirilmemiş (non-personalized)** olarak yapılır:

- Davranışsal hedefleme yapılmaz
- Kullanıcı profili oluşturulmaz
- Çapraz uygulama takibi yapılmaz
- iOS App Tracking Transparency (ATT) izin ekranı **gösterilmez** çünkü takip işlemi gerçekleşmez

Google'a yalnızca temel teknik bilgi iletilir (yaklaşık konum, cihaz dili, reklam yerleştirme ID'si). Premium abonelerde reklam tamamen kapalıdır.

### Satın alma geçmişi
- Premium aboneliğin durumu (aktif / iptal / yenileme tarihi). Apple App Store ve RevenueCat üzerinden alınır. Apple ID veya kart bilgilerin **hiçbir zaman Lumoo'ya iletilmez**.

## Verilerini nasıl kullanırız

- **Uygulama işlevi**: Bebek bakım takibinin sürdürülmesi, Lumoo'ya Sor (AI sohbet) yanıtlarının üretilmesi, abonelik yönetimi.
- **Reklam (sadece ücretsiz katmanda)**: AdMob aracılığıyla kişiselleştirilmemiş reklam gösterimi.
- **Yasal yükümlülükler**: Hukuki taleplere yanıt vermek için minimum gereken kadar.

## Üçüncü taraflarla paylaşım

Sağlık ve hesap verilerini reklam ortaklarıyla veya veri brokerlarıyla **asla paylaşmayız, satmayız**.

Aşağıdaki üçüncü taraf hizmetleri kullanılır. Her biri kendi gizlilik politikası altında Lumoo'nun standartlarına **eşdeğer veri koruma taahhüdü** verir:

- **Anthropic, PBC** (Claude API): Lumoo'ya Sor mesaj metni AI yanıtı için işlenir. Eğitim için kullanılmaz, 30 gün içinde silinir. [Gizlilik Politikası](https://www.anthropic.com/legal/privacy)
- **Apple StoreKit**: Ödeme işlemleri Apple tarafından yönetilir; biz kart bilgilerini görmeyiz. [Apple Gizlilik](https://www.apple.com/privacy/)
- **RevenueCat**: Abonelik durumu yönetimi. [RevenueCat Gizlilik](https://www.revenuecat.com/privacy/)
- **Google AdMob** (sadece ücretsiz katman): Kişiselleştirilmemiş reklam gösterimi. [AdMob Gizlilik](https://policies.google.com/technologies/partner-sites)
- **DigitalOcean**: Sunucu altyapısı (AB/ABD veri merkezi). [DigitalOcean Gizlilik](https://www.digitalocean.com/legal/privacy-policy)

## Haklarn

KVKK ve GDPR uyumlu:

- **Erişim ve dışa aktarma**: Profil → Veri Dışa Aktar üzerinden tüm verilerini PDF olarak indirebilirsin.
- **Silme**: Profil → Hesap → Hesabı Sil. Talep tarihinden itibaren 30 gün içinde tüm verilerin sunucularımızdan kalıcı silinir.
- **Düzeltme**: Bebek bilgilerini uygulama içinden düzenleyebilirsin.
- **Yapay zeka onayı**: "Lumoo'ya Sor" özelliğini kullanmadan önce uygulama içinde bir izin ekranı görürsün. Kabul etmezsen sadece bu özellik devre dışı kalır; uygulamanın diğer bölümleri çalışmaya devam eder.

## Veri saklama süreleri

- Hesap aktif olduğu sürece veriler saklanır.
- Hesap silme talebi sonrası 30 gün içinde tüm veriler kalıcı silinir.
- Yasal yükümlülükler nedeniyle daha uzun saklamamız gerekiyorsa (örn. fatura kayıtları), o veri ayrılır ve aktif kullanıma kapatılır.

## Çocukların gizliliği

Lumoo, anneler ve bebek bakıcıları içindir. 13 yaş altı çocuklardan bilerek veri toplamayız. Bebeğin bilgileri ebeveyn tarafından girilir ve ebeveyn sorumluluğundadır.

## Değişiklikler

Bu politikayı zaman zaman güncelleyebiliriz. Önemli değişikliklerde uygulama içinden bilgilendiririz.

## İletişim

Sorular ve veri işleme talepleri için: **support@lumoo.app**

Veri sorumlusu: Barış Fidan, Türkiye

---

# Lumoo Privacy Policy (English)

**Last updated: May 11, 2026**

This privacy policy explains what data Lumoo collects, how we use it, and your rights.

## Data we collect

### Account information
- **Email address**: for signup and login, stored linked to your user identity on our server.
- **Password**: irreversibly hashed via bcrypt. Plain text is never stored.

### Health and baby information
- Baby's name, birthdate, gender, birth weight, mother's name, mascot preference
- Feeding sessions (duration, side, amount, type)
- Pumped milk records and expiration dates
- Pumping sessions and cluster pump phases
- Growth measurements (height, weight, head circumference)
- Baby check-up notes

This data is encrypted on your device with **AES-256-GCM**. Baby profile fields that travel to our server are additionally encrypted with AES-256-GCM server-side.

### User content (Ask Lumoo — AI chat)
The text of the messages you write in the "Ask Lumoo" tab is sent to our server and then forwarded to **Anthropic, PBC** (Claude API) for AI response generation.

**Sent:** Only the text of your message.

**Not sent:** Your name, email, baby profile (name, birthdate, weight, etc.), feeding / pumping records, device identifier (IDFA/IDFV), location.

**Consent:** The first time you use this feature, you see an in-app consent screen. No message is sent without your explicit acceptance. Declining only disables this feature; the rest of the app continues to work.

**Data lifecycle:** Anthropic does not use API inputs to train models by default, and deletes them within 30 days.

### Advertising (free tier only)
Lumoo does **not use a device identifier (IDFA)** for ad serving. All AdMob ad requests are made as **non-personalized**:

- No behavioral targeting
- No user profile is built
- No cross-app tracking
- The iOS App Tracking Transparency (ATT) prompt is **not shown** because no tracking takes place

Google only receives basic technical info (approximate location, device language, ad slot ID). Premium subscribers see no ads at all.

### Purchase history
- Status of your Premium subscription (active / canceled / renewal date). Obtained via Apple App Store and RevenueCat. Your Apple ID and card details are **never sent to Lumoo**.

## How we use your data

- **App functionality**: Continuing baby care tracking, generating Ask Lumoo (AI chat) responses, managing your subscription.
- **Advertising (free tier only)**: Non-personalized ad serving via AdMob.
- **Legal compliance**: Responding to legal requests with the minimum data required.

## Sharing with third parties

We **never** share or sell your health or account data with advertising partners or data brokers.

The third-party services below are used. Each provides **equivalent data-protection guarantees** to Lumoo's standards under its own privacy policy:

- **Anthropic, PBC** (Claude API): Ask Lumoo message text is processed for AI responses. Not used for training, deleted within 30 days. [Privacy Policy](https://www.anthropic.com/legal/privacy)
- **Apple StoreKit**: Payment is handled by Apple; we do not see card details. [Apple Privacy](https://www.apple.com/privacy/)
- **RevenueCat**: Subscription status management. [RevenueCat Privacy](https://www.revenuecat.com/privacy/)
- **Google AdMob** (free tier only): Non-personalized ad serving. [AdMob Privacy](https://policies.google.com/technologies/partner-sites)
- **DigitalOcean**: Server infrastructure (EU/US data centers). [DigitalOcean Privacy](https://www.digitalocean.com/legal/privacy-policy)

## Your rights

GDPR and KVKK compliant:

- **Access and export**: Profile → Export Data downloads all your data as a PDF.
- **Deletion**: Profile → Account → Delete Account. All data permanently deleted from our servers within 30 days of request.
- **Correction**: Edit baby info within the app.
- **AI consent**: Before using "Ask Lumoo", an in-app consent screen is shown. If you decline, only this feature is disabled; the rest of the app continues to work.

## Data retention

- Data is retained while your account is active.
- Account deletion: all data permanently deleted within 30 days.
- If we are legally required to retain longer (e.g., billing records), that data is separated and not used actively.

## Children's privacy

Lumoo is for mothers and baby caregivers. We do not knowingly collect data from children under 13. Baby info is entered by the parent and is the parent's responsibility.

## Changes

We may update this policy occasionally. For significant changes, we'll notify you in-app.

## Contact

Questions and data requests: **barisfidann3@gmail.com**

Data controller: Barış Fidan, Turkey
