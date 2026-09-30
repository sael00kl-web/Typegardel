# TypeGuard

## ساخت Keystore
```
keytool -genkey -v -keystore release.jks -keyalg RSA -keysize 2048 -validity 10000 -alias typeguard
base64 -w0 release.jks > ks.txt
```

## Secrets در GitHub
Settings → Secrets and variables → Actions:
- `KEYSTORE_BASE64` = محتوای ks.txt
- `KEYSTORE_PASSWORD`
- `KEY_ALIAS` = typeguard
- `KEY_PASSWORD`

## دانلود APK
تب Actions → آخرین اجرا → Artifacts → `TypeGuard-APKs`.

## فعال‌سازی
اپ را باز کن → دکمه «دسترسی‌پذیری» و «کیبورد» → TypeGuard را روشن کن.

فقط استفادهٔ شخصی.
