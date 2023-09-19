# Economic_ANALYSIS_with_FRED_API
# Fred API Kullanımı

Bu GitHub repository, Fred API'sini kullanarak ekonomik verileri çekme ve analiz etme sürecini gösterir.

## İçindekiler

1. [Nasıl Başlamalı](#nasıl-başlamalı)
2. [Veri Çekme](#veri-çekme)
3. [Veri Analizi](#veri-analizi)
4. [Grafikler](#grafikler)

## Nasıl Başlamalı

Bu projeyi yerel bir Python ortamında çalıştırmak için aşağıdaki adımları izleyin:

1. Python'u yükleyin.
2. Gerekli kütüphaneleri yükleyin: `pip install pandas matplotlib`.
3. Fred API anahtarınızı `config.py` dosyasına ekleyin.

## Veri Çekme

Fred API'sini kullanarak ekonomik verileri çekmek için `fredapi` kütüphanesini kullanabilirsiniz. Veri çekme işlemi için örnek kod:

```python
from fredapi import Fred

# https://fred.stlouisfed.org sitesine gidin fred API key alın.

# API anahtarınızı buraya ekleyin
api_key = "YOUR_API_KEY"

fred = Fred(api_key=api_key)
data = fred.get_series("UNRATE")

## Veri görselleştirme

# Proje içinde fred apı kullanarak genellikle birbiri ile ilişki veriler açıklamalı ve grafik yardımı ile analiz edilmiştir.
# Proje daha gelişime açıktır.
# Grafiklerin altına profesyonel olmayan şekilde neden böyle olabileceği ile alakalı yorumlar eklenmiştir.


