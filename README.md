# Kiosk, cihaz ve saha yazılımları

Bir kioskun ödeme ekranından üretim istasyonunda kart programlamaya, sahadaki bir sayacın verisini sunucuya taşımaya kadar farklı yazılımlar geliştirdim. İşin bir ucunda kullanıcının dokunduğu ekran, diğer ucunda cihazın gönderdiği baytlar var.

### Kiosklar ve kart okuyucuları

Windows kioskları ve tabletler için WPF ve Windows Forms ile ödeme, QR, işlem geçmişi ve yardım ekranları geliştirdim. Kart okuyucularıyla haberleşme tarafında C++ ve Windows’un akıllı kart arayüzüyle de çalıştım.

### Üretim istasyonları ve cihaz testleri

USB üzerinden kart programlayan, firmware yükleyip sürümü doğrulayan üretim araçları geliştirdim. BLE/GATT üzerinden cihaz keşfi, komut gönderme ve yanıt doğrulama akışları için masaüstü test araçları ve komut satırı uygulamaları yazdım.

### Mobil uygulamalar ve saha operasyonları

.NET MAUI ile Android ve iOS’ta sayaçla doğrudan haberleşen uygulamalar geliştirdim. Sahadaki iş emirleri, montaj kayıtları ve cihaz güncellemeleri bu işin parçası. React Native ve TypeScript ile kayıtlarını cihazda tutan kişisel bir maliyet hesaplama uygulaması da geliştirdim.

### IoT altyapısı ve arka uç

Sigfox, LoRaWAN ve BLE ağ geçitlerinden gelen ikili paketleri çözümleyen .NET servisleri üzerinde çalıştım. Telemetriyi kalıcı kuyruğa alıp hedef sistemlere ileten ve bağlantı hatasından sonra teslimata devam eden akışlar geliştirdim.

### Kütüphaneler ve doğrulama

Tekrar kullanılan .NET bileşenleri, Modbus RTU/TCP ve MQTT paket işleme katmanları, BLE simülasyonları ve gerçek cihazla çalışan test araçları geliştiriyorum. Özellikle cihazın bağlantısı koptuğunda, bir yazma yarıda kaldığında veya aynı işlem tekrar geldiğinde sistemin davranışını test ediyorum.
