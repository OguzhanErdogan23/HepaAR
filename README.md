## Oğuzhan Erdoğan - 215541014

## 🎥 Proje Tanıtım ve Demo Videosu



https://github.com/user-attachments/assets/c97ccb15-19dc-4fb1-8ce1-548e053b0b3d



# HepaAR — Karaciğer Nakli Hastaları İçin AR Destekli İmmünosüpresif İlaç Uyum Takip Uygulaması

## 1. Proje Başlığı

**HepaAR: Karaciğer Nakli Hastalarına Yönelik Artırılmış Gerçeklik (AR) Destekli İmmünosüpresif İlaç Uyum Takibi**

Yazılım Mühendisliğinde Güncel Konular (YMGK) dersi projesidir.
Hedef: TÜBİTAK Teknoloji Hazırlık Seviyesi THS-7 (gerçek operasyonel ortamda çalışan prototip — fiziksel Android cihaz).

---

## 2. Proje Özeti

HepaAR, karaciğer nakli sonrası ömür boyu immünosüpresif ilaç kullanması gereken hastaların ilaç uyumunu artırmak amacıyla geliştirilmiş, **artırılmış gerçeklik (AR)** ve **oyunlaştırma** teknolojilerini bir arada kullanan bir mobil sağlık (mHealth) uygulamasıdır.

Uygulama, hastaların ilaçlarını doğru zamanda ve doğru dozda almalarını sağlamak için akıllı hatırlatmalar, QR kod ile ilaç doğrulama, AR tabanlı interaktif karaciğer modeli ve klinik düzeyde uyum analitiği sunar. Çocuk, yetişkin, ebeveyn-bakıcı ve doktor olmak üzere **dört farklı kullanıcı modunu** destekler.

---

## 3. Problem Tanımı

Karaciğer nakli sonrasında hastaların organ reddini önlemek için immünosüpresif ilaçları ömür boyu düzenli kullanması hayati önem taşır. Ancak mevcut durumda:

- Nakil hastalarının **%17–51'i** immünosüpresif ilaç uyumsuzluğu yaşamaktadır (PMC10510935).
- En yaygın sorun doz atlamak değil, **zamanlama uyumsuzluğudur (%43)**; 2 saatten uzun gecikmeler organ red riskini önemli ölçüde artırmaktadır (PMC8869578).
- Geç akut rejeksiyonların yaklaşık **%25'i** ilaç uyumsuzluğu ile ilişkilidir (EASL 2024).
- Mevcut dijital sağlık araçlarının kullanım oranı ilk yılda **%59'a** gerilemektedir (PMID 33682207).

Bu veriler, hastaların ilaç uyumunu artırmaya yönelik daha etkili, etkileşimli ve sürdürülebilir bir dijital çözüme ihtiyaç olduğunu ortaya koymaktadır.

---

## 4. Amaçlar

- İmmünosüpresif ilaç uyumunu artırmak için AR ve oyunlaştırma teknolojilerini kullanan bir mobil uygulama geliştirmek.
- ±2 saatlik klinik uyum penceresine dayalı akıllı doz zamanlama motoru tasarlamak.
- 3B karaciğer modeli ile hastanın organ durumunu görselleştirmek ve farkındalık oluşturmak.
- QR kod tabanlı ilaç doğrulama sistemi ile yanlış ilaç alımını önlemek.
- Çocuk hastalar için oyunlaştırılmış deneyim sunarak uzun vadeli uygulama kullanımını teşvik etmek.
- Doktor paneli ile uzaktan hasta uyum takibi altyapısı sağlamak.
- Günlük his raporu ve kritik semptom bildirimi ile erken uyarı mekanizması kurmak.
- TÜBİTAK THS-7 seviyesinde gerçek cihazda çalışan bir prototip ortaya koymak.

---

## 5. Temel Kavramlar

