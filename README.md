# SQLink - SierraEcho & Team Hotspot System
### Powered by SvxLink | Developed by SQ7UTP

Witamy w oficjalnym repozytorium dystrybucyjnym obrazów systemowych dla hotspotów **SQLink**.
System oparty jest na stabilnym Debianie oraz oprogramowaniu SvxLink, zoptymalizowany do pracy w sieci **SQLink - SierraEcho & Team**.

---

## 🚀 Szybki Start / Quick Start

### 🔐 Loginy i Hasła / Credentials

| Usługa / Service | Login / User | Hasło / Password | Adres / Address |
| :--- | :--- | :--- | :--- |
| **Terminal (SSH)** | `root` | `sqlink` | Port: 22 |
| **Dashboard WWW** | *(brak / none)* | *(brak / none)* | `http://sqlink.local` lub IP |
| **Hotspot WiFi (AP)**\* | -- | `sqlink123` | SSID: **SQLink_WiFi_AP** |

*\*Tryb Hotspot WiFi (AP) dotyczy tylko wersji Raspberry Pi Zero W przy pierwszym uruchomieniu.*

---

## 📥 Pobieranie / Downloads

Gotowe obrazy systemu (`.img`) spakowane w archiwum znajdziesz w zakładce **Releases** po prawej stronie.

👉 **[PRZEJDŹ DO POBIERANIA / GO TO RELEASES](https://github.com/SQLinkgit/SQLink-Official/releases)**

Dostępne wersje dla:
1.  **Raspberry Pi Zero W**
2.  **Orange Pi Zero (v1)**

---

## 🇵🇱 Instrukcja Instalacji

### 1. Wgrywanie obrazu
1. Pobierz odpowiedni plik obrazu z sekcji "Releases".
2. Rozpakuj archiwum (np. programem 7-Zip).
3. Użyj programu **Balena Etcher** lub **Rufus**, aby nagrać plik `.img` na kartę pamięci microSD (zalecane min. 8GB, Class 10).

### 2. Pierwsze uruchomienie
Włóż kartę do urządzenia i podłącz zasilanie.

* **Dla Orange Pi Zero:** Podłącz kabel sieciowy (Ethernet). Urządzenie pobierze IP z Twojego routera.
* **Dla Raspberry Pi Zero W:** Urządzenie uruchomi własną sieć WiFi.
    > **⚠️ Ważna uwaga:** Pierwsze uruchomienie i konfiguracja systemu trwa chwilę. Prosimy o cierpliwość – sieć WiFi o nazwie **SQLink_WiFi_AP** pojawi się po około **3 minutach** od włączenia zasilania.
    
    1. Wyszukaj w telefonie/laptopie sieć WiFi: **SQLink_WiFi_AP**
    2. Połącz się hasłem: **sqlink123**
    3. Wpisz w przeglądarce adres: **http://192.168.4.1** lub **http://sqlink.local**
    4. Skonfiguruj swoją domową sieć WiFi w panelu.

### 3. Dostęp do Dashboardu
Po podłączeniu do sieci, wpisz w przeglądarce:
> **http://sqlink.local/**

Jeśli adres nie działa, znajdź adres IP urządzenia na routerze lub użyj skanera sieciowego (np. "Advanced IP Scanner" lub aplikacji na telefon "Fing").

### 4. Aktualizacje (OTA)
System posiada wbudowany mechanizm aktualizacji. W dashboardzie znajdziesz opcję aktualizacji, która automatycznie pobiera najnowsze poprawki z naszych repozytoriów technicznych.

---

## 🇬🇧 Installation Guide

### 1. Flashing the Image
1. Download the appropriate image file from the "Releases" section.
2. Unzip the archive.
3. Use **Balena Etcher** or **Rufus** to burn the `.img` file to a microSD card (min. 8GB, Class 10 recommended).

### 2. First Boot
Insert the card into the device and power it on.

* **For Orange Pi Zero:** Connect an Ethernet cable. The device will get an IP from your router.
* **For Raspberry Pi Zero W:** The device will start in Access Point (AP) mode.
    > **⚠️ Important Note:** The initial boot and system configuration take a moment. Please be patient – the WiFi network named **SQLink_WiFi_AP** will appear approximately **3 minutes** after powering on.

    1. Search for WiFi network: **SQLink_WiFi_AP**
    2. Connect using password: **sqlink123**
    3. Open browser and go to: **http://192.168.4.1** or **http://sqlink.local**
    4. Configure your home WiFi via the dashboard.

### 3. Dashboard Access
After connecting to the network, type in your browser:
> **http://sqlink.local/**

If this address does not work, find the device IP address on your router or use a network scanner (e.g., "Advanced IP Scanner" or "Fing" app).

---

## 📜 Licencja i Źródła / License & Source Code

Oprogramowanie udostępniane jest na licencji **GNU GPL v3.0**.
This software is provided under the **GNU GPL v3.0** license.

**Kod źródłowy oraz skrypty systemowe są dostępne w naszych repozytoriach technicznych:**
**Source code and system scripts are available in our technical repositories:**

* 📂 **Raspberry Pi Zero W:** [github.com/sqlinkgit/SQLink_RPI0W-Update](https://github.com/sqlinkgit/SQLink_RPI0W-Update)
* 📂 **Orange Pi Zero:** [github.com/sqlinkgit/SQLink_OPI0V1-Update](https://github.com/sqlinkgit/SQLink_OPI0V1-Update)

### Credits
* **SQLink - SierraEcho & Team** - Community & Infrastructure
* **SQ7UTP** - System & Dashboard Developer
* **Tobias Blomberg (SM0SVX)** - SvxLink Core Author

---
*Disclaimer: This software is provided "AS IS", without warranty of any kind. Use at your own risk.*
