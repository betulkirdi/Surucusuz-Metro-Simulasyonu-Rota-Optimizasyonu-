🚇 Betül Kırdı - Metro Simulation Projesi

Bu proje, sürücüsüz bir metro ağı üzerinde iki istasyon arasındaki **en az aktarma** ve **en hızlı** rotaları bulmayı amaçlayan bir simülasyondur.

 🔧 Kullanılan Teknolojiler ve Kütüphaneler
- Python 3
- collections modülü:
 -  deque: BFS algoritması için kuyruk yapısı.
- heapq modülü:
  - Öncelik kuyruğu oluşturmak için kullanıldı (A* algoritması).

📌 Algoritmaların Açıklamaları

1. BFS (Breadth-First Search) - en_az_aktarma_bul
- İstasyonlar arasında **en az aktarmalı** rotayı bulmak için kullanılır.
- Kuyruk yapısı ile çalışır.
- Komşu istasyonları keşfeder ve hedefe ilk ulaştığında rota döndürülür.

2. A* Algoritması - en_hizli_rota_bul
- İstasyonlar arası **en kısa sürede ulaşılabilecek** rotayı bulur.
- Her bağlantının süresi (dakika) göz önünde bulundurulur.
- Öncelik kuyruğu kullanılarak en düşük süreli rotalar öncelikli değerlendirilir.
- Bu projede basitleştirilmiş haliyle, heuristik kullanılmadan uygulanmıştır.

 🧪 Test Senaryoları

Aşağıdaki senaryolar test edilmiştir:

1. AŞTİ -> OSB
- En az aktarma: AŞTİ → Kızılay → Ulus → Demetevler → OSB
- En hızlı rota: (25 dakika)

2. Batıkent -> Keçiören
- En az aktarma: Batıkent → Demetevler → Gar → Keçiören
- En hızlı rota: (21 dakika)

3. Keçiören -> AŞTİ
- En az aktarma: Keçiören → Gar → Sıhhiye → Kızılay → AŞTİ
- En hızlı rota: (19 dakika)

 🚀 Projeyi Geliştirme Fikirleri
- Görsel arayüz ile istasyonların harita üzerinde gösterimi
- Kullanıcının başlangıç ve hedef istasyonları seçebileceği bir CLI/GUI arayüz
- Gerçek zamanlı yoğunluk verisine göre rota önerisi
- Daha büyük ve gerçekçi metro ağı entegrasyonu

 🗂️ Dosya Yapısı
BetülKırdı_MetroSimulation.py  # Ana Python kodu
README.md                      # Açıklayıcı döküman (bu dosya)

🧠 Yazar Bilgisi
Ad: Betül Kırdı  
Bootcamp: Akbank x Global AI Hub - Python ile Yapay Zekaya Giriş

---
Herhangi bir sorunuz olursa iletişime geçebilirsiniz. İyi kodlamalar! 💻🚇

