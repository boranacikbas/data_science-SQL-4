# Data Science SQL Project 4 — VIEW, CTE, CASE & Subqueries

Bu proje, PostgreSQL veritabanı üzerinde gelişmiş SQL sorgulama tekniklerini (VIEW, CTE, CASE WHEN, Subquery) ve Python (`psycopg2`) entegrasyonunu kapsayan analitik bir veri bilimi çalışmasıdır. Projedeki tüm sorgular otomatize edilmiş `pytest` test senaryoları ile doğrulanmıştır.

---

## 📌 Proje Kapsamı ve SQL Teknikleri

Proje 11 analitik görevden oluşmakta ve aşağıdaki temel SQL konularını içermektedir:

### 1. VIEW Oluşturma
- **`completed_orders`**: Tamamlanmış siparişlerin filtrelenmiş dinamik görünümü.
- **`electronics_products`**: Elektronik kategorisindeki ürünlerin filtrelenmiş görünümü.

### 2. Common Table Expressions (WITH / CTE)
- **Müşteri Bazlı Harcama**: CTE kullanarak müşteri bazında toplam harcama hesaplaması.
- **Sipariş ve Ürün Detayları**: Çoklu tablo birleştirmeleri (JOIN) ile sipariş tutarlarının detaylandırılması.

### 3. Koşullu Mantık (CASE WHEN) ve Subqueries
- **Sipariş Durumu Türkçeleştirme**: Sipariş statülerinin iş mantığına göre etiketlenmesi.
- **Müşteri Segmentasyonu**: Sipariş frekansına göre müşterilerin sınıflandırılması (`Sadık Müşteri`, `Orta Seviye`, `Yeni Müşteri`).
- **Fiyat Kategorilendirmesi**: Ürünlerin fiyat aralıklarına göre etiketlenmesi (`Pahalı`, `Orta`, `Ucuz`).
- **Ortalama Üstü Analizler**: Alt sorgular (Subquery) ile ortalama fiyatın üzerindeki ürünlerin ve en pahalı ürünü satın alan müşterilerin tespiti.

---

## 🛠️ Teknolojiler ve Araçlar

- **Veritabanı:** PostgreSQL
- **Programlama Dili:** Python 3.x
- **Veritabanı Sürücüsü:** `psycopg2`
- **Test Otomasyonu:** `pytest`, `watch.py`

---

## 🚀 Kurulum ve Çalıştırma

1. **Bağımlılıkları Yükleyin:**
   ```bash
   pip install -r requirements.txt
