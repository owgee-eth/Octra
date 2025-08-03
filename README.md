# Octra

<img width="926" height="221" alt="Screenshot 2025-08-01 144619" src="https://github.com/user-attachments/assets/2b0aff75-2ccd-43da-bbbd-4a8d9c1a66d0" />

# Testnet Rehberi

Zincirler arası finans artık daha akıllı, daha şeffaf ve daha merkeziyetsiz olacak ve bu dönüşüm Octra ile birlikte başlıyor.

Octra, 2021’de İsviçre merkezli olarak kurulan ve bugün Fully Homomorphic Encryption teknolojisini kullanarak gizliliği en üst seviyeye taşıyan yeni nesil bir blockchain ağı.

Octra, DeFi dünyasında zincirler arası takasları daha hızlı, güvenli ve kullanıcı dostu hale getirmeyi amaçlıyor. 

Bu erken aşamada yer alarak ekosisteme ilk katılanlardan biri olabilirsin! Katılım için sadece bir GitHub hesabı yeterli.

Şu anda neler yapabilirsin?

- Cüzdan oluştur
- Test token talep et
- Octra Client görevlerini yerine getir
- Güncellemeler için takipte kal

# 1. Octra Hesabı Oluşturma

Bu bölümde bir Octra hesap cüzdanı nasıl oluşturulur birlikte keşfedeceğiz.

İşlem sonucunda yepyeni bir Octra cüzdanına sahip olacak ve testnet işlemlerini gerçekleştirmeye başlayabileceksiniz!

## 1.1. GitHub Üzerinde Bir Fork Yaratıyor ve Codespace Oluşturuyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/TR-dF0_h2_M/0.jpg)](https://www.youtube.com/watch?v=TR-dF0_h2_M)

### 1.1.1. Fork Yaratma

Octra Labs'in ilgili Github sayfasına girerek proje üzerinde bir fork yaratıyoruz:

https://github.com/octra-labs/wallet-gen

### 1.1.2. Codespace Oluşturrma

Yarattığımız bu fork üzerinde yeni bir Codespace oluşturuyoruz.

## 1.2. Terminal Kullanarak Octra Hesabımızı Yaratıyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/7tbCkYM6_Qw/0.jpg)](https://www.youtube.com/watch?v=7tbCkYM6_Qw)

### 1.2.1. Komutları Terminale Giriyoruz.

```bash
curl -fsSL https://bun.sh/install | bash

source ~/.bashrc

bun --version

bun install

bun run build

bun start
```

### 1.2.2. Octra Cüzdanımızı Yaratıyoruz

Octra cüzdan bilgilerinizi kaydetmeyi ve güvenli bir yerde saklamayı lütfen unutmayınız.

# 2. Octra Testnet Token Talep Etme

Bu bölümde, yarattığımız Octra hesap cüzdanımız için Octra testnet tokenları talep edeceğiz.

Talep ettiğimiz tokenlarını Octra Client üzerinde gerçekleştireceğimiz görevler için kullanacağız.

### 2.1. Octra Faucet

https://faucet.octra.network/ adresine giderek Octra testnet tokenlarınızı talep edin.

Bir validator olmadığınız üzere, lütfen "this is a validator address" seçeneğini işaretlemeyin.

### 2.2. Discord Faucet

Eğer resmi faucet haznesinde yeterli Octra testnet tokeni bulunmuyorsa, alternatif olarak Octranın Discord sunucusuna giderek "for-token-sharing" kanalına Octra cüzdan adresinizi yayınlayarak diğer kullanıcılardan test token talep edebilirsiniz.

Octra Discord: https://discord.gg/octra/

# 3. Octra Client Kurulumu

Bu bölümde, bir Octra Client'ın nasıl kurulacağını birlikte öğreneceğiz. 

Bölüm sonunda, Octra testnet görevlerini yerine getirmek için kullanacağımız Octra Client arayüzüne giriş yapacağız.

## 3.1. GitHub Üzerinde Bir Fork Yaratıyor ve Codespace Oluşturuyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/Qien2ndffJw/0.jpg)](https://www.youtube.com/watch?v=Qien2ndffJw)

### 3.1.1. Fork Yaratma

Octra Labs'in ilgili Github sayfasına girerek proje üzerinde bir fork yaratıyoruz:

