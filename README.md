# Cüzdan AI — Yasal Bilgi Sayfası

Bu repo Cüzdan AI: Bütçe & Birikim uygulamasının resmi gizlilik politikası ve kullanım şartlarını barındıran statik web sayfasıdır. GitHub Pages üzerinden yayınlanır.

## Yayınlama

1. GitHub'da `cuzdan-privacy` adında yeni public repo aç (https://github.com/new)
2. Bu klasörün içeriğini push'la:
   ```bash
   cd /Users/mertkan/cuzdan-privacy-site
   git init
   git add .
   git commit -m "Initial: gizlilik politikası + kullanım şartları"
   git branch -M main
   git remote add origin https://github.com/MertkanFirlar/cuzdan-privacy.git
   git push -u origin main
   ```
3. GitHub'da repo → Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, root → Save
4. 1-2 dakika sonra şu URL aktif olur:
   - **https://mertkanfirlar.github.io/cuzdan-privacy/**

## URL'leri

- Ana sayfa: https://mertkanfirlar.github.io/cuzdan-privacy/
- Gizlilik: https://mertkanfirlar.github.io/cuzdan-privacy/privacy.html
- Şartlar: https://mertkanfirlar.github.io/cuzdan-privacy/terms.html

## Güncelleme

Uygulama içi `PrivacyPolicyScreen.tsx` veya `TermsOfServiceScreen.tsx` değişirse
buradaki HTML'leri de paralel güncelle. Aynı metni iki yerde tutuyoruz çünkü:
- App Store / Play Store dış URL ister
- Kullanıcı offline'ken in-app version okuyabilsin
