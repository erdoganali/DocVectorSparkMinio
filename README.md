# DocVectorSparkMinio

DocVectorSparkMinio, büyük miktarda PDF dokümanını işlemek ve bunları vektör formatına dönüştürmek için kullanılan bir Docker Compose tabanlı projedir. Projeyi kullanarak PDF dokümanlarınızı saklayabilir, işleyebilir ve vektör formatına dönüştürebilirsiniz.

## Proje Amaçları

Bu projenin ana hedefleri şunlardır:

- **Veri Saklama**: MinIO kullanarak PDF dokümanlarınızı güvenli bir şekilde saklama yeteneği sağlar. Her saat yeni dokümanlarınızı MinIO'ya yükler ve düzenler.

- **Dağıtık İşleme**: Apache Spark ile dağıtık veri işleme sağlar. Yeni dokümanlarınızı saatlik olarak izler ve işler.

- **Doküman Vektörleştirme**: PDF dokümanlarını metin verilerine dönüştürme ve ardından bu metinleri vektör formatına dönüştürme yeteneği sunar. Bu, dokümanlarınızı sayısal verilere dönüştürmek için kullanışlıdır.

- **Hızlı Doküman Yükleme**: FastAPI ile hızlı ve kolay bir şekilde yeni PDF dokümanlarınızı projeye eklemenizi sağlar.

## Kurulum

Projeyi yerel geliştirme ortamınızda çalıştırmak için aşağıdaki adımları izleyin:

### Ön Gereksinimler

- Docker
- Docker Compose
- Python 3.6+

### Kurulum Adımları

1. Bu depoyu klonlayın:

   ```bash
   git clone https://github.com/erdoganali/DocVectorSparkMinio.git
 
   cd DocVectorSparkMinio

   docker-compose up -d

   docker-compose exec docvector_app python main.py
 
 