| Kavram | Açıklama |
|--------|----------|
| **İmmünosüpresif İlaçlar** | Organ nakli sonrasında bağışıklık sistemini baskılayarak organ reddini önleyen ilaçlardır (Tacrolimus, Mycophenolate vb.). |
| **İlaç Uyumu (Adherence)** | Hastanın ilaçlarını reçeteye uygun dozda ve zamanda almasıdır. |
| **±2 Saat Uyum Penceresi** | Klinik rehberlere göre, immünosüpresif ilaçların planlanan saatten ±2 saat içinde alınması gerektiğini belirten standart. |
| **Artırılmış Gerçeklik (AR)** | Gerçek dünya görüntüsü üzerine dijital içeriklerin bindirilmesi teknolojisidir. |
| **ARCore / Scene Viewer** | Google'ın Android cihazlar için AR platformu ve 3B model görüntüleme aracıdır. |
| **Oyunlaştırma (Gamification)** | Oyun mekaniklerinin (puan, rozet, seviye) oyun dışı bağlamlarda motivasyonu artırmak için kullanılmasıdır. |
| **THS (Teknoloji Hazırlık Seviyesi)** | TÜBİTAK'ın teknolojilerin olgunluk düzeyini ölçmek için kullandığı 1-9 arası ölçektir. |
| **SUS (System Usability Scale)** | 10 soruluk standart kullanılabilirlik anketidir. |
| **Hive** | Flutter için hafif, offline-first yerel NoSQL veritabanıdır. |
| **Riverpod** | Flutter uygulamalarında reaktif durum yönetimi sağlayan bir kütüphanedir. |

---

## 6. Kullanılan Teknolojiler

| Kategori | Teknoloji | Açıklama |
|----------|-----------|----------|
| **Geliştirme Ortamı** | Flutter 3.x + Dart | Çapraz platform mobil uygulama çatısı |
| **Durum Yönetimi** | Riverpod | Reaktif state management |
| **Navigasyon** | GoRouter | Bildirimsel, rol bazlı yönlendirme |
| **Yerel Depolama** | Hive (hive_flutter) | Offline-first NoSQL veritabanı (6 kutu) |
| **AR / 3B Model** | model_viewer_plus | 3B model ve ARCore Scene Viewer entegrasyonu |
| **QR Kod** | mobile_scanner / qr_flutter | QR okuma ve QR üretimi |
| **Grafikler** | fl_chart | Uyum istatistikleri ve trend grafikleri |
| **Bildirimler** | flutter_local_notifications | Günlük ilaç hatırlatma bildirimleri |
| **Animasyonlar** | flutter_animate | Mikro animasyonlar ve geçiş efektleri |
| **Bulut (Opsiyonel)** | Firebase (Auth, Firestore, Messaging) | Opsiyonel bulut senkronizasyonu |
| **Diğer** | intl, uuid, permission_handler, equatable, image_picker | Lokalizasyon, benzersiz ID, izin yönetimi vb. |

---

## 7. Proje Kapsamı

### Kapsam İçi
- **AR Deneyimi:** 3B karaciğer modeli, anatomi turu, durum varyantları (sağlıklı/yağlanma/siroz/tümör/nakil sonrası), "Odanda Gör" AR yerleştirme.
- **İlaç Yönetimi:** İlaç ekleme/düzenleme/arşivleme, hızlı seçim listesi, QR kod üretimi ve tarama, doz onaylama.
- **Doz Zamanlama Motoru:** ±2 saatlik klinik uyum penceresi, durum makinesi (yaklaşıyor → şimdi al → alındı/geç/kaçırıldı/atlandı).
- **Bildirimler:** Günlük hatırlatmalar, exact/inexact alarm desteği, saat dilimi doğruluğu, cihaz yeniden başlatma sonrası yeniden kurulum.
- **Analitik:** Haftalık uyum halkası, 7 günlük trend grafiği, geçmiş ekranı (7/30 gün).
- **Çocuk Modu & Oyunlaştırma:** Puan sistemi, seviye, 7 rozet, bilgi quizi, "karaciğer arkadaşın" bakım oyunu.
- **Eğitim Modülü:** 6 ilaç prospektüsü, 5 klinik konu, çocuk/yetişkin içerik varyantları.
- **Doktor Paneli:** Klinik metrikler, 14 günlük trend, hasta dosyası, radyolojik görüntü takibi, kritik semptom uyarısı.
- **Günlük His Raporu:** Ruh hâli, semptom bildirimi, kritik semptom kuralları.
- **UX Ölçümü:** Gömülü SUS anketi (10 soru, standart skorlama).
- **Dört Kullanıcı Modu:** Çocuk, Yetişkin, Ebeveyn-Bakıcı, Doktor.

### Kapsam Dışı
- iOS platform desteği (şu aşamada yalnızca Android).
- Hastane bilgi sistemi (HIS) entegrasyonu.
- Klinik pilot çalışma ve gerçek hasta denemeleri.
- KVKK/GDPR tam uyum sertifikasyonu.
- Play Store yayınlama.

