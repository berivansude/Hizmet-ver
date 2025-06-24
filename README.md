
# Hizmet Bul - Armut Benzeri Mobil Uygulama 📱🔧

Flutter ile geliştirilen bu mobil uygulama, kullanıcıların çeşitli hizmet kategorilerinde ihtiyaçlarını belirleyip teklif verebildiği **Armut benzeri** bir sistem sunar. Kullanıcılar kayıt olabilir, giriş yapabilir ve hizmet sağlayıcılarla iletişime geçebilir.

## 🔍 Uygulama Özellikleri

- 📌 **Giriş & Kayıt Sistemi** (Firebase Authentication)
- 🏠 **Ana Ekran Hizmet Kategorileri**:
  - Ev Hizmetleri
  - Fotoğraf ve Video Hizmetleri
  - Kişisel Bakım ve Sağlık
  - Nakliye ve Taşınma
  - Organizasyon ve Etkinlik Hizmetleri
  - Teknik Hizmetler
  - Diğer Hizmetler
- 📂 **Alt Kategoriler** ile detaylı hizmet seçimi
- 📞 **Hizmet veren kişi bilgisi**, **telefon numarası** ve **verilen teklifler**
- 📝 Kullanıcının kendi teklifini oluşturma ve gönderme
- 👤 Kullanıcı Profil Sayfası (E-posta, ID, Oluşturulma tarihi, Şifre Değiştirme, Çıkış)
- 🔒 Firebase ile güvenli kullanıcı yönetimi

## 🖼 Ekran Görüntüleri

| Giriş Ekranı | Kayıt Ekranı | Profil Sayfası |
|-------------|--------------|----------------|
| ![Giriş](screenshots/giris.jpg) | ![Kayıt](screenshots/kayit.jpg) | ![Profil](screenshots/profil.jpg) |

*(Görseller `screenshots/` klasörüne eklenmelidir)*

## 🛠 Kullanılan Teknolojiler

- **Flutter (Dart)**
- **Firebase Authentication**
- **Firebase Firestore** – Kullanıcı bilgileri ve teklifler
- **Material Design**
- **State Management** – `setState`, `Navigator`, vs.

## 🗂 Veritabanı Yapısı (Firestore)

```

Koleksiyon: users

* email
* uid
* oluşturulma\_tarihi

Koleksiyon: hizmetler

* kategori: "Ev Hizmetleri"

  * alt\_kategori: "Temizlik"
  * teklif\_veren: "[berivan@gmail.com](mailto:berivan@gmail.com)"
  * teklif\_notu: "Hafta içi yapılabilir"
  * telefon: "05xxxxxxxxx"

````

## ⚙️ Kurulum Talimatları

1. Depoyu klonlayın:

```bash
git clone https://github.com/kullaniciadi/hizmet-bul-app.git
cd hizmet-bul-app
````

2. Gerekli paketleri kurun:

```bash
flutter pub get
```

3. Firebase projesi oluşturun:

   * Firebase Console’da yeni bir proje oluşturun.
   * **Authentication** sekmesinden e-posta/şifre girişini aktif edin.
   * **Cloud Firestore**’u başlatın.
   * `google-services.json` dosyasını `android/app/` klasörüne ekleyin.

4. Uygulamayı çalıştırın:

```bash
flutter run
```

## 🧑‍💻 Geliştirici

* **Adı Soyadı**: Berivan Sude Gün
* 📧 **İletişim**: [berivan@gmail.com](mailto:berivan@gmail.com)
* 🎯 **Amacı**: Armut benzeri bir hizmet platformu geliştirme

## ⚠️ Notlar

* Bu uygulama örnek geliştirme projesidir.
* Kategoriler ve teklif yapısı sade tutulmuştur, geliştirilmeye açıktır.
* Uygulama Firebase ile tam entegredir ancak Firebase güvenlik kuralları düzenlenmeden yayına alınmamalıdır.

## 📄 Lisans

Bu proje MIT lisansı ile yayınlanmıştır.


