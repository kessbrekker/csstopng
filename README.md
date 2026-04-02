# Live Logo Editor 🎨

Bu proje, HTML ve CSS kullanarak tarayıcı üzerinden canlı olarak logo tasarlamanıza ve tasarladığınız logoyu tek tıkla **PNG** formatında indirmenize olanak tanıyan minimalist bir web aracıdır.

---

## ✨ Özellikler

* **Canlı Önizleme:** HTML ve CSS editörlerinde yaptığınız değişiklikleri anında sol panelde görün.
* **Gelişmiş Editör:** CodeMirror altyapısı sayesinde VS Code teması, sözdizimi vurgulama (syntax highlighting) ve otomatik tamamlama desteği.
* **Akıllı Ölçekleme:** CSS içindeki `#logo` boyutlarına göre önizleme alanını otomatik olarak sığdıran dinamik transform yapısı.
* **PNG Olarak Kaydet:** `html2canvas` kütüphanesi ile tasarladığınız alanı yüksek kaliteli bir görsel olarak indirme.

---

## 🚀 Başlangıç

Proje herhangi bir sunucu veya kurulum gerektirmez. Sadece dosyayı klonlayıp tarayıcınızda açmanız yeterlidir.

### Kullanım

1.  Depoyu klonlayın:
    ```bash
    git clone [https://github.com/kessbrekker/csstopng.git](https://github.com/kessbrekker/csstopng.git)
    ```
2.  `index.html` (veya ilgili dosya) dosyasını herhangi bir modern tarayıcıda açın.
3.  **HTML** panelinden içeriği, **CSS** panelinden ise tasarımı düzenleyin.
4.  **Save as PNG** butonuna basarak logonuzu indirin.

---

## 🛠️ Teknik Detaylar

Bu araç aşağıdaki teknolojileri ve kütüphaneleri kullanmaktadır:

* **CodeMirror 5.65.13:** Kod editörü ve sözdizimi vurgulama için.
* **html2canvas 1.4.1:** HTML elementlerini canvas üzerinden görsele dönüştürmek için.
* **VS Code Theme:** Editör görünümü için özelleştirilmiş CSS teması.
* **Inter Font Family:** Modern ve temiz tipografi desteği.

---

## 📁 Proje Yapısı

Proje, tüm mantığı (CSS, HTML, JS) tek bir dosya içerisinde barındıracak şekilde tasarlanmıştır:

* **Styles:** Panel düzeni, karanlık mod arayüzü ve editör teması.
* **Editor:** HTML ve CSS için iki ayrı `CodeMirror` instance'ı.
* **Logic:** `applyHTML()` ve `applyCSS()` fonksiyonları ile anlık render alma ve `saveBtn` ile görsel çıktısı oluşturma.

---

## 📄 Lisans

© 2025 [Kessbrekker](https://github.com/Kessbrekker). Tüm hakları saklıdır.
