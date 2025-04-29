Bu program, Red-Black Tree veri yapısı ve grafik (graph) temelli arkadaşlık bağlantıları kullanılarak geliştirilen bir sosyal ağ analiz sistemidir. Kullanıcılar ve onların arkadaşlık ilişkileri üzerinden çeşitli analizler yapılmasını sağlar.

📌 Program Özeti
Kullanıcılar Red-Black Tree yapısında saklanır.

Kullanıcılar arasında çift yönlü arkadaşlık bağlantıları kurulur.

DFS ile derinlik bazlı arkadaş keşfi yapılır.

Ortak arkadaşlar listelenir.

Etki alanı (etkileyebileceği kullanıcı sayısı) hesaplanır.

Topluluk tespiti ile bağlantılı bileşenler belirlenir.

Tüm kullanıcı ve arkadaşlık ilişkileri veriseti.txt dosyasına kaydedilir.

🧱 Kullanılan Veri Yapıları
Red-Black Tree: Kullanıcılar, benzersiz ID'leriyle bu dengeli arama ağacına eklenir.

Graph (Adjacency List): Kullanıcıların arkadaşları sabit boyutlu dizilerde tutulur.

▶️ Derleme ve Çalıştırma
bash
Kopyala
Düzenle
gcc sosyal_ag.c -o sosyal_ag
./sosyal_ag
💡 Kullanım Akışı
1. Kullanıcı ve Arkadaşlık Girişi
Program ilk olarak kullanıcı sayısını ister, ardından her kullanıcı için bir ID girilir.

txt
Kopyala
Düzenle
Kac kullanici eklemek istersiniz? 3
Kullanici ID girin: 1
Kullanici ID girin: 2
Kullanici ID girin: 3
Sonrasında arkadaşlık ilişkileri tanımlanır:

txt
Kopyala
Düzenle
Kac arkadaslik iliskisi tanimlanacak? 2
Arkadaslik (id1 id2): 1 2
Arkadaslik (id1 id2): 2 3
2. DFS ile Arkadaşları Listeleme
Verilen bir kullanıcıdan başlayarak en fazla 2 derinliğe kadar arkadaşlar DFS ile keşfedilir.

txt
Kopyala
Düzenle
Baslangic kullanici ID: 1
Kullanici 1 derinlik 0
Kullanici 2 derinlik 1
Kullanici 3 derinlik 2
3. Ortak Arkadaşlar
İki kullanıcı arasında ortak arkadaşlar listelenir:

txt
Kopyala
Düzenle
Ortak arkadas analizi icin iki kullanici ID girin (ID1 ID2): 1 3

Ortak Arkadaslar: 2
4. Etki Alanı Hesaplama
Belirli bir kullanıcıdan başlayarak DFS ile etkileşim kurabileceği kullanıcılar sayılır.

txt
Kopyala
Düzenle
Etki alani hesaplamak icin bir kullanici ID girin: 1

Kullanici 1 derinlik 0
Kullanici 2 derinlik 1
Kullanici 3 derinlik 2
Toplam Etki Alani: 3 kullanici
5. Topluluk Tespiti
Bağlantılı kullanıcı kümeleri (connected components) belirlenir.

txt
Kopyala
Düzenle
Topluluk: 1 2 3
📄 Veriseti Çıktısı
Program sonunda veriseti.txt adlı bir dosya oluşturulur. İçeriği şöyledir:

txt
Kopyala
Düzenle
# Kullanicilar
KULLANICI 1
KULLANICI 2
KULLANICI 3

# Arkadaslik Iliskileri
ARKADAS 1 2
ARKADAS 2 3

🛠️ Fonksiyon Açıklamaları

Fonksiyon	Açıklama
kullanici_ekle()	Yeni kullanıcı oluşturur ve Red-Black Tree'ye ekler.
arkadaslik_ekle()	İki kullanıcı arasında arkadaşlık bağlantısı kurar.
dfs()	Derinlik bazlı arkadaş taraması yapar.
ortak_arkadas()	İki kullanıcının ortak arkadaşlarını listeler.
etki_alani()	Belirli bir kullanıcıdan ulaşılabilecek kullanıcı sayısını verir.
topluluk_tespiti()	Bir kullanıcı ile bağlantılı topluluğu (connected component) yazdırır.
dosyaya_yaz()	Kullanıcı ve arkadaşlık ilişkilerini dosyaya yazar.

📌 Notlar
Maksimum kullanıcı sayısı: 100 (#define MAX_KULLANICI 100)

Dosya çıktısı sayesinde ağ verisi dış sistemlerde de kullanılabilir.

Renkli düğümler ve döndürmelerle Red-Black Tree dengeli kalır.

Hafıza yönetimi manuel yapılmaktadır (malloc).


