# Ziyaretçi Yönetim Sistemi

Python ile geliştirilmiş, etkinlik katılımcı kayıtlarını ve güvenli giriş kodlarını yönetmeye yönelik ziyaretçi yönetim sistemi.

## Genel Bakış

Bu proje, bir yazılım festivali organizasyonunda kullanılabilecek temel bir ziyaretçi yönetim senaryosunu modellemek amacıyla geliştirilmiştir.

Uygulama, katılımcıların kayıt altına alınmasını, kayıtlı katılımcı bilgilerinin sorgulanmasını ve katılımcılar için giriş kodu ile güvenlik şifresi oluşturulmasını sağlar.

## Özellikler

- Yeni katılımcı kaydı oluşturma
- Katılımcı bilgilerini ID üzerinden sorgulama
- Katılımcılar için otomatik giriş kodu oluşturma
- Katılımcılar için güvenlik şifresi oluşturma
- Kullanıcı girişi ile anlık giriş kodu ve güvenlik şifresi oluşturma
- Katılımcı bilgilerinin dosya üzerinde saklanması
- Komut satırı üzerinden menü tabanlı kullanıcı etkileşimi

## Proje Yapısı

```text
ZiyaretciYonetimSistemi/
├── main.py
├── islemler.py
├── README.md
└── .gitignore
```

### Dosya Açıklamaları

- `main.py` — Uygulamanın ana giriş noktasıdır ve kullanıcı menüsünü yönetir.
- `islemler.py` — Katılımcı kayıtları, bilgi sorgulama ve giriş kodu/güvenlik şifresi oluşturma gibi işlemleri içerir.

## Kullanılan Teknolojiler

- Python
- Dosya İşlemleri
- Komut Satırı Arayüzü (CLI)

## Sistem Akışı

Uygulama, kullanıcıya menü üzerinden farklı işlemler sunar.

Temel akış:

```text
Kullanıcı
   │
   ▼
Ana Menü
   │
   ├── Yeni Katılımcı Kaydı
   │
   ├── Katılımcı Sorgulama
   │
   ├── Giriş Kodu / Güvenlik Şifresi Oluşturma
   │
   └── Kullanıcı Girişi
```

Katılımcı kaydı sırasında gerekli bilgiler alınarak ilgili kayıt oluşturulur. Katılımcıların sistem içerisinde ayırt edilebilmesi için ID bilgileri kullanılır.

## Güvenlik Kodu Yönetimi

Sistem, katılımcılar için giriş işlemlerinde kullanılmak üzere otomatik olarak giriş kodu ve güvenlik şifresi oluşturur.

Bu mekanizma, etkinlik girişlerinin temel seviyede kontrol edilmesini ve katılımcıların oluşturulan bilgiler üzerinden doğrulanabilmesini simüle eder.

> Not: Bu proje eğitim amaçlı bir uygulamadır. Kullanılan giriş kodu ve güvenlik mekanizmaları gerçek bir üretim ortamında kullanılmak üzere tasarlanmamıştır.

## Veri Yönetimi

Projenin mevcut yapısında katılımcı bilgileri ve oluşturulan kodlar metin dosyaları üzerinden saklanmaktadır.

Gerçek kişilere ait katılımcı verileri veya gerçek giriş/güvenlik bilgileri public repository içerisinde tutulmamalıdır.

## Projenin Amacı

Bu projenin temel amacı, Python kullanarak gerçek hayattan bir etkinlik yönetimi senaryosunu modellemek ve temel programlama konularını uygulamaktır.

Proje kapsamında:

- Fonksiyonlar
- Koşul ifadeleri
- Kullanıcı girdileri
- Dosya işlemleri
- Rastgele veri üretimi
- Menü tabanlı program yapısı
- Modüler Python dosya yapısı

gibi konularda pratik yapılmıştır.

## Proje Durumu

Bu proje, Python programlama temellerini ve dosya tabanlı veri yönetimini pekiştirmek amacıyla geliştirilmiş eğitim amaçlı bir uygulamadır.

Üretim ortamına hazır kapsamlı bir ziyaretçi yönetim sistemi olarak tasarlanmamıştır.

Gelecekte geliştirilebilecek özellikler:

- Veritabanı entegrasyonu
- Gerçek kullanıcı kimlik doğrulama sistemi
- Ziyaretçi giriş ve çıkış zamanlarının takibi
- Yetkilendirme ve rol yönetimi
- QR kod tabanlı giriş sistemi
- Grafiksel veya web tabanlı kullanıcı arayüzü

## Çalıştırma

Repository'yi klonladıktan sonra ana Python dosyasını çalıştırabilirsiniz:

```bash
python main.py
```
