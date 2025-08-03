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

# 3. Octra Client Kurulumu ve Octra Testnet Görevlerini Yerine Getirin

Bu bölümde, bir Octra Client'ın nasıl kurulacağını ve terminal aracılığı ile Octra testnet görevlerinin nasıl yerine getirilebileceğini birlikte keşfedeceğiz.

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





