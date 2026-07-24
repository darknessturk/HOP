# Hızlı Okuma Pro Android APK Projesi

Bu paket, mevcut `Hizli_Okuma_Pro_v10_4_5_Kitap_Baslangic_Focus_Fix.html` dosyanı Android WebView uygulaması olarak sarar.

## İçerik
- Uygulama adı: **Hızlı Okuma Pro**
- Paket adı: `com.akpa.hizliokumapro`
- Sürüm: `10.4.5`
- Ana içerik: `app/src/main/assets/index.html`
- WebView ayarları: JavaScript, localStorage, dosya seçici, kamera fotoğraf seçimi açık
- İnternet izni: OCR motoru CDN üzerinden yüklenebildiği için eklendi

## APK alma
1. Android Studio ile bu klasörü aç.
2. Gerekirse `compileSdk 35` yüklü değilse Android Studio yüklemeyi önerecektir.
3. Menüden **Build > Generate Signed App Bundle / APK** seç.
4. APK seç, keystore oluştur veya mevcut keystore kullan.
5. Çıktıyı telefona yükle.

## Hızlı debug APK
Terminalden, Android Studio Gradle kurulumuyla:

```bash
./gradlew assembleDebug
```

veya Android Studio içinden **Build > Build APK(s)**.

## Not
Bu ortamda Android SDK/Gradle kurulu olmadığı için gerçek `.apk` ikili dosyası burada derlenemedi. Proje APK üretmeye hazır olacak şekilde düzenlendi.

Kaynak HTML kelime adedi yaklaşık: 23673


## GitHub Actions ile otomatik APK
Projeyi GitHub'a yükleyip **Actions > Build Android APK > Run workflow** dediğinizde debug APK otomatik üretilir ve artifact olarak indirilebilir.
