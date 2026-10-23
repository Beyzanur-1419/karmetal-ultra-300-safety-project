# Karmetal ULTRA 300x300 Otomatik Şerit Testere - SWOT Analizi
**Hazırlayan:** Beyza Nur Ozanalp (Gündüz 4B)
**Standartlar:** IEC 62443 & Safety 4.0

## 1. Strengths (Güçlü Yönler)
- **Donanımsal Bağımsız Emniyet Mimarisi:** Acil stoplar, kapı switch'leri ve şerit kopma sensörleri doğrudan donanımsal Safety PLC ve STO (Safe Torque Off) devresine bağlıdır.
- **Yüksek Hassasiyetli Hidrolik ve Mekanik Yapı:** Otomatik malzeme sürme ve hidrolik mengene sıkıştırma sistemleri mekanik kararlılık sağlar.
- **Yerli Üretim Avantajı:** Karmetal üretimi olması sayesinde hızlı yedek parça ve teknik servis desteği.

## 2. Weaknesses (Zayıf Yönler)
- **Açık IoT / Uzak Bakım Modülü:** Kestirimci bakım için internete veya kurumsal ağa doğrudan bağlı modem/router barındırması.
- **Zayıf / Varsayılan Kimlik Doğrulama:** HMI ve PLC arayüzlerinde fabrika çıkışlı standart parolaların kullanılması riski.
- **Korunmasız Bakım Portları:** Kontrol paneli üzerindeki USB portlarının fiziksel kilidinin bulunmaması.

## 3. Opportunities (Fırsatlar)
- **Sıfır Güven (Zero Trust) ve VPN Entegrasyonu:** Uzak bakım hattına IPsec/SSL VPN ve Jump Server mimarisinin entegre edilmesi.
- **Rol Tabanlı Erişim (RBAC) ve Loglama:** Teknisyenlerin kişisel hesaplar ve MFA ile giriş yaparak tüm işlemlerin "Audit Log" olarak kaydedilmesi.
- **Endüstri 4.0 Güvenlik Farkındalığı:** Güvenli bulut mimarileriyle şifrelenmiş veri aktarımı sağlanması.

## 4. Threats (Tehditler)
- **Uzak Erişimin Kötüye Kullanımı:** Uzak bakım modülü üzerinden sızılarak hidrolik mengene basınçlarının veya kesim parametrelerinin manipüle edilmesi.
- **Fiziksel Yaralanma Riski (S=3):** Yazılımsal zafiyetler nedeniyle operatör malzeme yüklerken mengenenin ani kapanması veya şerit fırlaması (ciddi uzuv kaybı riski).
- **Zararlı Yazılım Tehditleri:** Fabrika içi ağa sızan fidye yazılımlarının HMI ve PLC'yi kilitlemesi.
