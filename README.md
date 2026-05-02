# 🚀 Şirket İçi İş Akışı Darboğaz Tespit Sistemi (n8n & Notion & Gemini AI)

Bu proje, bir işletmenin iş akışlarını (workflow) otomatik olarak analiz eden ve verimliliği düşüren "darboğazları" (bottlenecks) tespit eden yapay zeka destekli bir otomasyon sistemidir.

## 🛠️ Kullanılan Teknolojiler
* **n8n:** İş akışı otomasyonu ve entegrasyon merkezi.
* **Notion:** Veri kaynağı (Tasks) ve raporlama (Alerts) merkezi.
* **Google Gemini AI:** Verilerin analizi ve risk skorlaması için kullanılan LLM.
* **JavaScript:** n8n içindeki özel veri işleme mantığı için.

## 📋 Sistem Nasıl Çalışır?
 **Veri Çekme:** n8n, Notion üzerindeki `Tasks` veritabanından mevcut görevleri çeker.
 ekran görüntüleri
 <img width="1689" height="814" alt="Ekran görüntüsü 2026-05-02 152832" src="https://github.com/user-attachments/assets/b1374f31-662c-437e-ba46-210018623a01" />
  
 **AI Analizi:** Google Gemini, görevlerin bekleme sürelerini ve aşamalarını analiz ederek bir "Darboğaz Skoru" oluşturur.
 ekran görüntüleri
<img width="943" height="860" alt="Ekran görüntüsü 2026-05-02 221908" src="https://github.com/user-attachments/assets/6273bb2c-2438-4e4e-8561-7a78be4c9c47" />

**Risk Filtreleme:** Eğer risk skoru "Yüksek" veya "Kritik" ise sistem devreye girer
 ekran görüntüleri
<img width="1718" height="527" alt="Ekran görüntüsü 2026-05-02 153016" src="https://github.com/user-attachments/assets/7ccacee2-af7f-4458-b63b-89a0d59d6a36" />

**Raporlama:** Tespit edilen darboğazlar, çözüm önerileriyle birlikte Notion'daki `Alerts` veritabanına otomatik olarak işlenir.
 ekran görüntüleri
<img width="1760" height="696" alt="Ekran görüntüsü 2026-05-02 152959" src="https://github.com/user-attachments/assets/1ccbbdf6-89ce-4266-a6aa-94c3a9c12b76" />



## 🚀 Kurulum
1. `Şirket içi Workflow Bottleneck Tespit Sistemi.json` dosyasını indirin.
2. n8n arayüzünden "Import from file" diyerek içeri aktarın.
3. Notion API anahtarlarınızı tanımlayın.
