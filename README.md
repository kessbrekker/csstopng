# Live Logo Editor 🎨

**Live Logo Editor**, HTML ve CSS kullanarak tarayıcı üzerinden anlık olarak logo tasarlamanıza ve tasarladığınız logoyu yüksek kaliteli **PNG** formatında indirmenize olanak tanıyan minimalist bir web aracıdır.

---

## 🔗 Canlı Demo

Projeyi anında denemek için buraya tıklayın:  
👉 **[kessbrekker.github.io/csstopng/](https://kessbrekker.github.io/csstopng/)**

---

## ✨ Özellikler

* **Canlı Önizleme:** HTML ve CSS panellerinde yaptığınız her değişiklik anında sol taraftaki logo alanına yansır.
* **Profesyonel Editör:** CodeMirror altyapısı ile VS Code teması, sözdizimi vurgulama ve otomatik tamamlama desteği.
* **Dinamik Ölçekleme:** CSS içindeki `#logo` boyutları ne olursa olsun, önizleme alanı tasarımı merkeze alacak şekilde otomatik ölçeklenir.
* **PNG Çıktısı:** `html2canvas` entegrasyonu sayesinde tasarladığınız alanı tek tıkla şeffaf olmayan yüksek kaliteli bir görsel olarak indirin.

---

## 🚀 Yerel Kurulum

Projeyi kendi bilgisayarınızda çalıştırmak isterseniz:

```bash
# Depoyu klonlayın
git clone [https://github.com/kessbrekker/csstopng.git](https://github.com/kessbrekker/csstopng.git)

# Proje dizinine gidin
cd csstopng

# index.html dosyasını tarayıcınızda açmanız yeterlidir.
```

---

## 🛠️ Teknik Altyapı

* **CodeMirror 5.65.13:** Gelişmiş kod düzenleme deneyimi için.
* **html2canvas 1.4.1:** HTML elementlerini görsel dosyasına dönüştürmek için.
* **Modern CSS:** Flexbox ve Grid sistemleri ile duyarlı panel yapısı.
* **VS Code Dark Theme:** Göz yormayan karanlık mod editör tasarımı.

---

## 📁 Dosya Yapısı

Proje, taşınabilirliği artırmak adına tüm mantığı tek bir dosya içinde toplar:

* **UI:** `.ext` (konteynır), `.export` (önizleme) ve `.code` (editörler) katmanları.
* **Editors:** HTML ve CSS için ayrılmış iki farklı `CodeMirror` nesnesi.
* **Scripts:** Değişiklikleri anlık işleyen `applyHTML()` / `applyCSS()` fonksiyonları ve kayıt mantığı.

---

## 📄 Lisans

© 2025 [Kessbrekker](https://github.com/Kessbrekker). Tüm hakları saklıdır.
