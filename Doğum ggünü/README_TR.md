# Doğum Günü Sitesi (Hazır Paket)

Bu klasörü **GitHub Pages** veya **Netlify** ile doğrudan yayınlayabilirsiniz.

## 1) Kişiselleştirme
- `index.html` içindeki başlık otomatik olarak **?isim=Ayşe** gibi bir URL parametresiyle değişir.
  - Örnek: `https://kullanici.github.io/dogum-gunu/?isim=Ayşe`
- `assets/images/` klasöründeki `foto1.png` ve `foto2.png` dosyalarını kendi fotoğraflarınızla değiştirin.
- `assets/videos/` klasöründeki `video1.mp4` ve `video2.mp4` yerlerine kendi videolarınızı koyun.
  - iOS uyumluluğu için H.264/AAC kodlu `.mp4` kullanın.
  - Gerekirse ffmpeg komutu:
    ```bash
    ffmpeg -i input.mov -vcodec libx264 -acodec aac -movflags +faststart -preset veryfast -crf 23 output.mp4
    ```

## 2) Yayınlama (GitHub Pages)
1. GitHub hesabı açın (yoksa).
2. Yeni bir repo oluşturun (ör. `dogum-gunu`).
3. Bu klasördeki tüm dosyaları repoya yükleyin (root'a).
4. `Settings` → **Pages** → *Deploy from a branch* → `main` ve `/ (root)` seçin.
5. Kaydedin. Birkaç dakika sonra `https://<kullanici>.github.io/dogum-gunu/` adresinden açılır.

## 3) Yayınlama (Netlify - Sürükle Bırak)
1. Netlify hesabı açın.
2. `Add new site` → `Deploy manually` adımını seçin.
3. Bu klasörü `.zip` yapıp sayfaya sürükleyin veya klasörü yükleyin.
4. Verilen URL'yi paylaşın.

## 4) İpuçları
- Görselleri 1600px genişlik civarında tutmak hız kazandırır.
- Dosya adlarında **boşluk** yerine `-` kullanın (ör. `dogum-gunu-2025.png`).
- Videoların otomatik başlaması mobil tarayıcılarda kısıtlıdır; **controls** açık kalsın.
- Gizlilik: Repo *public* ise linki olan herkes görebilir. İsterseniz Netlify'da şifre koruması ekleyin.

Bol eğlenceler 🎉
