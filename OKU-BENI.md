# Aile Bütçesi – Yayın Adımları

1. Klasörün tamamını HTTPS destekli bir yere yükleyin (GitHub Pages, Netlify, Cloudflare Pages). index.html kök dizinde olmalı.
2. privacy.html adresini kopyalayın ve içindeki [E-POSTA ADRESİNİZİ YAZIN] kısmını doldurun.
3. pwabuilder.com → site adresini girin → Package for stores → Android (Google Play).
   - Package ID: com.acamay.ailebutcesi · Name: Aile Bütçesi · Version: 1.0.0 (code 1)
   - Signing key: "New" seçin; indirilen .keystore dosyasını ve şifreleri GÜVENLİ SAKLAYIN (kaybederseniz güncelleme yapamazsınız).
4. İndirilen pakette gelen SHA-256 parmak izini .well-known/assetlinks.json içine yazın (şablon: .well-known-assetlinks.json.sablon) ve sitede /.well-known/assetlinks.json adresinden yayınlayın. Aksi halde uygulama üstte adres çubuğuyla açılır.
5. Play Console'a .aab dosyasını yükleyin; store/ klasöründeki ikon, kapak görseli ve magaza-aciklamalari.md metinlerini kullanın.
6. Not: Kayıt anahtarları eski sürümdeki (arslan_v8_*) gibi bırakıldı; mevcut verileriniz aynı adreste korunur. Adres değişirse önce Ayarlar'dan yedek alıp yeni uygulamada içe aktarın.
