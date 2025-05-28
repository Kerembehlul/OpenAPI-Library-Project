# 📘 OpenAPI Tasarımı Ödevi Teslim Raporu

---

## 👤 Öğrenci Bilgileri

| Alan              | Bilgi               |
|-------------------|---------------------|
| **Ad Soyad**      | Kerem Behlül Yeşil     |
| **Öğrenci Numarası** | 170422054 |

---

## 📂 OpenAPI YAML Dosyası

- `openapi.yaml` dosyası başarıyla hazırlanmış ve Swagger Editor üzerinde test edilmiştir.
- API sürümü: `3.0.3`
- Sunucu adresi: `http://localhost:8080/api`

### 🔗 GitHub Repo Linki

👉 [https://github.com/Kerembehlul/OpenAPI-Library-Project](https://github.com/Kerembehlul/OpenAPI-Library-Project)

---

## 📝 API Açıklaması

### 📌 Varlıklar (Entities)

- **📚 Books**
  - `id`, `title`, `author`, `isbn`, `publisher`, `pageCount`, `stock`
- **👤 Students**
  - `id`, `name`, `studentNumber`, `email`, `isActive`
- **🔄 Loans**
  - `id`, `studentId`, `bookId`, `loanDate`, `returnDate`, `status`

### 🔧 CRUD İşlemleri

Her varlık için CRUD işlemleri REST prensiplerine uygun olarak tanımlanmıştır:

| Varlık     | Endpoint Örnekleri                          |
|------------|---------------------------------------------|
| Books      | `GET /books`, `POST /books`, `PUT /books/{id}`, `DELETE /books/{id}` |
| Students   | `GET /students`, `POST /students`, `PUT /students/{id}`, `DELETE /students/{id}` |
| Loans      | `GET /loans`, `POST /loans`, `PATCH /loans/{id}/return` |

### 🧩 Kullanılan OpenAPI Özellikleri

- `components/schemas` altında tüm veri modelleri tanımlandı.
- `parameters` içinde `page`, `size` gibi query parametreleri tanımlandı.
- `responses` altında `200`, `201`, `400`, `404`, `500` gibi cevap türleri örneklerle yer aldı.
- `example` kullanımı en az bir endpointte sağlandı.
- `GET /books` endpointi sayfalama (`page`, `size`) desteklidir.
- `description`, `tags` açıklayıcı şekilde yazıldı.

---

## 🧪 Test Notları (Opsiyonel)

| Endpoint          | Sonuç / Açıklama |
|-------------------|------------------|
| `GET /books`      | Tüm kitapları listeler (sayfalama destekli) |
| `POST /students`  | Yeni öğrenci ekler, `email` ve `studentNumber` zorunludur |
| `PATCH /loans/{id}/return` | Kitap iadesini gerçekleştirir |
| Hatalı istek (`GET /books/1234`) | `404 Not Found` döner |

---

## 📌 Ek Açıklamalar

- Dosya Swagger Editor üzerinde test edilmiştir, geçerlilik kontrolünden başarıyla geçmiştir.
- Teslim dosyası olarak yalnızca bu `DELIVERY.md` belgesi Google Classroom’a yüklenecektir.

---

## 🎓 Ders Bilgisi

- **Ders**: Açık Kaynak Kodlu Yazılımlar  
- **Teslim Tarihi**: 28.05.2025  
- **Teslim Yeri**: Google Classroom

---

## ✅ Özet

> Bu ödev kapsamında OpenAPI 3.0.3 standardına uygun, çevrimiçi bir üniversite kütüphanesi REST API’si tasarlanmış; gerekli endpoint'ler, veri şemaları, sayfalama, hata yanıtları ve örnekler eksiksiz olarak belirtilmiştir.

---

