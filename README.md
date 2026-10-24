Discord Portföy Yönetim Botu
Discord Portföy Yönetim Botu, kullanıcıların projelerini düzenlemelerine, proje bilgilerini saklamalarına ve projelerine ait becerileri takip etmelerine yardımcı olan Python tabanlı bir Discord botudur. Bot, projeleri SQLite veritabanında saklar ve kullanıcıların Discord komutları aracılığıyla projelerini yönetmelerini sağlar.

Projenin Özellikleri
Proje ekleme = Yeni projeler oluşturmayı sağlar.
Proje listeleme = Kullanıcının projelerini görüntüler.
Proje güncelleme = Mevcut projelerin bilgilerini değiştirmeyi sağlar.
Beceri ekleme = Bir projeye Python, SQL, API veya Discord gibi beceriler ekler.
Proje silme = Seçilen projeyi veritabanından siler.
Veritabanı yönetimi = Proje bilgilerini SQLite veritabanında saklar.

Kullanılabilir Komutlar
!start = Botu tanıtır ve kullanılabilir komutları gösterir.
!info = Botun komutları hakkında bilgi verir.
!new_project = Yeni bir proje ekler. Proje adı, bağlantısı ve durumu istenir.
!projects = Kullanıcının kayıtlı projelerini listeler.
!update_projects = Seçilen projenin bilgilerini günceller.
!skills = Seçilen projeye bir beceri ekler.
!delete = Seçilen projeyi veritabanından siler.

Desteklenen Beceriler
Python = Python programlama dili.
SQL = Veritabanı sorgulama dili.
API = Uygulamalar arasında iletişim kurmayı sağlayan arayüzler.
Discord = Discord botu geliştirme becerisi.

Proje Durumları
Prototip Oluşturma = Projenin ilk taslak aşaması.
Geliştirme Aşamasında = Projenin hâlâ geliştirildiği aşama.
Tamamlandı = Projenin tamamlandığı durum.
Güncellendi = Projenin güncellendiği durum.
Bırakılmış/Desteklenmiyor = Projenin artık geliştirilmediği veya desteklenmediği durum.

Kullanılan Teknolojiler
Python = Botun geliştirildiği programlama dili.
discord.py = Discord botunun çalışmasını sağlayan kütüphane.
SQLite = Proje bilgilerinin saklandığı veritabanı.
SQL = Veritabanı işlemlerinde kullanılan sorgulama dili.

Proje Dosyaları

proje/
├── bot.py
├── logic.py
├── config.py
└── database.db

bot.py = Discord botunu ve komutlarını içerir.
logic.py = Veritabanı işlemlerini ve proje yönetimini gerçekleştirir.
config.py = Veritabanı yolunu ve Discord bot tokenini içerir.
database.db = Proje verilerinin saklandığı veritabanı dosyasıdır.

Kurulum
1. Gerekli Kütüphaneyi Yükleme

pip install discord.py

2. Yapılandırma Dosyasını Oluşturma

config.py dosyasına aşağıdaki ayarları ekleyin:

DATABASE = "database.db"
TOKEN = "DISCORD_BOT_TOKENINIZ"

Gerçek bot tokeninizi GitHub'da paylaşmayın.

3. Veritabanını Oluşturma

python logic.py

Bu komut veritabanı tablolarını oluşturur ve varsayılan becerileri ve proje durumlarını ekler.

4. Botu Çalıştırma

python bot.py

Bot Discord'a bağlandıktan sonra komutları kullanabilirsiniz.

Veritabanı Yapısı
projects = Proje adlarını, bağlantılarını, kullanıcı kimliklerini ve durumlarını saklar.
skills = Kullanılabilir becerileri saklar.
project_skills = Projeler ile beceriler arasındaki ilişkiyi saklar.
status = Proje durumlarını saklar.


Gelecekte Yapılabilecek Geliştirmeler
Proje açıklamalarının ve becerilerinin daha ayrıntılı görüntülenmesi.
Hatalı girişler için hata kontrolünün geliştirilmesi.
Projelere eklenen becerileri silme özelliğinin eklenmesi.
Proje güncelleme komutunun iyileştirilmesi.
Botun ekran görüntülerinin eklenmesi.

Proje Hakkında
Bu proje, Python ile Discord botu geliştirme ve SQLite veritabanı kullanımı konularında deneyim kazanmak ve projeleri düzenli bir şekilde yönetmek amacıyla hazırlanmıştır.
