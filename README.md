# Custom ROM Yükleme Rehberi

Bu rehber, cihazınıza custom recovery ve custom ROM yüklemek için adım adım yapılması gereken işlemleri anlatır.

---

## Notlar

- Yedeklerinizi almadan bu işlemleri yapmayın.  
- Yanlış ROM veya recovery yüklenmesi cihazınızda ciddi sorunlara yol açabilir.  
- Bu işlem garanti kapsamı dışına çıkartabilir.

---

## Gereksinimler

- **Odin** veya uygun flash aracı (Windows için)  
- Cihaza uygun **Custom Recovery (.tar dosyası)**  
- İndirilen ve kurulacak **Custom ROM (.zip dosyası)**  
- Cihazınız ile bilgisayar arasında iletişim kurmak için gerekli **USB sürücüleri**  
- USB kablosu 

---

## Adımlar

### 1. Hazırlık

- Cihazınızı kapatın.  
- Bilgisayarınıza USB sürücülerini yükleyin.  
- Odin programını indirin ve çalıştırın.

### 2. Cihazı Download Mode’a alma

- Cihaz kapalıyken gerekli tuş kombinasyonunu kullanarak Download Mode’a geçin.  
- Cihazı bilgisayara bağlayın. Odin programında bağlantı doğrulama kutusunun renk değiştiğini göreceksiniz.

### 3. Custom Recovery Yükleme

- Odin’de **AP** butonuna tıklayın ve custom recovery `.tar` dosyasını(twrp dosyası) seçin.  
- **Options** kısmında **Auto Reboot** seçeneğinin işaretini kaldırın.  
- **Start** butonuna basarak yüklemeyi başlatın.  
- İşlem tamamlandığında Odin "PASS" mesajı verecektir.

### 4. Recovery Moduna Geçiş

- Cihaz otomatik açılmaz, cihazı kapatın.  
- Gerekli tuş kombinasyonu ile recovery moduna geçin(Kısaca TWRP' ye girin).

### 5. Recovery’de Temizlik

- **Wipe** bölümünden **Dalvik / ART Cache**, **Cache**, **System** ve **Data** alanlarını temizleyin.  
- Ana menüye geri dönün.

### 6. Custom ROM Yükleme

- Cihazı USB ile bilgisayara bağlayın.(Zaten bağlıysa da problem yok)  
- Recovery’de **Mount > Enable MTP** seçeneğini açın.(Telefonunuzu pc' den görüp içine os atmmamız için)  
- Bilgisayarınızdan custom ROM `.zip` dosyasını cihazın iç depolamasına kopyalayın(Kısaca LineageOS, RevengeOS... dosyanızı pcden telefona kopyala yapıştır yapmak için).  
- Recovery’den **Install** seçeneğine giderek `.zip` dosyasını seçin ve kurulumu başlatın.  
- Kurulum tamamlandıktan sonra **Wipe Cache/Dalvik** işlemini yapın.

### 7. Cihazı Yeniden Başlatma

- Ana menüden **Reboot System** seçeneği ile cihazı yeniden başlatın.  
- İlk açılış biraz uzun sürebilir, sabırlı olun.

---

# Custom ROM Installation Guide

This guide explains step-by-step how to install a custom recovery and custom ROM on your device.

---

## Notes

- Always back up your data before proceeding.  
- Installing the wrong ROM or recovery can cause serious issues.  
- This process may void your warranty.

---

## Requirements

- **Odin** or a suitable flashing tool (for Windows)  
- A compatible **Custom Recovery (.tar file)**  
- The **Custom ROM (.zip file)** to be installed  
- Necessary **USB drivers** to connect your device to the PC  
- USB cable  

---

## Steps

### 1. Preparation

- Power off your device.  
- Install USB drivers on your computer.  
- Download and launch the Odin program.

### 2. Enter Download Mode

- With the device powered off, use the correct button combination to enter Download Mode.  
- Connect your device to the PC. You should see a color change in Odin’s connection box indicating successful connection.

### 3. Flash Custom Recovery

- In Odin, click the **AP** button and select the custom recovery `.tar` file (e.g. TWRP).  
- In the **Options** section, uncheck **Auto Reboot**.  
- Click **Start** to begin flashing.  
- Once completed, Odin will display a “PASS” message.

### 4. Enter Recovery Mode

- The device will not reboot automatically. Power it off manually.  
- Use the button combination to enter recovery mode (i.e. enter TWRP).

### 5. Wipe Data in Recovery

- In the **Wipe** menu, select **Dalvik / ART Cache**, **Cache**, **System**, and **Data** partitions to wipe.  
- Return to the main menu.

### 6. Install Custom ROM

- Connect your device to the PC via USB (if not already connected).  
- In Recovery, go to **Mount > Enable MTP** (to allow PC access to device storage).  
- Copy the custom ROM `.zip` file (e.g. LineageOS, RevengeOS) from your PC to your device’s internal storage.  
- In Recovery, select **Install**, locate the `.zip` file, and swipe to flash it.  
- After installation, perform **Wipe Cache/Dalvik**.

### 7. Reboot Device

- From the main menu, select **Reboot System**.  
- The first boot may take some time, please be patient.

---

