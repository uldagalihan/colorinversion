# Görüntü İşleme ve Histogram Eşitleme

 Proje, temel görüntü işleme tekniklerini Assembly dilinde uygulayarak color inversion ve histogram eşitleme işlemlerini gerçekleştirmektedir.

## Proje Hakkında

### Amaç
- Görüntü üzerindeki her pikselin renk değerlerini tersine çevirme (color inversion).
- Histogram eşitleme yöntemiyle görüntünün kontrastını optimize etme.

### Teknik Özellikler
- **Diller:** C++ ve Assembly
- **Platform:** Visual Studio 2022 (x86 - 32 bit)


### İşlevler
1. **Color Inversion**  
   Her pikselin renk değerleri şu şekilde tersine çevrilir:  
   `color[i, j] = 255 - color[i, j]`
   
2. **Histogram Eşitleme**  
   Histogram eşitleme işlemi dört adımdan oluşur:
   - **Histogram oluşturma:** Piksel değerlerinin dağılımını belirleme.
   - **Kümülatif Dağılım Fonksiyonu (CDF):** Piksel yoğunluklarının birikimli toplamını hesaplama.
   - **CDF Normalizasyonu:** Piksel değerlerini normalize etme.
   - **Histogram eşitleme uygulama:** Görüntüye yeni piksel değerlerini atama.

## Projeyi Çalıştırma

### Gereksinimler
- Visual Studio 2022 veya üstü
- C++ geliştirme ortamı yüklü olmalı
- 32-bit (x86) modunda derleme yapılmalı

### Kurulum
1. Bu projeyi klonlayın:
   ```bash
   git clone https://github.com/uldagalihan/image-processing.git
