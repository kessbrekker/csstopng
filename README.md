# csstopng 🎨 ➡️ 🖼️

**csstopng**, CSS kodlarınızı veya HTML bileşenlerinizi hızlı bir şekilde yüksek kaliteli PNG görsellerine dönüştüren, Node.js tabanlı güçlü bir araçtır. Kod parçacıklarını görselleştirmek, dinamik sosyal medya görselleri oluşturmak veya UI dökümantasyonu için idealdir.

---

## ✨ Özellikler

* **Hızlı Dönüşüm:** Saf CSS veya HTML+CSS yapısını saniyeler içinde görsele dönüştürür.
* **Modern CSS Desteği:** Flexbox, Grid, Animasyonlar ve Gradient gibi modern özellikleri tam destekler.
* **Headless Engine:** Arka planda Puppeteer kullanarak tarayıcı kalitesinde çıktılar üretir.
* **Çift Kullanım:** Hem CLI (Terminal) üzerinden hem de projelerinizde bir kütüphane (API) olarak kullanılabilir.

---

## 🚀 Kurulum

Projeyi yerelinizde kullanmak için aşağıdaki adımları sırasıyla izleyin:

```bash
# Depoyu klonlayın
git clone [https://github.com/kessbrekker/csstopng.git](https://github.com/kessbrekker/csstopng.git)

# Proje dizinine gidin
cd csstopng

# Bağımlılıkları yükleyin
npm install
```

---

## 🛠️ Kullanım

### 1. Terminal (CLI) Kullanımı
Basit bir komutla CSS dosyanızı PNG'ye çevirin:
```bash
node index.js --input style.css --output result.png --width 800 --height 600
```

### 2. Modül Olarak Kullanım
Kendi Node.js projelerinize entegre edin:
```javascript
const csstopng = require('./src/converter');

const options = {
    css: '.box { background: linear-gradient(45deg, #fe6b8b, #ff8e53); padding: 50px; border-radius: 10px; color: white; font-family: Arial; }',
    html: '<div class="box"><h1>csstopng</h1><p>CSS to Image Converter</p></div>',
    width: 600,
    height: 400
};

csstopng.generate(options)
    .then(path => console.log('Görsel oluşturuldu:', path))
    .catch(err => console.error('Hata:', err));
```

---

## ⚙️ Yapılandırma

| Parametre | Tip | Açıklama | Varsayılan |
| :--- | :--- | :--- | :--- |
| `input` | `String` | Kaynak CSS dosyasının yolu | `style.css` |
| `output` | `String` | Oluşturulacak PNG adı | `output.png` |
| `width` | `Number` | Görsel genişliği (piksel) | `1200` |
| `height` | `Number` | Görsel yüksekliği (piksel) | `630` |
| `transparent`| `Boolean`| Arka planın şeffaf olması | `false` |

---

## 📁 Proje Yapısı

```text
csstopng/
├── src/                # Dönüştürücü çekirdek dosyaları
├── examples/           # Kullanım örnekleri
├── index.js            # CLI giriş noktası
├── package.json        # Bağımlılıklar
└── README.md           # Kılavuz
```

---

## 🤝 Katkıda Bulunma

1. Projeyi fork edin.
2. Yeni bir özellik dalı açın (`git checkout -b feature/yeniOzellik`).
3. Değişikliklerinizi commit edin (`git commit -m 'Özellik eklendi'`).
4. Dalınızı push edin (`git push origin feature/yeniOzellik`).
5. Pull Request oluşturun.

---

## 📄 Lisans

Bu proje [MIT](LICENSE) lisansı altında dökümante edilmiştir.

---

**Geliştirici:** [@kessbrekker](https://github.com/kessbrekker)
