# E-Commerce Return Analytics

### Financial, Operational & ESG Insights

## 📌 Tentang Proyek

Proyek ini menganalisis data transaksi e-commerce untuk memahami pola retur, dampak finansial dan operasional, karakteristik pelanggan, serta dampak lingkungan yang berkaitan dengan proses retur.

Analisis dilakukan menggunakan Microsoft Excel, Power Query, Power BI, dan DAX dengan dataset synthetic e-commerce returns yang terdiri dari 5.000 transaksi.

---

## 🎯 Tujuan Analisis

Proyek ini bertujuan untuk menjawab beberapa pertanyaan bisnis:

1. Kategori produk mana yang memiliki Return Rate dan total biaya retur tertinggi?
2. Apakah tingkat diskon dan metode pengiriman berkaitan dengan tingkat retur yang lebih tinggi?
3. Apa alasan retur utama pada tiap kategori produk?
4. Berapa CO₂ Emissions dan Packaging Waste yang berkaitan dengan pesanan yang dikembalikan?
5. Bagaimana profil demografi pelanggan yang melakukan retur?
6. Berapa CO₂ Saved dan Waste Avoided dari pesanan yang tidak dikembalikan?

---

## 🗂️ Dataset

Dataset yang digunakan merupakan **Synthetic E-Commerce Returns Dataset** dengan:

- **5.000 transaksi**
- **23 kolom utama**
- Informasi transaksi, produk, pelanggan, retur, biaya, profit/loss, dan metrik lingkungan

Beberapa variabel utama:

- Order ID
- Product Category
- Product Price
- Order Quantity
- Discount Applied
- Shipping Method
- User Age
- User Gender
- User Location
- Return Status
- Return Reason
- Return Cost
- Profit/Loss
- CO₂ Emissions
- Packaging Waste
- CO₂ Saved
- Waste Avoided

---

## 🛠️ Tools & Technologies

- **Microsoft Excel** — data inspection, cleaning, dan exploratory analysis
- **Power Query** — data transformation dan perbaikan format numerik
- **Power BI** — dashboard dan data visualization
- **DAX** — pembuatan measures dan calculated columns

---

## 🔄 Data Preparation & Analysis Process

### 1. Data Cleaning

Melakukan pengecekan kualitas data untuk memastikan data siap dianalisis, meliputi:

- Checking missing values
- Checking duplicate Order ID
- Checking data types
- Perbaikan format numerik dan decimal separator
- Validasi format tanggal

### 2. Data Preparation

Membuat beberapa variabel tambahan untuk mendukung analisis:

- Age Group
- Discount Band
- Month
- Return Flag

### 3. Data Analysis

Analisis dilakukan berdasarkan:

- Product Category
- Discount Band
- Shipping Method
- Return Reason
- Customer Demographics
- Financial Impact
- Environmental Impact

### 4. Dashboard Development

Membangun interactive dashboard menggunakan Power BI yang terdiri dari tiga halaman:

**Page 1 — Executive Overview**
- Total Orders
- Returned Orders
- Return Rate
- Total Return Cost
- Total Profit/Loss
- Monthly Order Value
- Return Rate by Product Category
- Returned vs Not Returned

**Page 2 — Return & Financial Analysis**
- Return Rate by Discount Band
- Return Rate by Shipping Method
- Return Reason by Product Category
- Interactive filters

**Page 3 — Customer & ESG Analysis**
- Return Rate by Age Group
- Return Rate by Gender
- Top 10 Locations by Return Rate
- CO₂ Emissions
- Packaging Waste
- CO₂ Saved
- Waste Avoided

---

## 📊 Key Insights

### 1. Overall Return Rate

Dari 5.000 transaksi, terdapat **1.450 returned orders**, sehingga overall Return Rate mencapai **29.00%**.

### 2. Product Category

**Clothing** memiliki Return Rate tertinggi sebesar **37.43%** dan total Return Cost sebesar **Rp132,200**.

### 3. Discount

Transaksi dengan diskon **>30%** memiliki Return Rate sebesar **34.2%**, lebih tinggi dibandingkan overall Return Rate sebesar 29.00%.

### 4. Shipping Method

Return Rate antar metode pengiriman relatif serupa:

- Express: 29.09%
- Next-Day: 28.50%
- Standard: 29.41%

Perbedaan antar metode pengiriman relatif kecil.

### 5. Return Reason

Secara keseluruhan, alasan retur terbanyak adalah:

- **Defective: 382**
- Changed Mind: 379
- Wrong Item: 348
- Size Issue: 341

### 6. Customer Demographics

Return Rate berdasarkan kelompok usia relatif stabil, berada pada kisaran **27.52%–29.68%**.

Berdasarkan gender:

- Female: 30.20%
- Male: 27.72%

### 7. Environmental Impact

Pada returned orders:

- **CO₂ Emissions: 2,167.5**
- **Packaging Waste: 864.2**

Sementara dari non-returned orders:

- **CO₂ Saved: 5,333**
- **Waste Avoided: 2,133.4**

---

## 💡 Recommendations

Berdasarkan hasil analisis:

1. **Prioritaskan evaluasi kategori Clothing** karena memiliki Return Rate tertinggi.
2. **Evaluasi transaksi dengan diskon tinggi**, terutama diskon di atas 30%, untuk memahami pola retur yang berkaitan dengan segmen tersebut.
3. **Perkuat quality control**, terutama karena defective menjadi alasan retur terbanyak.
4. **Evaluasi proses fulfillment** untuk mengurangi potensi kesalahan pengiriman seperti Wrong Item.
5. **Monitor environmental metrics** sebagai bagian dari evaluasi dampak retur terhadap keberlanjutan operasional.

> Catatan: Analisis menunjukkan hubungan/pola pada data dan tidak dimaksudkan untuk menyimpulkan hubungan sebab-akibat.

---

## 📈 Dashboard

Dashboard dibuat menggunakan Microsoft Power BI dan terdiri dari tiga halaman:

### Executive Overview
![Executive Overview](dashboard/page-1-overview.png)

### Return & Financial Analysis
![Return & Financial Analysis](dashboard/page-2-return-financial.png)

### Customer & ESG Analysis
![Customer & ESG Analysis](dashboard/page-3-customer-esg.png)

---

## 📁 Project Structure

```text
ecommerce-return-analytics/
│
├── README.md
│
├── data/
│   └── README.md
│
├── powerbi/
│   └── ecommerce_return_analytics.pbix
│
├── dashboard/
│   ├── page-1-overview.png
│   ├── page-2-return-financial.png
│   └── page-3-customer-esg.png
│
└── documentation/
    └── project-summary.pdf
