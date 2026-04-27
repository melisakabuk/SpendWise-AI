# Product Requirements Document (PRD): SpendWise AI v1.0

> **Global Standard Compliance:** This document follows international Business Analysis standards. Turkish translations are provided in collapsed sections for accessibility.

---

## 1. Executive Summary & Objective / Yönetici Özeti ve Amaç
**SpendWise AI** is an autonomous financial intelligence tool designed to eliminate "subscription leakage." The primary objective of the MVP is to provide users with a 100% transparent view of their recurring liabilities and to automate the prevention of unwanted charges.

<details>
<summary><b>🇹🇷 Türkçe Özet</b></summary>
SpendWise AI, "abonelik sızıntılarını" ortadan kaldırmak için tasarlanmış otonom bir finansal zeka aracıdır. MVP'nin temel amacı, kullanıcılara tekrarlayan yükümlülükleri üzerinde %100 şeffaf bir görünüm sağlamak ve istenmeyen ücretlerin önlenmesini otomatikleştirmektir.
</details>

---

## 2. Technical Scope & Logic / Teknik Kapsam ve Mantık

### 2.1. Subscription Intelligence (SI) Engine
* **Logic:** The engine utilizes a **Pattern Recognition Algorithm** to scan transaction history. It identifies recurring merchant IDs, consistent billing dates, and slight variations in amounts (e.g., FX rate changes).
* **Edge Case Handling:** If a transaction occurs twice in 30 days but with different amounts, the AI flags it as a "Potential Overcharge" or "Tier Change" for user verification.

<details>
<summary><b>🇹🇷 Abonelik Zekası (SI) Motoru Mantığı</b></summary>
* **Mantık:** Motor, işlem geçmişini taramak için Örüntü Tanıma Algoritması kullanır. Tekrarlayan satıcı kimliklerini, tutarlı fatura tarihlerini ve tutarlardaki hafif sapmaları (örneğin döviz kuru değişiklikleri) tanımlar.
* **İstisnai Durum Yönetimi:** Bir işlem 30 gün içinde iki kez ancak farklı tutarlarla gerçekleşirse, yapay zeka bunu kullanıcı doğrulaması için "Potansiyel Fazla Ödeme" olarak işaretler.
</details>

### 2.2. Predictive Liquidity Algorithm
* **Logic:** Calculates the **Cash Burn Rate** by aggregating all detected subscriptions against the user's current balance. 
* **Feature:** Generates a "Safe-to-Spend" limit, which subtracts all upcoming automated payments from the current liquidity.

<details>
<summary><b>🇹🇷 Tahminleyici Likidite Algoritması</b></summary>
* **Mantık:** Kullanıcının mevcut bakiyesine karşı tespit edilen tüm abonelikleri toplayarak "Nakit Tüketim Oranını" hesaplar.
* **Özellik:** Mevcut likiditeden yaklaşan tüm otomatik ödemeleri çıkararak bir "Harcaması Güvenli" limiti oluşturur.
</details>

---

## 3. Detailed Functional Requirements / Detaylı Fonksiyonel Gereksinimler

| Requirement ID | Feature Name | Detailed Description | Priority |
| :--- | :--- | :--- | :--- |
| **FR.01** | **Multi-Format Ingestion** | Support for parsing CSV, JSON, and PDF (via OCR) bank statements. | Must-Have |
| **FR.02** | **Dynamic Categorization** | AI must distinguish between 'Subscription' (e.g., Netflix) and 'Utility' (e.g., Electric Bill). | High |
| **FR.03** | **Ghost Card Simulation** | Users create virtual cards with a 'Self-Destruct' timer (e.g., 30 days for Free Trials). | High |
| **FR.04** | **Negotiation Scripting** | System generates a pre-filled email/chat template for cancellation or discount requests. | Medium |
| **FR.05** | **Alert Hierarchy** | 3-Day Warning: Before a trial ends. 24-Hour Warning: Before a price hike takes effect. | High |

<details>
<summary><b>🇹🇷 Detaylı Fonksiyonel Gereksinimler (TR)</b></summary>
- **FR.01:** CSV, JSON ve PDF (OCR ile) banka dökümlerini ayrıştırma desteği.
- **FR.02:** Yapay zeka, 'Abonelik' (Netflix) ve 'Fatura' (Elektrik) ayrımını yapabilmelidir.
- **FR.03:** 'Kendi Kendini Yok Etme' zamanlayıcısına sahip sanal kartlar (Deneme sürümleri için).
- **FR.04:** İptal veya indirim talepleri için önceden doldurulmuş taslak metin oluşturma.
- **FR.05:** Bildirim Hiyerarşisi: Deneme bitmeden 3 gün önce ve fiyat artışından 24 saat önce uyarı.
</details>

---

## 4. Non-Functional Requirements / Fonksiyonel Olmayan Gereksinimler

* **Security & Privacy (GDPR/KVKK):** All financial data must be anonymized. No raw banking credentials are stored on the server during the MVP phase.
* **Performance:** AI classification of 12-month transaction data must be completed in under 5 seconds.
* **Usability:** Dashboard must provide a "Financial Health Score" (0-100) based on subscription efficiency.

<details>
<summary><b>🇹🇷 Teknik Olmayan Gereksinimler</b></summary>
* **Güvenlik ve Gizlilik:** Tüm finansal veriler anonimleştirilmelidir. MVP aşamasında sunucuda ham bankacılık bilgisi saklanmaz.
* **Performans:** 12 aylık işlem verisinin yapay zeka ile sınıflandırılması 5 saniyenin altında tamamlanmalıdır.
* **Kullanılabilirlik:** Dashboard, abonelik verimliliğine göre bir "Finansal Sağlık Skoru" sunmalıdır.
</details>

---

## 5. Success Metrics (KPIs) / Başarı Metrikleri

1.  **Subscription Optimization Rate:** Percentage of users who cancel at least one "zombie" subscription within 30 days.
2.  **Avoided Charges:** Total monetary value of payments blocked by "Ghost Cards."
3.  **User Friction Score:** Time taken from data upload to first saving insight.

<details>
<summary><b>🇹🇷 Başarı Metrikleri</b></summary>
1. **Abonelik Optimizasyon Oranı:** 30 gün içinde en az bir gereksiz aboneliği iptal eden kullanıcı oranı.
2. **Engellenen Ücretler:** "Hayalet Kartlar" tarafından engellenen toplam parasal değer.
3. **Kullanıcı Sürtünme Skoru:** Veri yüklemeden ilk tasarruf içgörüsüne kadar geçen süre.
</details>

---

## 6. Future Roadmap / Gelecek Yol Haritası
- **Phase 2 (Scalability):** Real-time integration with European Open Banking APIs (PSD2 Compliance).
- **Phase 3 (Automation):** Robotic Process Automation (RPA) to handle cancellations without user leaving the app.

<details>
<summary><b>🇹🇷 Gelecek Yol Haritası</b></summary>
- **2. Aşama:** Avrupa Açık Bankacılık API'leri ile gerçek zamanlı entegrasyon (PSD2 Uyumu).
- **3. Aşama:** Kullanıcının uygulamadan çıkmasına gerek kalmadan iptalleri gerçekleştiren RPA teknolojisi.
</details>
