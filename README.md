# 📊 EDA Pipeline: Hastane Veri Analizi ve Ön İşleme 🏥

**Adı Soyadı:** Fatma Tuğçe Mukul 💻

**E-posta:** mukultugce@gmail.com ✉️

## 📋 Proje Özeti

Bu proje, ham hastane verilerini temizlemek, dönüştürmek ve analiz için hazır hale getirmek üzere tasarlanmış kapsamlı bir Python betiğidir. Veri setindeki eksik değerleri akıllı stratejilerle doldurur, metin tabanlı sütunlardaki tutarsızlıkları giderir ve makine öğrenmesi modelleri için uygun özellikler oluşturur. Pipeline, aşağıdaki adımları otomatikleştirerek veri ön işleme sürecini standartlaştırır:

### 1. 🧹 Veri Temizliği ve Dönüşümü
- `'UygulamaSuresi'` ve `'TedaviSuresi'` gibi metinsel verileri sayısal formatlara çevirir.

### 2. 🔄 Eksik Değer Yönetimi
- `HastaNo` grubuna göre veya `KNNImputer` gibi gelişmiş yöntemlerle eksik verileri doldurur.

### 3. 🔡 Metin Normalizasyonu
- `'Tanilar'`, `'TedaviAdi'`, `'Alerji'` ve `'KronikHastalik'` gibi sütunlarda metinleri temizler ve standartlaştırır.
  

### 4. 📊 Kategorik Değişken Kodlaması
- `'Cinsiyet'` ve `'Alerji'` kategorik verileri  **One-Hot Encoding** ile makine öğrenmesi modellerinin anlayacağı sayısal formata dönüştürür.

### 5. 📈 Görsel Analiz ve Kontroller
- Veri setindeki ilişkileri gösteren çeşitli grafikler oluşturur ve yinelenen sütunları temizler.

---

## 🛠️ Kurulum ve Çalıştırma Talimatları

### 1. 📦 Gerekli Kütüphaneler

Projeyi çalıştırmadan önce aşağıdaki Python kütüphanelerinin sisteminizde yüklü olduğundan emin olun. Gerekli kütüphaneleri tek bir komutla kurabilirsiniz:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn fuzzywuzzy python-Levenshtein openpyxl
```

### 2. 🗂️ Dosya Yapısı

Kodun sorunsuz çalışması için, orijinal Excel dosyasının (`talent.xlsx`) betiğin bulunduğu dizinle aynı yerde olması gerekmektedir.

```
.
├── talent.xlsx           # Orijinal ham veri dosyası
├── eda_pipeline.py       # Bu projenin ana betiği
└── README.md
```

### 3. ▶️ Betiği Çalıştırma

Projeyi çalıştırmak için **Jupyter Notebook** veya **Google Colab** ortamını açın.  
`talent.xlsx` dosyasının çalışma dizininde bulunduğundan ve gerekli kütüphanelerin yüklü olduğundan emin olun.  

Ardından, notebook üzerindeki hücreleri sırayla çalıştırarak veri ön işleme sürecini başlatabilirsiniz.

> **Not:** Proje hakkında daha fazla bilgi ve analiz sonuçlarına *Bulgular_FatmaTugceMukul.pdf* dosyasını indirerek ulaşabilirsiniz. 📄

### 4. 📂 Çıktı

Tüm hücreler başarıyla çalıştırıldığında, ön işleme adımlarından geçmiş olan temiz veri seti `temizlenmis_veri_son.csv` adıyla çalışma dizinine kaydedilecektir.

```
.
├── talent.xlsx
├── eda_pipeline.py
├── temizlenmis_veri_son.csv  # İşlenmiş ve temizlenmiş veri
└── README.md
```" 
