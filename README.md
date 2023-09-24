# DocVectorSparkMinio


## İçindekiler

- [Proje Açıklaması](#proje-açıklaması)
- [Kurulum](#kurulum)
  - [Ön Gereksinimler](#ön-gereksinimler)
  - [Proje Kurulumu](#proje-kurulumu)
- [Kullanım](#kullanım)
  - [Docker Compose ile Ortamı Başlatma](#docker-compose-ile-ortamı-başlatma)
  - [FastAPI ile Doküman Yükleme](#fastapi-ile-doküman-yükleme)
 
 

Proje Açıklaması - Bu proje, Docker Compose ile oluşturulan bir Spark cluster, MinIO ve Airflow ortamını içerir. Ayrıca, FastAPI kullanarak MinIO veritabanına PDF dokümanları yükleme yeteneği sağlar. Proje, PDF dosyalarını saatlik olarak kaydedip Spark Streaming ile bu dokümanları işleyerek vektör formatına dönüştürme amacını taşır.

Projeyi Açıklama
Bu proje, büyük miktarda PDF dokümanı işlemek ve bunları vektör formatına dönüştürmek isteyenler için tasarlanmıştır. Projenin ana bileşenleri şunlardır:

Spark Cluster: Büyük veri işleme ve dağıtık hesaplama için Spark kullanılır. Spark, MinIO ile iletişim kurarak saatlik olarak kaydedilen PDF dosyalarını işler.

MinIO: MinIO, PDF dokümanlarını saklamak ve erişmek için kullanılır. PDF dosyaları saatlik olarak MinIO'ya kaydedilir ve Spark tarafından işlenir.

Airflow: Airflow, iş akışlarını planlamak ve otomatikleştirmek için kullanılır. Proje, PDF dosyalarını düzenli aralıklarla MinIO'ya kaydetmek için Airflow kullanır.

FastAPI: FastAPI, PDF dokümanlarını MinIO veritabanına yükleme yeteneği sunar. Bu, projeye yeni dokümanlar eklemenizi ve Spark tarafından işlenmelerini sağlar.

Projenin kullanımı ve kurulumu için ayrıntılı talimatlar Kurulum ve Kullanım bölümlerinde bulunmaktadır.

## Kurulum

Bu bölümde projenin yerel geliştirme ortamınızda nasıl çalıştırılacağı ve yapılandırılacağı açıklanır.

### Ön Gereksinimler

Proje çalıştırmak için aşağıdaki ön gereksinimlere ihtiyacınız vardır:

- Docker
- Docker Compose
- Python 3.6+

### Proje Kurulumu

1. Bu depoyu klonlayın:

   ```bash
   git clone https://github.com/erdoganali/DocVectorSparkMinio.git
 

Docker
Docker Compose
Python 3.6+
Proje, bu gereksinimleri yerine getiren bir geliştirme ortamı sağlar.
 
 
