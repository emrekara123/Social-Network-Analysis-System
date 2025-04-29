Bu program, Red-Black Tree veri yapısı ve grafik (graph) temelli arkadaşlık bağlantılarını kullanarak geliştirilen bir sosyal ağ analiz sistemidir. Kullanıcılar ve onların arkadaşlık ilişkileri üzerinden çeşitli analizler yapılmasını sağlar.

🧾 Program Özeti
Kullanıcılar Red-Black Tree yapısına aktarılır.

Kullanıcılar arası doğrudan ve dolaylı arkadaşlık bağlantıları kurulur.

DFS ile grafik analizi yapılır.

Ortak arkadaşlar listelenir.

Belirli kullanıcılar arasındaki bağlantı sayısı hesaplanır.

Topluluk (community) tespiti yapılır.

Tüm kullanıcılar ve ilişkileri .txt dosyasına kaydedilir.

🗂 Kullanılan Veri Yapıları
Red-Black Tree: Kullanıcılar, benzersiz ID’leriyle bu dengeli arama ağacına eklenir.

Graph (Adjacency List): Kullanıcıların arkadaşları ağı şeklinde temsil edilir.

🛠 Derleme ve Çalıştırma
bash
Kopyala
Düzenle
gcc sosyal_ag.c -o sosyal_ag_anayol_ag
👣 Kullanım Akışı
Kullanıcı ve Arkadaşlık Girişi:

Kullanıcı eklemek istenir: 3 kullanıcı ID girilir → 1. Kullanıcı ID → 2. Kullanıcı ID → 3. Kullanıcı ID

Arkadaşlık Tamamlama:

Kaç arkadaşlık ilişkisi tanımlanacak?

2 arkadaş ID girilir → 1. kullanıcı → 2. kullanıcı

DFS ile Arkadaşlık İlişkisi Analizi:

Kaç defa yapılacak?

Her analiz için 2 kullanıcı ID girilir.

Ortak Arkadaşlar:

2 kullanıcı ID girilir.

Belli Arama Mesafesi:

Kaç işlem yapılacak?

Her işlemde 3 kullanıcı ID girilir.

Topluluk Tespiti:

Topluluk sayısı belirlenir.

🔧 Fonksiyon Açıklamaları
Açıklama
kullanici_ekle(): Yeni kullanıcı oluşturur ve Red-Black Tree’ye ekler.

arkadas_ekle(): İki kullanıcı arasında arkadaşlık bağlantısı kurar.

dfs(): Derinlik bazlı arkadaş taraması yapar.

ortak_arkadaslar(): Ortak arkadaşları listeler.

etki_alani(): Belirli bir kullanıcıya dolaylı/dolaysız ulaşabilecek kullanıcıları verir.

topluluk_tespit(): DFS kullanarak ayrık kullanıcı gruplarını belirler.

dosyaya_yaz(): Kullanıcı ve arkadaşlık bilgilerini .txt dosyasına kaydeder.

📌 Notlar
Maksimum kullanıcı sayısı: 100 (#define MAX_KULLANICI 100)

Her kullanıcı benzersiz bir ID ile tanımlanır.

Red-Black Tree yapısı dinamik dengelenmiş ağaç olduğu için hızlı arama sağlar.

Arkadaşlık bağlantıları çift yönlüdür.

📁 Çıktı Dosyaları
kullanicilar.txt: Tüm kullanıcılar ve ilişkileri burada listelenir.

Programdan çıkış yapıldığında otomatik oluşturulur.

Kullanıcılar, ID’leri ve arkadaşları ile birlikte kayıt edilir.

Dosyada son yapılan işlemler güncellenmiş olarak yer alır.

Yukarıdaki metni README.md dosyanıza yapıştırarak kullanabilirsiniz. İsterseniz bir .md dosyasına dönüştürüp gönderebilirim. Devam edeyim mi?
