# 👥 Sosyal Ağ Tabanlı Kullanıcı Yönetim ve Analiz Sistemi

Bu program, Red-Black Tree veri yapısı kullanılarak kullanıcıların yönetimi ve sosyal ağ üzerindeki arkadaşlık ilişkileri analiz edilir. Topluluk tespiti gibi analizleri yapar. Bu çıktılar oluşturulan veriler `.txt` dosyasına kaydedilir.

---

## ⚙️ Özellikler

- Red-Black Tree ile kullanıcı ekleme ve arama
- Arkadaşlık ilişkileri tanımlama
- DFS ile derinlik tabanlı dolaşım
- Ortak arkadaş analizi
- Etki alanı (influence area) hesaplama
- Topluluk tespiti
- Verileri dosyaya kaydetme ve güncelleme

---

## 1. 👤 Kullanıcı ve Arkadaşlık Tanımı

Kullanıcı sayısı ve her bir kullanıcı için ID bilgisi alındıktan sonra, arkadaşlık ilişkileri tanımlanır.

![image](https://github.com/user-attachments/assets/06ab79f8-6653-4b08-a0bf-9aae47db188a)


---

## 2. 🔍 DFS ile Derinlik Bazlı Gezinme

Bir kullanıcının başlangıçtan 2 derinliğe kadar olan arkadaşları ekrana yazdırılır.

![image](https://github.com/user-attachments/assets/f1f2720c-6e33-4e10-9647-c80608b99c01)


---

## 3. 👥 Ortak Arkadaş Analizi

İki kullanıcının arasındaki ortak arkadaşlar ekrana yazdırılır.

![image](https://github.com/user-attachments/assets/95e51a9d-d1b6-48bb-99a2-db4d4ea16017)


---

## 4. 🌐 Etki Alanı Hesaplama

Bir kullanıcının kaç farklı kullanıcıyı doğrudan veya dolaylı etkileyebildiği hesaplanır.

![image](https://github.com/user-attachments/assets/d702c6db-4009-4018-b646-3b3c84bfcfa2)

---

## 5. 🧩 Topluluk Tespiti

Graf üzerinde ayrık kullanıcı grupları belirlenir. Her grup ayrı bir topluluk olarak listelenir.
![image](https://github.com/user-attachments/assets/bc5aea09-d9ab-4ad3-8066-9880f8429630)

---

## 📁 Kullanılan Veri Yapıları

- **Red-Black Tree**: Kullanıcılar, benzersiz ID’leriyle bu dengeli arama ağacına eklenir.
- **Graph (Adjacency List)**: Kullanıcıların arkadaşları, bağlantı listeleri şeklinde tutulur.

---

## 🔄 Kullanım Akışı (Özet)

- **Kullanıcı ve Arkadaşlık Girişi**  
  Kullanıcı eklemek istenir: 3 kullanıcı ID girilir → 1. Kullanıcı ID → 2. Kullanıcı ID → 3. Kullanıcı ID  

- **Arkadaşlık Tanımlama**  
  Kaç arkadaşlık ilişkisi tanımlanacak?  
  2 arkadaş ID girilir → 1. kullanıcı → 2. kullanıcı

- **DFS ile Arkadaşlık İlişkisi Analizi**  
  DFS derinlik girilir → Hedef kullanıcıya ulaşılır.

- **Ortak Arkadaşlar**  
  İki kullanıcı girilir → Ortak olanlar listelenir.

- **Etki Alanı**  
  Belirli kullanıcıdan erişilebilen kullanıcılar listelenir.

- **Topluluk Tespiti**  
  DFS ile ayrık bileşenler tespit edilir.

- **Veri Kaydı**  
  `veriseti.txt` dosyasına tüm kullanıcı ve arkadaşlık bilgileri yazılır.

---

## 🗃 Çıktı Dosyası: `veriseti.txt`

- Kullanıcılar ve arkadaşlıkları tutulur.
- Her işlem sonunda güncellenerek üzerine yazılır.
- Yapı şu şekildedir:
- ![image](https://github.com/user-attachments/assets/f9adfd9c-4747-414b-a212-560d48c1bbe6)











