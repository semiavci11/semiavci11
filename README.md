<div align="center">

# Semi Avcı

<a href="https://github.com/semiavci11">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=58A6FF&center=true&vCenter=true&width=640&lines=Silikondan+sahaya+kadar+yaz%C4%B1l%C4%B1m;Protokol%C3%BC+bayt%C4%B1na+kadar+%C3%A7%C3%B6zerim;%C3%9Cretim+hatt%C4%B1n%C4%B1+otomatikle%C5%9Ftiririm;Masa%C3%BCst%C3%BC+%C2%B7+Web+%C2%B7+Mobil+%C2%B7+G%C3%B6m%C3%BCl%C3%BC" alt="Typing SVG" />
</a>

**Yazılım Geliştirici · Gömülü Sistem Entegrasyonu · Üretim ve Saha Yazılımları**

Bir kartın üretim hattında programlanmasından sahadaki telefonla konuşmasına,<br>
oradan buluttaki panele kadar olan yolun tamamını yazarım.

![Inodya](https://img.shields.io/badge/Inodya-Teknoloji-1f6feb?style=flat-square)
![Ankara](https://img.shields.io/badge/Konum-Ankara-30363d?style=flat-square)
![Odak](https://img.shields.io/badge/Odak-Donan%C4%B1m%20%C2%B7%20.NET%20%C2%B7%20IoT-512BD4?style=flat-square)

</div>

---

## Uçtan uca: tek kişide bütün zincir

```mermaid
flowchart LR
    A["🔌 Çıplak kart<br/>STM32 / BLE SoC"] --> B["🏭 Üretim istasyonu<br/>firmware · kimlik · test"]
    B --> C["📱 Saha<br/>BLE ile kurulum<br/>FUOTA güncelleme"]
    C --> D["📡 Ağ<br/>Sigfox · LoRaWAN<br/>BLE gateway"]
    D --> E["☁️ Sunucu<br/>API · kuyruk · panel"]
    E -.->|sürüm, iş emri| B
```

Zincirin her halkasını ayrı ayrı biliyorum; asıl işim halkalar arasındaki kuralı **tek yerde** tutup her uygulamanın aynı kaynaktan beslenmesini sağlamak.

---

## Neler yapabilirim

<table>
<tr>
<td width="50%" valign="top">

### 🔬 Protokolü baytına kadar çözerim
Dokümanı eksik bir cihazla bile konuşurum. Çerçeve, checksum, bayt sırası, komut/onay akışı; **BLE GATT**, **PC/SC APDU**, **Modbus RTU/TCP**, seri port ve ham ikili paketler. Çözdüğüm kuralı testli bir pakete çevirip herkesin kullanacağı tek giriş yaparım.

</td>
<td width="50%" valign="top">

### 🏭 Üretim hattını otomatikleştiririm
Aynı anda birden çok kartı programlayan, firmware ve radyo yığınını yükleyip sürümü doğrulayan, kimliği yazıp sonucu sunucuya bildiren istasyonlar. Hattaki tuhaf vakayı logdan kovalar, kök nedeni bulurum; donanımsız simülatörle tekrar üretirim.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📱 Sahada çalışan uygulama yazarım
.NET MAUI ve React Native ile telefondan cihaza doğrudan bağlanan, iş emri ve montaj kaydı işleyen, cihazı kablosuz güncelleyen uygulamalar. Kötü sinyale, uyuyan cihaza, yarıda kalan bağlantıya dayanıklı akışlar.

</td>
<td width="50%" valign="top">

### 🚀 Kendi kendini yöneten sistem kurarım
İmzalı paketle kendini güncelleyen, başarısız olursa önceki sürüme dönen Windows servisleri; tek tıkla kurulum paketleri, sürüm etiketleme ve changelog disiplini. Sahaya çıktıktan sonra elle müdahale istemeyen yazılım.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📡 IoT veri hattı kurarım
Sigfox, LoRaWAN ve BLE ağ geçitlerinden gelen paketleri çözen, kalıcı kuyruğa alan ve bağlantı koptuğunda veriyi kaybetmeden teslim eden .NET servisleri; MQTT ve yönetim panelleri.

</td>
<td width="50%" valign="top">

### 💳 Ödeme ve kiosk entegre ederim
WPF/WinForms kiosk akışları, POS terminaliyle mesajlaşma, akıllı kart okuyucular, kart bakiye yükleme ve işlem geçmişi; ödeme senaryolarını donanımsız deneyen test araçları.

</td>
</tr>
</table>

---

## Nasıl çalışırım

| | |
|---|---|
| ✅ **Önce doğruluk, sonra hız** | Birkaç saniyelik kazanç yerine yanlış karta yazılan tek bir kimliği önlemeyi seçerim. |
| 🧪 **Kanıtsız değişiklik yok** | Akışı değiştiren her şey ayarla açılıp kapanır ve gerçek donanımda açık, kapalı ve hatalı durumda denenir. |
| 🧩 **Kural tek yerde yaşar** | Bir protokol kuralı iki uygulamada kopya olarak durmaz; test edilmiş ortak pakete taşınır. |
| 📦 **İş muallakta kalmaz** | Değişiklik commit, test, belge ve gerekiyorsa sürümle biter. |

---

## Kanıt: Orion Üretim Platformu

> Şu an üzerinde çalıştığım, sayaç üretim hattını tek ekrandan yöneten sistem. Yukarıdaki kabiliyetlerin hepsi burada bir arada.

- **5 kanallı paralel ST-LINK** ile STM32WB kartlarına aynı anda firmware, BLE yığını ve FUS yükleme
- Her adımda kart UID'sini yeniden doğrulayan **kimlik ve Sigfox provisioning**
- Sunucudan imzalı paket çekip **kendini güncelleyen istasyon ajanı** ve otomatik geri dönüş
- Masaüstü, web ve mobil uygulamaların paylaştığı **ortak protokol paket ailesi**

![C#](https://img.shields.io/badge/C%23-.NET%2010-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-Blazor-5C2D91?style=flat-square&logo=blazor&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![STM32](https://img.shields.io/badge/STM32WB-ST--LINK-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![BLE](https://img.shields.io/badge/BLE-GATT-0082FC?style=flat-square&logo=bluetooth&logoColor=white)

---

## Araç kutusu

<p>
<img src="https://skillicons.dev/icons?i=cs,cpp,dotnet,ts,react,postgres,mongodb,docker,linux,windows,git,vscode&perline=12" alt="skills" />
</p>

![.NET MAUI](https://img.shields.io/badge/.NET%20MAUI-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![WPF](https://img.shields.io/badge/WPF%20%2F%20WinForms-0078D4?style=flat-square&logo=windows&logoColor=white)
![Blazor](https://img.shields.io/badge/Blazor-5C2D91?style=flat-square&logo=blazor&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white)
![Bluetooth LE](https://img.shields.io/badge/Bluetooth%20LE-0082FC?style=flat-square&logo=bluetooth&logoColor=white)
![Sigfox](https://img.shields.io/badge/Sigfox-7B2CBF?style=flat-square)
![LoRaWAN](https://img.shields.io/badge/LoRaWAN-1A73E8?style=flat-square)
![Modbus](https://img.shields.io/badge/Modbus%20RTU%2FTCP-555555?style=flat-square)
![PC/SC](https://img.shields.io/badge/PC%2FSC%20Smart%20Card-555555?style=flat-square)
![Inno Setup](https://img.shields.io/badge/Inno%20Setup-264de4?style=flat-square)

---

## Açık depolar

| Proje | Açıklama |
|---|---|
| [**hp-victus-cachyos-field-guide**](https://github.com/semiavci11/hp-victus-cachyos-field-guide) | Bir laptop arızasını donanım seviyesine kadar kovaladığım vaka notları: Hall/LID sensörü, flex kablo ve Linux'ta fan kontrolü. Türkçe ve İngilizce. |
| [**Yakıt Hesabı**](https://semiavci11.github.io/yakithesabi-gizlilik/) | React Native ve TypeScript ile yazdığım, verilerini cihazda tutan yakıt ve enerji maliyeti hesaplayıcısı (Android). |

---

<div align="center">

<sub>Çoğu çalışmam şirket içi depolarda. Donanımla konuşması gereken bir yazılımınız varsa yazın.</sub>

</div>
