# ESTella Ecosystem
## User Profile & Account Management — UI/UX Design Specification

**Project:** ESTella Mobile Application  
**Module:** User Profile & Account Management  
**Version:** 2.4

---

# 1. Project Overview

## Məqsəd

İstifadəçi autentifikasiyadan keçdikdən sonra alt menyunun (Bottom Navigation Bar) ən sağındakı **Profil** tabına daxil olur.

Bu bölmə istifadəçinin şəxsi məlumatlarını, təhlükəsizlik parametrlərini, rezervasiya tarixçəsini, aktiv cihazlarını və tətbiq tənzimləmələrini idarə etdiyi mərkəzdir.

Bütün ekranlar tətbiqin mövcud Design System-inə uyğun hazırlanmalıdır. Light Mode və Dark Mode dəstəyi nəzərə alınmalıdır.

---

# 2. ESTella Brand Identity & Design System

## 2.1 Brand Colors

ESTella loqosunda istifadə olunan orijinal rənglər qorunmalıdır.

| Color Name | HEX Code | Usage |
|---|---|---|
| Primary Emerald Green | #0B4C34 | Primary buttons, active states, icons |
| Gold Accent | #B79240 | Logo accents, highlights, badges |
| White | #FFFFFF | Main background |
| Light Mint | #F0F6F2 | Secondary backgrounds |
| Soft Green | #F6F9F6 | Cards and input backgrounds |
| Main Text | #202A24 | Headings and primary text |
| Secondary Text | #7A857E | Descriptions and labels |
| Error Red | #D94B4B | Errors and destructive actions |
| Success Green | #23865C | Success feedback |

## 2.2 Visual Style

- Modern, minimal and premium interface.
- Emerald green as the primary brand color.
- Gold used for subtle decorative details.
- Clean white and light mint backgrounds.
- Rounded cards and input fields.
- Consistent typography.
- Clear visual hierarchy.
- Minimal line icons.
- Soft shadows and subtle borders.
- Consistent spacing system: 4, 8, 12, 16, 24, 32 px.

**Important:** Do not change the original ESTella logo or its colors.

---

# 3. Information Architecture (Sitemap)

Profil bölməsinin strukturuna aşağıdakı ekranlar daxildir:

1. Profil Əsas Ekranı (Dashboard)
2. Şəxsi Məlumatların Redaktəsi
3. Rezervasiya və Sifarişlər
4. Təhlükəsizlik və Hesab
5. Aktiv Sessiyalar / Cihazlar
6. Tətbiq Tənzimləmələri
7. Hüquqi Məlumatlar və Dəstək

## 3.1 Screen Structure

### A. Profil Əsas Ekranı (Dashboard)

- Avatar
- Ad və Soyad
- Telefon nömrəsi
- VIP / Loyallıq statusu
- Sürətli keçid kartları

### B. Şəxsi Məlumatların Redaktəsi

- Ad
- Soyad
- E-poçt
- Doğum tarixi
- Cins
- Profil şəklinin dəyişdirilməsi

### C. Rezervasiya və Sifarişlər

- Aktiv görüşlər
- Keçmiş tarixlər
- Ləğv olunan rezervasiyalar
- Rezervasiya detal səhifəsi

### D. Təhlükəsizlik və Hesab

- Şifrə dəyişimi
- İki mərhələli doğrulama (2FA)
- Biometrik giriş (Face ID / Touch ID)

### E. Aktiv Sessiyalar / Cihazlar

- Cari cihaz
- Digər daxil olunmuş cihazlar
- Sessiyanın sonlandırılması

### F. Tətbiq Tənzimləmələri

- Dil seçimi: AZ, EN, RU
- Push bildirişləri
- SMS bildirişləri
- Email bildirişləri
- Tema: Light / Dark / System

### G. Hüquqi Məlumatlar və Dəstək

- İstifadə şərtləri
- Məxfilik siyasəti
- Dəstəklə əlaqə (Chat / FAQ)
- Hesabın silinməsi

---

