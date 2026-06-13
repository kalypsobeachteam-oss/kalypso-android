# Kalypso Rezervasyon — Android

reservation.kalypsobeach.com.tr adresini tam ekran WebView olarak açar.

## Özellikler
- Tam ekran WebView
- Session/cookie kalıcılığı (login kaybolmaz)
- İnternet yok → offline ekranı + "Tekrar Dene"
- Back button → sayfa geçmişinde geri git
- Yükleme progress bar

## Android Studio ile Build

1. Android Studio'yu aç
2. "Open an existing project" → bu klasörü seç
3. Gradle sync tamamlandıktan sonra:
   - Debug APK: `Build > Build Bundle(s) / APK(s) > Build APK(s)`
   - Release APK için önce keystore oluştur (imzala)

## Komut satırından build (Android SDK gerekli)

```bash
./gradlew assembleDebug
# APK: app/build/outputs/apk/debug/app-debug.apk
```

## Minimum Gereksinim
- Android 7.0+ (API 24)
