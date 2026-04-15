# Product Requirements Document (PRD): SpendWise AI v1.0

> **Note:** This document is prepared in English for international standards, with comprehensive Turkish translations provided in collapsed sections.

---

## 1. Executive Summary / Yönetici Özeti
SpendWise AI is an intelligent assistant that optimizes subscriptions to protect financial health. This document covers the technical and functional requirements for the MVP phase.

<details>
<summary><b>🇹🇷 Türkçe Özet</b></summary>
SpendWise AI, kullanıcıların finansal sağlığını korumak amacıyla abonelikleri optimize eden bir yapay zeka asistanıdır. Bu doküman, MVP sürecindeki teknik ve işlevsel gereksinimleri kapsar.
</details>

---

## 2. Problem Statement & Market Fit / Problem Tanımı ve Pazar Uyumu
- **Problem:** Users lose between €200-€500 annually on unused or forgotten subscriptions.
- **Solution:** Instead of passive tracking, using AI for active intervention and preventive action.

<details>
<summary><b>🇹🇷 Problem ve Çözüm</b></summary>
- **Problem:** Kullanıcılar her yıl ortalama 200-500€ arası tutarı, kullanmadıkları veya unuttukları aboneliklere harcamaktadır.
- **Çözüm:** Harcamaları pasif takip etmek yerine, yapay zeka ile aktif müdahale ve önleyici aksiyon almak.
</details>

---

## 3. User Personas / Kullanıcı Personaları
1. **Digital Nomad Melisa:** A time-constrained professional with numerous SaaS and entertainment subscriptions.
2. **Budget-Conscious Student:** A user wanting to protect their limited budget from "free trial" traps.

<details>
<summary><b>🇹🇷 Kullanıcı Personaları</b></summary>
1. **Dijital Göçebe Melisa:** Çok sayıda SaaS ve eğlence aboneliği olan, zamanı kısıtlı profesyonel.
2. **Bütçe Dostu Öğrenci:** Sınırlı bütçesini "free trial" tuzaklarından korumak isteyen kullanıcı.
</details>

---

## 4. Functional Requirements / Fonksiyonel Gereksinimler

### 4.1. Subscription Intelligence (SI)
- **FR.01:** The system shall parse raw bank statements in CSV/JSON formats.
- **FR.02:** The AI model shall classify "Recurring" vs. "One-time" expenses with 95% accuracy.
- **FR.03:** The system shall detect price increases for the same service (e.g., Netflix 15% hike) and notify the user.

<details>
<summary><b>🇹🇷 Abonelik Zekası (SI) Detayları</b></summary>
- **FR.01:** Sistem, CSV/JSON formatındaki ham banka verilerini parse edebilmelidir.
- **FR.02:** AI modeli, "Abonelik" (Recurring) ve "Tek Seferlik" harcamaları %95 doğrulukla sınıflandırmalıdır.
- **FR.03:** Sistem, aynı servis için yapılan fiyat artışlarını (Örn: Netflix %15 zam) tespit edip bildirmelidir.
</details>

### 4.2. Predictive Analytics & Dashboard
- **FR.04:** The system shall visualize the user's "Monthly Burn Rate."
- **FR.05:** The system shall forecast the expected end-of-month balance, accounting for upcoming bills.

<details>
<summary><b>🇹🇷 Tahminleme ve Panel Detayları</b></summary>
- **FR.04:** Kullanıcının "Aylık Nakit Tüketim Oranı" (Burn Rate) görselleştirilmelidir.
- **FR.05:** Sistem, ay sonu beklenen bakiyeyi, yaklaşan faturaları hesaba katarak tahmin etmelidir.
</details>

### 4.3. Ghost Card & Security
- **FR.06:** Users shall be able to define virtual cards that auto-expire after a set period (e.g., 30 days).
- **FR.07:** Instant blockage shall be applied for limit violations or unexpected withdrawal attempts.

<details>
<summary><b>🇹🇷 Hayalet Kart ve Güvenlik Detayları</b></summary>
- **FR.06:** Kullanıcı, belirli bir süre (Örn: 30 gün) sonra otomatik kapanacak sanal kartlar tanımlayabilmelidir.
- **FR.07:** Kart limit aşımı veya beklenmedik çekim taleplerinde anlık blokaj uygulanmalıdır.
</details>

---

## 5. Non-Functional Requirements / Teknik Olmayan Gereksinimler
- **Security:** Data shall be processed locally or end-to-end encrypted (Data Privacy).
- **Usability:** Analysis results must be converted into a "Savings Score" understandable by non-technical users.
- **Scalability:** The system shall be modular enough to support 10,000+ different bank statement formats.

<details>
<summary><b>🇹🇷 Teknik Olmayan Gereksinimler</b></summary>
- **Güvenlik:** Veriler yerel cihazda işlenmeli veya uçtan uca şifrelenmelidir (Veri Gizliliği).
- **Kullanılabilirlik:** Analiz sonuçları teknik olmayan bir kullanıcının anlayacağı "Tasarruf Skoruna" dönüştürülmelidir.
- **Ölçeklenebilirlik:** Sistem, aynı anda 10.000+ farklı banka dökümü formatını destekleyecek modüler yapıda olmalıdır.
</details>

---

## 6. MVP Success Metrics (KPIs) / Başarı Metrikleri
- **Conversion Rate:** At least 40% of users should cancel/optimize an expense within the first 7 days.
- **Savings Per User (SPU):** Target of €150 average annual savings per user.

<details>
<summary><b>🇹🇷 Başarı Metrikleri</b></summary>
- **Dönüşüm Oranı:** Ürünü kuran kullanıcıların en az %40'ı ilk 7 günde bir aboneliğini iptal etmeli veya optimize etmelidir.
- **Kullanıcı Başı Tasarruf (SPU):** Kullanıcı başına yıllık ortalama 150€ tasarruf hedefi.
</details>

---

## 7. Future Roadmap / Gelecek Yol Haritası
- **Phase 2:** Direct Open Banking API integrations.
- **Phase 3:** AI-powered live customer service negotiation automation.

<details>
<summary><b>🇹🇷 Gelecek Planları</b></summary>
- **2. Aşama:** Doğrudan Banka API entegrasyonları (Open Banking).
- **3. Aşama:** AI Bot ile canlı müşteri hizmetleri pazarlık otomasyonu.
</details>