# 4. Screen 01 — Profil Əsas Ekranı (Dashboard)

Bu ekran istifadəçinin profil bölməsinə daxil olduqda gördüyü əsas idarəetmə panelidir.

## 4.1 Header / Masthead

- Sol yuxarıda səhifə başlığı: "Profil"
- Sağ tərəfdə Ayarlar (Gear) ikonu.
- Client-side navigation.

## 4.2 User Profile Card

- Dairəvi profil şəkli (Avatar).
- Avatar üzərində kiçik redaktə / qələm ikonu.
- Ad və Soyad.
- Telefon nömrəsi.
- VIP / Loyallıq status nişanı.

**API Endpoint:** `GET /api/v1/user/profile`

## 4.3 Quick Statistics

Üç statistik göstərici:

1. Aktiv Rezervasiyalar
2. Qazanılmış Bonuslar (Cashback)
3. Sevimli Salonlar

**API Endpoint:** `GET /api/v1/user/stats`

## 4.4 Menu List

Hər menyu elementində ikon, başlıq və sağ tərəfdə keçid oxu (Chevron) olmalıdır.

Menyu elementləri:

- Şəxsi Məlumatlar
- Rezervasiyalarım
- Təhlükəsizlik
- Cihazlar
- Bildirişlər
- Dəstək
- Çıxış (Logout)

Navigation: Static menu / Route redirect.

---

# 5. Screen 02 — Təhlükəsizlik və Cihazların İdarə Edilməsi

İstifadəçi hesabının qorunması və aktiv sessiyaların izlənməsi üçün aşağıdakı komponentlər hazırlanmalıdır.

## 5.1 Şifrə Dəyişimi

Input sahələri:

- Cari şifrə
- Yeni şifrə
- Yeni şifrənin təkrarı

Tələblər:

- Hər şifrə sahəsində Show / Hide Password ikonu olmalıdır.
- Şifrə gücü indikatoru əlavə edilməlidir.
- Progress bar vasitəsilə Zəif / Güclü şifrə vəziyyətləri göstərilməlidir.

## 5.2 İki Mərhələli Doğrulama (2FA)

- Toggle (Açıq / Bağlı) düyməsi.
- İstifadəçi 2FA funksiyasını aktiv və ya deaktiv edə bilməlidir.
- Deaktiv edildikdə SMS təsdiq kodu tələb olunur.

## 5.3 Aktiv Sessiyalar Siyahısı

Hər cihaz üçün aşağıdakı məlumatlar göstərilməlidir:

- Cihaz adı (məsələn: iPhone 15 Pro).
- IP ünvanı.
- Son giriş tarixi.
- Cihazın yerləşdiyi yer.

Cari cihaz "Bu cihaz" (Current Device) etiketi ilə göstərilməlidir.

Hər cihaz sətrinin sağ tərəfində:

- "Sessiyanı sonlandır" düyməsi.
- Qırmızı rəngdə destructive action.

---

# 6. Screen 03 — Tətbiq Tənzimləmələri

## 6.1 Language Settings

İstifadəçi aşağıdakı dillərdən birini seçə bilməlidir:

- Azərbaycan dili (AZ)
- English (EN)
- Русский (RU)

## 6.2 Notification Settings

Bildirişlər ayrıca idarə olunmalıdır:

- Push Notifications
- SMS Notifications
- Email Notifications

Hər biri üçün aktiv / deaktiv Toggle istifadə edilməlidir.

## 6.3 Theme Settings

Üç seçim olmalıdır:

- Light Mode
- Dark Mode
- System Default

Light və Dark Mode üçün ESTella brend rəngləri qorunmalıdır.

---

# 7. Screen 04 — Loading, Empty, Error & Success States

Hər bir ekran üçün aşağıdakı xüsusi vəziyyətlər prototipdə hazırlanmalıdır.

## 7.1 Loading State

- Məlumatlar yüklənərkən Skeleton Loader animasiyası göstərilməlidir.
- Skeleton həm profil kartında, həm də siyahılarda istifadə olunmalıdır.

