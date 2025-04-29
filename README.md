Bu program, Red-Black Tree veri yapısı ve grafik (graph) temelli arkadaşlık bağlantıları kullanılarak geliştirilen bir sosyal ağ analiz sistemidir. Kullanıcılar ve onların arkadaşlık ilişkileri üzerinden çeşitli analizler yapılmasını sağlar.

## 📌 Program Özeti

- Kullanıcılar Red-Black Tree yapısında saklanır.
- Kullanıcılar arasında çift yönlü arkadaşlık bağlantıları kurulur.
- DFS ile derinlik bazlı arkadaş keşfi yapılır.
- Ortak arkadaşlar listelenir.
- Etki alanı (etkileyebileceği kullanıcı sayısı) hesaplanır.
- Topluluk tespiti ile bağlantılı bileşenler belirlenir.
- Tüm kullanıcı ve arkadaşlık ilişkileri `veriseti.txt` dosyasına kaydedilir.

## 🧱 Kullanılan Veri Yapıları

- **Red-Black Tree**: Kullanıcılar, benzersiz ID’leriyle bu dengeli arama ağacına eklenir.
- **Graph (Adjacency List)**: Kullanıcıların arkadaşları sabit boyutlu dizilerde tutulur.

## ▶️ Derleme ve Çalıştırma

```bash
gcc sosyal_ag.c -o sosyal_ag
./sosyal_ag
