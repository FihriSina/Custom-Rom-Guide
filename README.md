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