## 7.2 Empty State

Rezervasiyalar və ya aktiv sessiya siyahısı boş olduqda:

- Mərkəzləşdirilmiş illüstrasiya.
- Başlıq: "Hələ ki heç nə yoxdur".
- İzahat mətni.

## 7.3 Error / Failure State

API xətası zamanı:

- Ekranın yuxarısında qırmızı fonlu Toast bildirişi və ya Modal.
- Mesaj: "Bağlantı xətası, yenidən cəhd edin".

## 7.4 Success Feedback

Məlumatlar uğurla yeniləndikdə:

- Yaşıl rəngli Toast mesajı.
- Və ya qısa konfetti animasiyası.
- Xüsusilə şəxsi məlumatlar dəyişdirildikdə göstərilməlidir.

---

# 8. Screen 05 — Hesabın Silinməsi və Çıxış Axını

## 8.1 Logout — Hesabdan Çıxış

Logout əməliyyatı Bottom Sheet vasitəsilə göstərilməlidir.

Təsdiq mətni:

"Hesabdan çıxmaq istədiyinizə əminsinizmi?"

Düymələr:

- "Ləğv et"
- "Çıxış et" — qırmızı rəngdə.

İstifadəçi əməliyyatı təsdiqləmədən hesabdan çıxarılmamalıdır.

## 8.2 Delete Account — Hesabın Silinməsi

- Təhlükəsizlik səhifəsinin ən aşağı hissəsində yerləşdirilməlidir.
- İstifadəçi hesabı silmək üçün xəbərdarlıq səhifəsinə yönləndirilməlidir.
- Şifrənin daxil edilməsi və ya SMS kodu ilə təsdiqləmə tələb olunmalıdır.
- Proses tamamlandıqdan sonra istifadəçinin məlumatları bazadan silinməlidir.
- Tətbiq ilkin qeydiyyat ekranına qayıtmalıdır.

---

# 9. Navigation & Interaction Requirements

Bütün ekranlar arasında keçidlər düzgün qurulmalıdır.

Əsas Profil menyusundan:

- Şəxsi Məlumatlar → Profil məlumatlarının redaktəsi.
- Rezervasiyalarım → Rezervasiya tarixçəsi.
- Təhlükəsizlik → Şifrə, 2FA və biometrik giriş.
- Cihazlar → Aktiv sessiyalar.
- Bildirişlər → Bildiriş parametrləri.
- Dəstək → Chat / FAQ.
- Çıxış → Logout Bottom Sheet.

Bütün düymələr, ikonlar, Toggle-lar və keçidlər funksional prototipdə göstərilməlidir.

---

# 10. Technical & Design Requirements

- Mobile-first design.
- Existing ESTella Design System ilə tam uyğunluq.
- Light Mode və Dark Mode dəstəyi.
- Backend API strukturuna uyğun UI.
- Consistent spacing and typography.
- Reusable components.
- Consistent icon style.
- Proper input validation.
- Clear error and success feedback.
- Accessible touch targets.
- Responsive layouts.

---

# 11. Final Design Instructions for Stitch

Create all screens described in this document as separate mobile frames.

IMPORTANT:

1. Preserve the original ESTella logo.
2. Use the exact brand colors #0B4C34 and #B79240.
3. Use emerald green for primary actions and active states.
4. Use gold only for subtle accents, badges and highlights.
5. Keep the interface fresh, minimal, elegant and premium.
6. Maintain visual consistency with the existing ESTella Home, Authentication, Splash and Onboarding screens.
7. Do not use blue as the primary color.
8. Do not remove any requested functionality.
9. Design all required interaction states.
10. Keep all interface text in Azerbaijani.
11. Create separate screens for all major sections.
12. Do not combine the entire profile system into one overloaded screen.

**Final Goal:** Build a complete, professional ESTella User Profile & Account Management experience with a consistent design system, clear navigation, intuitive interactions and a premium emerald-green and gold visual identity.