https://github.com/octra-labs/octra_pre_client

### 3.1.2 Codespace Oluşturrma

Yarattığımız bu fork üzerinde yeni bir Codespace oluşturuyoruz.

## 3.2. Octra Client Kurulumunu Başlatıyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/zJ5cwge4c_A/0.jpg)](https://www.youtube.com/watch?v=zJ5cwge4c_A)

### 3.2.1 Komutları Terminale Giriyoruz

 - 3.2.1.1 Install Python:

```bash
sudo apt install python3 python3-pip python3-venv python3-dev -y
```

 - 3.2.1.2.Install CLI

```bash
git clone https://github.com/octra-labs/octra_pre_client.git
cd octra_pre_client

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

cp wallet.json.example wallet.json
```

## 3.3. Octra Cüzdanımızı Client'a Entegre Ediyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/3RUF5quDHzI/0.jpg)](https://www.youtube.com/watch?v=3RUF5quDHzI)

### 3.3.1 Entegrasyon İşlemi

```bash
nano wallet.json
```

Komutu girerek cüzdan entegrason ekranına ulaşıyoruz.

İlgili satırlara, B64 formatında private key'imizi ve Octra cüzdan adresimizi giriyoruz.

### 3.3.2 Değişiklikleri Kaydetme

Yaptığınız değişiklikleri kaydetmek için öncelikle CTRL + O (harf) tuşuna ve ardından Enter tuşuna basın.

Son olarak ana terminal ekranına dönmek için CTRL + X tuşlarına basınız.

## 3.4. Octra Client Ayrayüzüne Erişim Sağlıyoruz

### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/p_dCZnG43YA/0.jpg)](https://www.youtube.com/watch?v=p_dCZnG43YA)

### 3.4.1. Client'ı Çalıştırma

```bash
python3 -m venv venv
source venv/bin/activate
python3 cli.py
```

Komutunu girerek Octra Client ayaryüzüne ulaşıyoruz.

### 3.4.2 Tekrar Erişim

Octra Client oturumunuzu sonlandırdıktan sonra, ileride görevleri yapmaya devam etmek için Client'a tekrar erişmek isterseniz, yarattığımız GitHub Codespace'i yeniden başlatıyor ve şu konutları terminalimize girerek dilediğimiz zaman Octra Client arayüzüne erişebiliyoruz.

```bash
cd octra_pre_client
python3 -m venv venv
source venv/bin/activate
python3 cli.py
```

# 4. Octra Testnet Görevlerini Yerine Getirme

Bu bölümde terminal aracılığı ile Octra testnet görevlerinin nasıl yerine getirilebileceğimizi ayrıntılı bir şekilde ve her görev için özenle düzenlenmiş videolu rehber yardımı ile birlikte keşfedeceğiz.

## 4.1. Send Transaction
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/y4LkBqNx9-U/0.jpg)](https://www.youtube.com/watch?v=y4LkBqNx9-U)

## 4.2. Refresh
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/4jkYx_4yoz4/0.jpg)](https://www.youtube.com/watch?v=4jkYx_4yoz4)

## 4.3. Multi Send
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/2PHArrND6WQ/0.jpg)](https://www.youtube.com/watch?v=2PHArrND6WQ)

## 4.4. Encrypt Balance
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/6IQ7ruv0KvI/0.jpg)](https://www.youtube.com/watch?v=6IQ7ruv0KvI)

## 4.5. Decrypt Balance
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/SuS1jw8GRRA/0.jpg)](https://www.youtube.com/watch?v=SuS1jw8GRRA)

## 4.6. Private Transfer
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/yRLnCHdVsuw/0.jpg)](https://www.youtube.com/watch?v=yRLnCHdVsuw)

## 4.7. Claim Transfers
### Video Rehber

[![Video Rehber](https://img.youtube.com/vi/LFaBGO-z_x0/0.jpg)](https://www.youtube.com/watch?v=LFaBGO-z_x0)

## 4.8. Export Keys

Bu bölümde cüzdan bilgilerinizi görüntüleyebilir ve dilerseniz cüzdan anahtarlarınızı dışarı aktarabilirsiniz.

## 4.9. Clear History

İşlem geçmişinizi temizleyebilirsiniz.

## 4.10. Exit

Sistemden çıkış.


