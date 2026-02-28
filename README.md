# GunesTakipSistemi
☀️ Dual-Axis Solar Tracking System (Çift Eksenli Güneş Takip Sistemi)
Bu proje, güneş panellerinin verimliliğini artırmak amacıyla güneşin konumunu anlık olarak takip eden, Arduino tabanlı bir otonom takip sistemidir. Sistem, 4 adet LDR sensörü kullanarak ışık yoğunluğunu ölçer ve paneli hem yatay (horizontal) hem de dikey (vertical) eksende en dik açıya getirecek şekilde servo motorları yönlendirir.

🚀 Özellikler
Tam Otomatik Kontrol: Işık kaynağını 2 eksende (X ve Y) gerçek zamanlı takip.

Hassas Ölçüm: 4 farklı yöne yerleştirilmiş LDR sensörleri ile yüksek doğruluk.

Dinamik Hareket: Servo motorlar sayesinde pürüzsüz ve stabil yönlendirme.

Verimlilik: Sabit panellere oranla %25-%40 arası daha fazla enerji üretimi simülasyonu.

🛠️ Donanım Bileşenleri
Mikrokontrolcü: Arduino Uno / Nano

Sensörler: 4x LDR (Işığa Duyarlı Direnç)

Motorlar: 2x SG90 Servo Motor (Yatay ve Dikey hareket için)

Dirençler: 4x 10k Ohm (LDR devresi için)

Mekanik: 3D baskı veya el yapımı hareketli iskelet

📐 Çalışma Mantığı
Sistem, LDR sensörlerinden gelen analog verileri karşılaştırarak çalışır:

Üst vs Alt LDR'ler: Dikey eksendeki servo motoru hareket ettirir.

Sağ vs Sol LDR'ler: Yatay eksendeki servo motoru hareket ettirir.

Eğer iki taraf arasındaki ışık farkı belirlenen eşik değerinden (threshold) büyükse, servo motor farkın azaldığı yöne doğru döner.

📂 Kurulum
Bu repoyu bilgisayarınıza klonlayın:

Bash
git clone https://github.com/senaaksakalli/solar-tracker.git
solar_tracker.ino dosyasını Arduino IDE ile açın.

Gerekli kütüphanelerin (Servo.h) yüklü olduğundan emin olun.

Kodu Arduino kartınıza yükleyin.
