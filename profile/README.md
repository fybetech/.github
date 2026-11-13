# <img src="./mascot.svg" width="38" height="38" align="top" alt="Fybetech" /> Fybetech

**Küçük adımlar, büyük değişim · Small steps, big change**

Fybetech, gündelik işlere yarayan küçük uygulamalar geliştiren bağımsız bir ürün stüdyosudur. Önce kendi ihtiyacım olan uygulamayı yapıyor, sonra herkesle paylaşıyorum.

Fybetech is an independent product studio building small, focused apps for everyday life — solving my own everyday problems first, then sharing them with everyone.

---

## 🛠️ Mimari ve Teknoloji / Architecture & Stack

Ürünler üç ana katmandan oluşur; üçüncü taraf reklam, analitik veya takip SDK'sı kullanılmaz:

| Katman / Layer | Teknolojiler / Stack | Yaklaşım / Approach |
| :--- | :--- | :--- |
| **iOS (Native UI)** | SwiftUI, Asset & String Catalogs, Keychain, UserNotifications | Apple'ın kendi bileşenleriyle tam native deneyim, açık/koyu tema, TR/EN dil desteği. |
| **Shared Logic (KMP)** | Kotlin Multiplatform, SQLDelight, Ktor, Coroutines, Koin | Offline-first yerel SQLite veritabanı; tüm iş ve hesaplama kuralları tek merkezde ve testli. |
| **Backend API** | Java (LTS), Spring Boot, Spring Security, PostgreSQL, Redis | Çift yönlü (UUID upsert) senkronizasyon, sunucu doğrulamalı ilerleme hesabı. |
| **Web** | Next.js (App Router), TypeScript, Tailwind CSS, Framer Motion | İnteraktif ürün önizlemesi ve çok dilli tanıtım sitesi ([fybetech.com](https://fybetech.com)). |

---

## ⚙️ Mühendislik İlkeleri / Engineering Principles

- **Offline-First:** Tüm veriler önce cihazdaki yerel veritabanına yazılır; internet bağlantısı olduğunda arka planda eşitlenir.
- **Tek Doğruluk Kaynağı:** Hesaplama ve zamanlama kuralları hem istemcide (Kotlin) hem sunucuda (Java) birebir aynı test senaryolarıyla doğrulanır.
- **Sürekli Teslimat (CI/CD):** İzole `develop` ve `master` ortamları, otomatik testler ve sağlık kontrolü (health-check / rollback) destekli konteyner dağıtımı.

---

## 📬 İletişim / Contact

- 🌐 **Web:** [fybetech.com](https://fybetech.com)
- ✉️ **E-posta / Email:** [support@fybetech.com](mailto:support@fybetech.com)