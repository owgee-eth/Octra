# Octra

<img width="1715" height="437" alt="Octra-Info" src="https://github.com/user-attachments/assets/d5e19da1-d016-4423-b204-f422cd06929b" />

# Testnet Rehberi II

Gelin Octra Labs'in henüz yayınladığı ve karmaşık matematik problemlerini dahi birkaç komut yardımıyla çözebilen yeni test kontratına birlikte göz atalım ve yapabileceklerimizi keşfedelim.

Octra Client’a gelen bu güncelleme, deneyimli kullanıcılar için uygundur. Eğer henüz bir Octra cüzdanı oluşturmadıysanız ya da Octra testnet işlemleri konusunda yeterli deneyime sahip değilseniz, lütfen önce testnet ana görevlerini tamamlamanızı sağlayacak rehberimize göz atınız.

https://github.com/owgee-eth/Octra/blob/main/README.md

# Codespace Temizliği

GitHub, aynı anda en fazla iki aktif codespace oluşturmanıza izin verir. Bu nedenle, yeni testnet işlemlerine başlamadan önce mevcut Codespacelerinizde temizlik yapmanız gerekebilir.

Wallet Generator’ı kurduğunuz Codespace’i silebilirsiniz, yeni alan açmak için güvenli bir tercihtir. Ancak Octra Pre Client kurulumunu yaptığınız Codespace’i silmeyin, ileride görevleri yerine getirirken bu alanı tekrar kullanmanız gerekecek.

### Video Rehber
[![Video Rehber](https://img.youtube.com/vi/DuvELCEbDqs/0.jpg)](https://www.youtube.com/watch?v=DuvELCEbDqs)

# 1. GitHub Üzerinde Bir Fork Yaratıyor ve Codespace Oluşturuyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/A3PhqwQQGnA/0.jpg)](https://www.youtube.com/watch?v=A3PhqwQQGnA)

### 1.1. Fork Yaratma

Octra Labs'in ilgili Github sayfasına girerek proje üzerinde bir fork yaratıyoruz:

https://github.com/octra-labs/ocs01-test

### 1.2. Codespace Oluşturrma

Yarattığımız bu fork üzerinde yeni bir Codespace oluşturuyoruz.

# 2. "OCS01" Test Client Kurulumu

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/GTPAixehwkg/0.jpg)](https://www.youtube.com/watch?v=GTPAixehwkg)

### 2.1. Komutları Terminale Giriyoruz

### 2.1.1. Server Update
```bash
sudo apt update -y && sudo apt upgrade -y
```

### 2.1.2. Download Packages
```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

### 2.1.3. Install Rust
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Kurulum ekranında bilgi ekranı belirdiğinde klavyemiz yardımı ile "1" yazarak Enter tuşuna basıyoruz ve kuruluma devam ediyoruz.

Komut satırı tekrar belirdiğinde şu komutları giriyoruz:
```bash
source $HOME/.cargo/env
```

### 2.1.4. Build
```bash
git clone https://github.com/octra-labs/ocs01-test.git
cd ocs01-test
cargo build --release
```

### 2.1.5. Interface
```bash
cp EI/exec_interface.json .
```

### 2.1.6. Cüzdan Entegrasyonu
```bash
nano wallet.json
```

Komutu girerek cüzdan entegrason ekranına ulaşıyoruz.

İlgili satırlara, B64 formatında private key'imizi ve Octra cüzdan adresimizi giriyoruz.

### 2.1.7. Değişiklikleri Kaydetme

Yaptığınız değişiklikleri kaydetmek için öncelikle CTRL + O (harf) tuşuna ve ardından Enter tuşuna basın.

Son olarak ana terminal ekranına dönmek için CTRL + X tuşlarına basınız.

# 3. "OCS01" Test Client Görevleri

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/kdXl9GONe9M/0.jpg)](https://www.youtube.com/watch?v=kdXl9GONe9M)

### 3.1. Terminale Erişim

Terminalimizin komut satırına şu komutu girerek kurulumunu gerçekleştirdiğimiz Octra Test Client menüsüne erişim sağlıyoruz.

```bash
./target/release/ocs01-test
```

### 3.2. Görevleri Yerine Getirme

Yayınladığımız Video Rehber yardımı ile Octra Labs'in henüz yayınladığı ve karmaşık matematik problemlerini dahi birkaç komut yardımıyla çözebilen yeni test kontratında yapabileceklerinizi keşfedin.

```bash
1. greeting (get personal msg): mesaj alma fonksiyonu. sizi bir hoş geldin mesajı ile karşılar.
2. contract info (get contract description): sözleşme hakkında bilgi verir.
3. claim 1 token (only once per address): octra cüzdan adresinize bir defaya mahsus olmak üzere bir adet octra token talep etme fonksiyonu. her adrese sadece bir defa token gönderir.
4. check token balance: bir adresin sahip olduğu octra token miktarını gösterir.
5. dot product: iki vektörün noktasal çarpımını hesaplama fonksiyonu. matematiksel olarak iki vektörün iç çarpımıdır.
6. vector magnitude: bir vektörün uzunluğunu hesaplama fonksiyonu. vektörün normunu bulur.
7. power: bir sayının üssünü hesaplama.
8. factorial: faktöriyel hesaplama fonksiyonu.
9. fibonacci number: fibonacci serisinden bir sayı bulma.
10. greatest common divisor: iki sayının en büyük ortak bölenini bulma. matematikte “GCD” veya “EBOB” olarak bilinir.
11. check (if) number is prime: bir sayının asal olup olmadığını kontrol etme fonksiyonu.
12. 2x2 matrix determinant: 2x2 matrisin determinantını hesaplama fonksiyonu.
13. linear interpolation: İki nokta arasında bir değeri tahmin etme.
14. modular exponentiation: modüler üs hesaplama işlemi.
0. exit: programdan çıkma.
```

Şimdilik yapacaklarımız bu kadar. Video rehberimiz boyunca 1. ile 4. görevler arasındaki işlemleri birlikte gerçekleştirdik. 

Fakat mevcut Octra testnet kontratındaki diğer görevleri de kendiniz keşfetmeyi unutmayın.

### Teşekkür

Bu rehber yalnızca bir içerik değil, Modularity topluluğunun vizyonu ve emeğinin bir yansıması.
Bu sürecin her adımında değer üreten, paylaşan ve birlikte öğrenen tüm Modularity ailesine içten teşekkür ederim. 💚

https://x.com/modularityx

Ayrıca bu rehberi hazırlarken ilham aldığım @FurkanL0eth’e de bir teşekkürü borç bilirim.

### Yazarın Notu

Bu tarz rehberlerin devamı gelsin diyorsanız, X profilimi takip etmeyi, gönderileri beğenip yorumlamayı ve paylaşmayı unutmayın.

Paylaşılan her bilgi, yeni bir başlangıcın kapısını açar. Birlikte kazanacağız. 💚

https://x.com/owgee_eth
