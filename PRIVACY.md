# EVroute Gizlilik Politikası ve KVKK Aydınlatma Metni

*Son güncelleme: 2 Ekim 2026* · [English version below](#evroute-privacy-policy)

Bu metin, EVroute mobil uygulamasını ("Uygulama") kullanırken hangi kişisel verilerinizin, hangi amaçla işlendiğini ve 6698 sayılı Kişisel Verilerin Korunması Kanunu ("KVKK") kapsamındaki haklarınızı açıklar.

## 1. Veri sorumlusu
**Mehmet Anıl ISLICIK** (EVroute geliştiricisi)
İletişim: **mehmetislicik@gmail.com**

## 2. İşlenen veriler
| Veri | Ne zaman | Nerede |
|---|---|---|
| **Destek kimliği** (rastgele kullanıcı kimliği) | Uygulama ilk açıldığında, giriş yapmasanız da | Firebase Authentication |
| **Hesap bilgileri**: e-posta, ad, profil fotoğrafı (Google ile girişte) | Hesap açtığınızda | Firebase Authentication |
| **Ayarlar ve yerler**: araç, şarj ve plan tercihleri, harita teması, favori yerler, son gidilen yerler (ad + koordinat) | Hesapla giriş yaptığınızda | Cloud Firestore (AB, eur3) |
| **Rota hesaplama kayıtları**: başlangıç ve varış (ad ve ~100 m'ye yuvarlanmış koordinat), araç, plan seçenekleri, kalkış zamanı, sonuç (mesafe, süre, duraklar, enerji, maliyet) veya hata, hesaplama süresi, uygulama sürümü, platform | Her "Rota planla"da | Cloud Firestore (AB, eur3) |
| **Konum** | Yalnızca "konumumu kullan", harita ve navigasyon sırasında | Cihazınızda; yalnızca rota hesaplamasının başlangıcı olarak gönderilir |

Navigasyon sırasında konum geçmişiniz **kaydedilmez**. Reklam, profil çıkarma veya üçüncü taraflarla pazarlama amaçlı paylaşım **yapılmaz**.

## 3. İşleme amaçları ve hukuki sebepler
- **Rota ve şarj planlama, navigasyon** — hizmetin sunulması (KVKK m.5/2-c, sözleşmenin ifası).
- **Ayarlarınızın ve yerlerinizin cihazlar arasında eşitlenmesi** — hesap açtığınızda, sözleşmenin ifası (m.5/2-c).
- **Hata giderme ve destek** (rota hesaplama kayıtları) — meşru menfaat (m.5/2-f): bir sorunu bildirdiğinizde ne olduğunu görebilmek.

## 4. Hizmet sağlayıcılar ve yurt dışına aktarım
Uygulama aşağıdaki hizmetleri kullanır. Bunlara, işin gerektirdiği en az veri gönderilir:

| Hizmet | Ne için | Gönderilen |
|---|---|---|
| Google Firebase (Google Ireland Ltd.) — Firestore AB (eur3) | Hesap, ayarlar, rota kayıtları | Yukarıdaki tablo |
| EVroute sunucusu (Render, Frankfurt) → OpenRouteService (HeiGIT, Almanya), Open Charge Map | Rota, şarj istasyonları | Rota noktaları (koordinat) |
| Photon (Komoot, Almanya) | Adres arama, haritada seçilen yerin adı | Aranan metin, seçilen koordinat |
| Open-Meteo (İsviçre) | Hava tahmini | Rota üzerindeki noktalar |
| OpenStreetMap Overpass | İstasyon çevresindeki yemek, WC vb. | İstasyon koordinatları |
| OpenFreeMap | Harita görüntüleri | Harita bölgesi, IP adresi (tüm web isteklerinde olduğu gibi) |
| GitHub | Güncelleme kontrolü ve indirme | IP adresi |

Bu sağlayıcıların bir kısmı Türkiye dışındadır. Kişisel verilerin yurt dışına aktarılması KVKK m.9 kapsamında gerçekleştirilir.

## 5. Saklama süreleri
- **Rota hesaplama kayıtları:** 90 gün, sonra silinir.
- **Hesap, ayarlar ve yerler:** Hesabınızı silene kadar.
- **Misafir (giriş yapılmamış) destek kimliği:** Uygulama silinene veya veriler temizlenene kadar.

## 6. Haklarınız (KVKK m.11)
Verilerinizin işlenip işlenmediğini öğrenme, bilgi isteme, düzeltilmesini veya silinmesini isteme, aktarıldığı üçüncü kişileri öğrenme, itiraz etme ve zararın giderilmesini isteme haklarına sahipsiniz.

- **Hesabınızı ve tüm verilerinizi** uygulamada **Hesap → Hesabı sil** ile silebilirsiniz. Ayarlar, yerler ve rota kayıtları birlikte silinir.
- Diğer talepleriniz için **mehmetislicik@gmail.com** adresine yazın. Uygulamadaki **Hesap → Destek kimliği**ni eklemeniz kaydınızı bulmamızı kolaylaştırır. Talepler en geç 30 gün içinde yanıtlanır.

## 7. Çocuklar
Uygulama 18 yaş altına yönelik değildir.

## 8. Değişiklikler
Bu metin güncellenebilir; güncel hâli her zaman bu sayfadadır.

---

# EVroute Privacy Policy

*Last updated: 2 October 2026*

**Controller:** Mehmet Anıl ISLICIK (developer of EVroute) · Contact: mehmetislicik@gmail.com

**What we process**
- A random **support ID** (Firebase user ID), created on first launch, even without signing in.
- **Account data** if you sign in: e-mail, name and profile photo (Google sign-in).
- **Settings and places** when signed in: vehicle, charging and plan options, map theme, favourite and recent destinations. Stored in Cloud Firestore (EU, eur3).
- **Route calculation logs** on every "Plan route": start and destination (name and coordinates rounded to ~100 m), vehicle, plan options, departure time, result or error, duration, app version, platform. Stored in Cloud Firestore (EU).
- **Location** only for "use my location", the map and navigation. It is sent only as the start of a route request; your location history is not stored.

There is no advertising, profiling or selling of data.

**Purposes:** route and charging planning and navigation, syncing your settings and places across devices, troubleshooting and support.

**Service providers:** Google Firebase (EU); our server (Render, Frankfurt) with OpenRouteService and Open Charge Map; Photon (Komoot); Open-Meteo; OpenStreetMap Overpass; OpenFreeMap; GitHub. Each receives only what it needs (coordinates, search text, IP address). Some of them are outside Türkiye.

**Retention:** route logs for 90 days; account, settings and places until you delete your account.

**Your rights:** delete your account and all its data in the app (**Account → Delete account**), or write to mehmetislicik@gmail.com with your support ID to access, correct or erase your data, or to object.
