# 🌞 Güneş Paneli Yerleşimi Optimizasyonu (Genetik Algoritma)

**Ad:** Alper Serin  
**Okul Numarası:** 2312729001  
**Ders:** Yapay Zeka Sistemleri – 1. Proje Ödevi  

---

## 📌 Proje Hakkında
Bu projede, bir belediyenin güneş enerjisi sistemi kurulumunda panellerin  
**eğim açısını (x1)** ve **güney yönüne göre sapma açısını (x2)**  
en verimli olacak şekilde belirlemek amaçlanmıştır.

Optimizasyon işlemi **Genetik Algoritma (Genetic Algorithm)** kullanılarak gerçekleştirilmiştir.

---

## 🎯 Problem Tanımı

### Amaç Fonksiyonu
y = 6x1 + 4x2 - 0.1x1^2


- **x1** : Panel eğim açısı (derece)  
- **x2** : Güney yönüne göre sapma açısı (derece)  
- **y** : Toplam enerji verimi (maksimize edilmek istenen değer)

---

## 🔢 Değişken Sınırları

- **Eğim (x1):** 10 – 45 derece  
- **Yön (x2):** 0 – 90 derece  

---

## ⚠️ Kısıtlar

### Minimum yönlenme şartı
x2 ≥ 15

### Fiziksel kurulum sınırı
x1 + 0.5x2 ≤ 60


Kısıtları ihlal eden bireylere **ceza yöntemi (penalty method)** uygulanmıştır.

---

## 🧠 Kullanılan Yöntemler

- Genetik Algoritma
- Rulet Seçimi (Roulette Wheel Selection)
- Tek Noktalı Çaprazlama
- Mutasyon
- Elitizm
- Ceza Yöntemi (Penalty Method)

---

## 🧩 Kod Yapısı ve Fonksiyonlar

Proje **tek bir Jupyter Notebook (.ipynb)** dosyası içerisinde geliştirilmiştir.

Notebook’ta yer alan temel fonksiyonlar:

- `kullanici_parametreleri()`  
  → Popülasyon sayısı, jenerasyon sayısı, mutasyon oranı ve ceza katsayısını kullanıcıdan alır.

- `birey_uret()`  
  → Rastgele bir birey (x1, x2) üretir.

- `populasyon_uret()`  
  → Başlangıç popülasyonunu oluşturur.

- `fitness_fonksiyonu()`  
  → Amaç fonksiyonu ve kısıt cezalarını kullanarak uygunluk değerini hesaplar.

- `rulet_secim()`  
  → Rulet tekerleği yöntemine göre ebeveyn seçimi yapar.

- `caprazlama()`  
  → Tek noktalı çaprazlama uygular.

- `mutasyon()`  
  → Belirli bir olasılıkla birey üzerinde mutasyon uygular.

---

## ▶️ Nasıl Çalıştırılır?

Bu proje bir **Jupyter Notebook (.ipynb)** dosyasıdır.

1. GitHub üzerindeki `.ipynb` dosyasına tıklayarak kodu ve çıktıları görüntüleyebilirsiniz.
2. Dosyayı **Google Colab** üzerinde açarak çalıştırabilirsiniz.
3. Çalıştırma sırasında gerekli parametreler kullanıcıdan alınır.
