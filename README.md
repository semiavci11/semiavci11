<div align="center">

# Semi Avcı

**Yazılım Geliştirici · Gömülü Sistem Entegrasyonu · Üretim ve Saha Yazılımları**

Donanımla konuşan yazılımlar yazıyorum: üretim hattında kartı programlayan istasyonlar,<br>
sahadaki sayaçla BLE üzerinden konuşan mobil uygulamalar ve ödeme alan kiosklar.

![Inodya](https://img.shields.io/badge/Inodya-Teknoloji-1f6feb?style=flat-square)
![Ankara](https://img.shields.io/badge/Konum-Ankara-30363d?style=flat-square)
![Odak](https://img.shields.io/badge/Odak-.NET%20%C2%B7%20IoT%20%C2%B7%20Donan%C4%B1m-512BD4?style=flat-square)

</div>

---

## Şu an üzerinde çalıştığım: Orion Üretim Platformu

> Sayaç üretim hattını tek ekrandan yöneten web tabanlı üretim sistemi. Her istasyondaki ajan kartları programlar, kimliklerini yazar ve sonucu sunucuya bildirir.

- **Paralel programlama:** Bir istasyonda 5 ST-LINK kanalıyla STM32WB kartlarına aynı anda firmware, BLE yığını ve FUS yükleme; her kartın sürümü okunarak doğrulanır.
- **Cihaz kimliği ve provisioning:** EEPROM yazımı, cihaz numarası ve Sigfox kimlik bilgisi atama; kart UID'si her adımda yeniden kontrol edilerek yanlış karta kimlik yazılması engellenir.
- **Kendini güncelleyen istasyon ajanı:** Sunucudan imzalı paket çeker, Windows servisi olarak takas eder, başarısız olursa önceki sürüme döner.
- **Ortak protokol çekirdeği:** Bayt sırası, çerçeve, checksum ve BLE komut kuralları tek bir test edilmiş NuGet paket ailesinde; masaüstü, web ve mobil uygulamalar aynı kaynağı kullanır.
- **Uçtan uca teslim:** ASP.NET Core sunucu, PostgreSQL, Inno Setup kurulumları ve sürüm notlarıyla yayımlanan sürümler.

![C#](https://img.shields.io/badge/C%23-.NET%2010-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-Blazor-5C2D91?style=flat-square&logo=blazor&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![STM32](https://img.shields.io/badge/STM32WB-ST--LINK-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![BLE](https://img.shields.io/badge/BLE-GATT-0082FC?style=flat-square&logo=bluetooth&logoColor=white)

---

## Neler yapıyorum

<table>
<tr>
<td width="50%" valign="top">

### 🏭 Üretim istasyonları
USB/ST-LINK üzerinden kart programlayan, firmware yükleyip sürümü doğrulayan Windows araçları ve komut satırı uygulamaları. Donanımsız paralel simülasyon ve canlı donanım testleri.

</td>
<td width="50%" valign="top">

### 📱 Mobil saha araçları
.NET MAUI ile Android ve iOS'ta sayaçla BLE üzerinden doğrudan konuşan, iş emri ve montaj kaydı işleyen, cihaza kablosuz güncelleme (FUOTA) yapan uygulamalar.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💳 Kiosk, ödeme ve kart okuyucular
WPF ve WinForms kiosk uygulamaları, POS terminal entegrasyonu, PC/SC ve USB üzerinden akıllı kart haberleşmesi; C# ve C++ cihaz kütüphaneleri.

</td>
<td width="50%" valign="top">

### 📡 IoT ve arka uç
Sigfox, LoRaWAN ve BLE ağ geçitlerinden gelen ikili paketleri çözen .NET servisleri; kalıcı kuyruk, Modbus RTU/TCP ve MQTT katmanları, yönetim panelleri.

</td>
</tr>
</table>

---

## Teknolojiler

**Diller ve platformlar**<br>
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![.NET MAUI](https://img.shields.io/badge/.NET%20MAUI-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![React Native](https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![WPF](https://img.shields.io/badge/WPF%20%2F%20WinForms-0078D4?style=flat-square&logo=windows&logoColor=white)

**Arka uç ve veri**<br>
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Blazor](https://img.shields.io/badge/Blazor-5C2D91?style=flat-square&logo=blazor&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)

**Donanım ve protokoller**<br>
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Bluetooth LE](https://img.shields.io/badge/Bluetooth%20LE-0082FC?style=flat-square&logo=bluetooth&logoColor=white)
![Sigfox](https://img.shields.io/badge/Sigfox-7B2CBF?style=flat-square)
![LoRaWAN](https://img.shields.io/badge/LoRaWAN-1A73E8?style=flat-square)
![Modbus](https://img.shields.io/badge/Modbus%20RTU%2FTCP-555555?style=flat-square)
![PC/SC](https://img.shields.io/badge/PC%2FSC%20Smart%20Card-555555?style=flat-square)

---

## Açık depolar

| Proje | Açıklama |
|---|---|
| [**hp-victus-cachyos-field-guide**](https://github.com/semiavci11/hp-victus-cachyos-field-guide) | HP Victus 16 + CachyOS: ekran kararması (Hall/LID) arızasının ve Linux'ta fan kontrolünün gerçek vaka notları. Türkçe ve İngilizce. |
| [**Yakıt Hesabı**](https://semiavci11.github.io/yakithesabi-gizlilik/) | React Native ve TypeScript ile yazdığım, verilerini cihazda tutan yakıt ve enerji maliyeti hesaplayıcısı (Android). |

---

<div align="center">

<sub>Çoğu çalışmam şirket içi depolarda. Donanım entegrasyonu, üretim yazılımı veya .NET üzerine konuşmak isterseniz yazın.</sub>

</div>