---

## 8. Beklenen Çıktılar

- THS-7 seviyesinde gerçek Android cihazda çalışan prototip uygulama (APK).
- AR destekli interaktif 3B karaciğer deneyimi.
- QR kod tabanlı ilaç doğrulama ve doz onay sistemi.
- Klinik standarda dayalı (±2 saat) ilaç uyum izleme motoru.
- Doktor klinik paneli ile uzaktan hasta takip altyapısı.
- Çocuk moduna özel oyunlaştırılmış sağlık eğitim deneyimi.
- Yerleşik SUS kullanılabilirlik anketi ile UX ölçüm verileri.
- Kapsamlı birim test altyapısı (69 test).
- Akademik sunuma yönelik THS-7 kanıt paketi (RAMS, SMART, STEAM, SWOT, THS raporu).

---

## 9. Katkıda Bulunanlar

| Rol | İsim |
|-----|------|
| **Geliştirici** | Oğuzhan Erdoğan |
| **Ders** | Yazılım Mühendisliğinde Güncel Konular (YMGK) |
| **Kurum** | Fırat Üniversitesi — Yazılım Mühendisliği |

---

## 10. Kaynaklar

1. **EASL Clinical Practice Guidelines on Liver Transplantation (2024)** — Avrupa Karaciğer Çalışmaları Derneği klinik rehberleri.
2. **PMC10510935** — İmmünosüpresif ilaç uyumsuzluk oranları meta-analizi.
3. **PMC8869578** — Zamanlama uyumsuzluğu ve organ red riski ilişkisi.
4. **PMID 33682207** — Dijital sağlık araçlarının uzun vadeli kullanım oranları.
5. **JMIR 2024 e56664** — Mobil sağlık uygulamalarında oyunlaştırma etkinliği.
6. **NCT05854472** — İlaç uyumu dijital müdahale klinik çalışması.

---

## 11. Anahtar Kelimeler

`Karaciğer Nakli` · `İmmünosüpresif İlaç Uyumu` · `Artırılmış Gerçeklik (AR)` · `Mobil Sağlık (mHealth)` · `Oyunlaştırma` · `Flutter` · `ARCore` · `İlaç Takibi` · `QR Kod Doğrulama` · `Hasta Eğitimi` · `THS-7`

---

## Çalıştırma

```bash
cd hepa_ar
flutter pub get
flutter run            # Fiziksel Android cihaz önerilir (AR için ARCore gerekli)
```

### Testler

```bash
flutter test           # 69 test: doz motoru, uyum, rozetler, SUS, bildirim, radyoloji, bakım oyunu
flutter analyze        # 0 issue
```

### APK Oluşturma

```bash
flutter build apk --debug    # veya --release
# build/app/outputs/flutter-apk/
```

---

## Mimari

```
Flutter 3.x + Riverpod (state) + GoRouter (navigasyon)
Hive (offline-first yerel depo, canlı box stream'leri)
model_viewer_plus (3D/AR — ARCore Scene Viewer) · mobile_scanner (QR)
fl_chart (grafikler) · flutter_local_notifications (hatırlatıcılar)
qr_flutter (ilaç QR üretimi) · flutter_animate (mikro animasyonlar)
```

Özellik bazlı klasörleme: `lib/features/<feature>/{models,services,providers,repositories,screens}`.
Saf Dart iş mantığı (`DoseScheduleEngine`, `AdherenceCalculator`, `BadgeRules`, `SusResponse`) UI'dan ayrık ve birim testli.

---

## ⚠️ Tıbbi Sorumluluk Reddi (Disclaimer)

Bu uygulama, akademik amaçlarla geliştirilmiş bir **öğrenci projesi prototipidir.** Uygulama içerisinde sunulan prospektüs bilgileri, hatırlatıcılar, uyum pencereleri ve semptom değerlendirmeleri klinik onaylı tıbbi tavsiye niteliği taşımamaktadır. Bu yazılım profesyonel bir tıbbi teşhis, tedavi veya doktor tavsiyesinin yerine kullanılamaz. İlaç dozajlarınız ve klinik süreçleriniz için her zaman kendi uzman hekiminizin ve transplant koordinatörünüzün yönlendirmelerini esas alınız.

---

## Lisans

Bu proje, Fırat Üniversitesi Yazılım Mühendisliğinde Güncel Konular dersi kapsamında akademik amaçlı geliştirilmiştir.
