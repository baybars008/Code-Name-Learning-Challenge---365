<h2> [Day-24] January 24, 2024 : Malware Analysis Temelleri - Adım 05 | [TR] </h2> 

<h3> Dinamik Kötü Amaçlı Yazılım Analizi |  Virtual Machine Creation </h3> 

#### 1. Sanallaştırma Yazılımını Yükleme
```
"Sanal bir işletim sistemi kurmadan önce, bunu sağlayacak bir sanallaştırma yazılımını yüklememiz gerekiyor."
Aralarında bazı farklılıklar olsa da, sanallaştırma yazılımlarının herhangi biri dinamik analizimiz için bize yardımcı olacaktır. 
Aşağıdaki sanallaştırma yazılımlarından birini yükleyebilirsiniz:

• VMware Workstation
• VMware Fusion (macOS için)
• Oracle Virtualbox
```

#### 2. İşletim Sistemini Yükleme
```
Kötü yazılım analizi için Sanal Makinemizde bazı yapılandırma değişiklikleri yapmamız gerekiyor.

Windows 10 iso indirmek için: https://www.microsoft.com/en-us/evalcenter/download-windows-10-enterprise
```

#### 3. Anti-malware Çözümlerini Kapatın
```
Başlat menüsünde “grup ilkesini düzenle” aratarak Yerel Grup İlkesi Düzenleyici uygulamasını açabilirsiniz. 
Alternatif olarak, “gpedit.msc” aratarak veya Windows'ta “Ara>Çalıştır” işlevi üzerinden Yerel Grup İlkesi Düzenleyici uygulamasına erişebilirsiniz.
Windows Defender'ı Yerel Grup İlkesi Düzenleyici uygulaması kullanarak devre dışı bırakmak için aşağıdaki politiğe erişmeniz gerekir.
“Bilgisayar Yapılandırması > Yönetim Şablonları > Windows Bileşenleri > Microsoft Defender Antivirus”
Burada, "Microsoft Defender Antivirus'u Kapat" politikasına çift tıklayın ve "Etkin" olarak ayarlayın.
Ayrıca, "Gerçek Zamanlı Koruma" altındaki "Bilgisayarınızdaki dosya ve program aktivitelerini izle" politikasını da devre dışı bırakmalısınız.
```

#### 4. Sanal işletim Sisteminizin Adını Değiştirin
```
Bazı kötü amaçlı yazılımlar, analiz ortamlarında çalışmamak için çeşitli kontroller yapar. 
Bu kontrollerden biri, ana bilgisayar adını kontrol etmektir. 
Çoğu sandbox'un "Sandbox", "Malware", "Cuckoo" gibi ana bilgisayar adları olduğu için, kötü amaçlı yazılımlar bu adlara sahip sistemlerde çalışmamak üzere programlanmıştır.
VM'nizin normal bir kullanıcının sistemi gibi görünmesini sağlamak, anti-analiz tekniklerinden kaçınmanıza yardımcı olacaktır. 
Ana bilgisayar adı olarak rastgele bir isim belirlemek, bu tür kontrollerden kaçınmanıza yardımcı olacaktır.
Cihaz adını değiştirmek için “Ayarlar → Sistem → Hakkında” seçeneğini seçip ardından “Bu PC'yi Yeniden Adlandır” butonuna tıklamalısınız.
Kullanıcı adınızı değiştirmeyi de unutmayın!
```

#### 5. Otomatik Güncellemeleri Kapatın
```
Analiz edeceğimiz kötü amaçlı yazılım, işletim sistemindeki güvenlik açıklarından faydalanıyor olabilir. 
Kötü amaçlı yazılımın olabildiğince normal çalışabilmesi için, sanal işletim sistemimizin otomatik güncellemelerini kapatmamız gerekiyor.
Otomatik güncellemeleri grup ilkesi ayarları üzerinden kapatabilirsiniz.
Yerel Grup İlkesi Düzenleyici uygulamasını, başlat menüsünde “grup ilkesini düzenle” aratarak açabilirsiniz. 
Alternatif olarak, “gpedit.msc” aratarak veya Windows'ta “Ara>Çalıştır” işlevi üzerinden Yerel Grup İlkesi Düzenleyici uygulamasına erişebilirsiniz.
Daha sonra aşağıdaki politiğe erişmelisiniz.
“Bilgisayar Yapılandırması > Yönetim Şablonları > Windows Bileşenleri > Windows Update”
İlgili politiğe eriştikten sonra, "Otomatik Güncellemeleri Yapılandır" adlı politikayı "Devre Dışı" olarak ayarlamalısınız.
```

#### 6. Gizli Uzantıları Devre Dışı Bırakın
```
Saldırganların kurbanlarını kandırmak için dosya uzantılarını değiştirdiğini görmüş olabilirsiniz. Bunu nasıl yaparlar?
Windows işletim sistemleri varsayılan olarak bilinen dosya uzantılarını gizlemek üzere ayarlanmıştır. 
Yani, "Chrome.exe" adlı bir dosya varsayılan olarak "Chrome" olarak görünür. 
Saldırganlar kötü amaçlı yazılımlarını "Foto.jpg.exe" olarak adlandırarak, kullanıcının dosyayı "Foto.jpg" olarak görmesine neden olurlar. 
Kullanıcı bu dosyanın bir resim dosyası olduğunu düşünüp açtığında, kötü amaçlı yazılım çalışmaya başlar.
Analiz sırasında bu konuda kafa karışıklığına düşmemek için, varsayılan olarak gizlenen uzantıların her zaman gösterilmesini sağlamamız gerekiyor.
Bunun için “Dosya Gezgini” adlı uygulamayı açmalı ve üst menüdeki “Dosya”yı ve ardından “Klasör ve arama seçeneklerini değiştir” butonlarını tıklayarak ayarlar menüsüne erişmemiz gerekiyor.
Daha sonra “Görünüm” sekmesinden “Bilinen dosya türleri için uzantıları gizle” seçeneğinin işaretini kaldırarak ayarları kaydetmelisiniz.
```

#### 7. Gizli Dosya ve Klasörleri Göster
```
Kötü amaçlı yazılımlar, dosyalarını gizleyerek kullanıcının bunları tespit etmesini engellemeyi amaçlar. 
Varsayılan olarak gizli dosya ve dizinleri göstermek, daha rahat bir analiz yapmamızı sağlayacaktır.
“Dosya Gezgini” adlı uygulamayı açalım ve üst menüdeki “Dosya” ile “Klasör ve arama seçeneklerini değiştir”i tıklayarak ayarlar menüsünü açalım.
Daha sonra, “Görünüm” sekmesinden “Gizli dosya, klasör ve sürücüleri göster”i işaretleyelim ve ayarı kaydedelim.
```

#### 8. ASLR'yi Devre Dışı Bırakın  (Address Space Layout Randomization)
```
Windows'un yeni sürümlerinde ASLR (Adres Uzayı Düzeni Rastgeleleştirme) adında bir anti-exploit güvenlik mekanizması bulunmaktadır.
Bu ayarı Kayıt Defteri yardımıyla devre dışı bırakabilirsiniz. 
Kayıt Defteri Düzenleyici uygulamasını açarak aşağıdaki kayıt defterine erişin.
“HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management”
"MoveImages" adında bir “REG_DWORD” türünde anahtar oluşturun.
Bu ayarlar sonunda ASLR özelliğini devre dışı bırakacaktır.
```

#### 9. Windows Güvenlik Duvarını Devre Dışı Bırakın
```
Önceki adımlarda uyguladığımız gibi, analiz ettiğimiz kötü amaçlı yazılımın güvenlik mekanizmalarıyla karışmasını önlemek için Windows Güvenlik Duvarını devre dışı bırakmalıyız.
Denetim Masası üzerinden Windows Defender Güvenlik Duvarı ayarlarına erişin. 
Dosya Gezgini'nin üst menüsündeki arama çubuğunu kullanarak bu ayarlara erişebilirsiniz. 
Bu arama çubuğuna aşağıdaki yolu kopyalayıp aratırsanız, sizi Windows Defender Güvenlik Duvarı ayarlarına götürecektir.
"Denetim Masası\Sistem ve Güvenlik\Windows Defender Güvenlik Duvarı\Özelleştir"
Defender Güvenlik Duvarı ayarlarına erişildikten sonra, "Windows Defender Güvenlik Duvarını kapat" seçeneğini seçin ve kaydedin. 
Bu, Güvenlik Duvarını devre dışı bırakacaktır.
```

#### 10. Son Kullanıcı Sistemi Taklidi Yapın
```
Analiz ettiğiniz kötü amaçlı yazılımın anti-analiz teknikleri tarafından yakalanmaması için, VM'nizin mümkün olduğunca normal bir son kullanıcı işletim sistemi gibi görünmesini sağlamalısınız.
Bunun için kesin talimatlar veya ayarlar olmadığından, analiz VM'nizin normal bir son kullanıcının bilgisayarı gibi görünmesi tamamen size bağlıdır. 
VM'nizde benzerliği sağlamak için aşağıdaki önerileri uygulayabilirsiniz:
Son kullanıcılar tarafından sıkça tercih edilen Chrome ve Firefox gibi tarayıcıların kurulması,
Saldırganın ilgisini çekecek farklı dizinlerde dosyalar bırakılması,
Masaüstü arka planının değiştirilmesi,
Tarayıcı üzerinden küçük uygulamalar indirilerek İndirilenler dizininde bazı dosyaların bulunmasının sağlanması
Ağ Ayarlarını Değiştirin
Kötü amaçlı yazılımın ağ bağlantısı üzerinden farklı cihazlara yayılmasını önlememiz gerekiyor. 
Sanallaştırma yazılımları tarafından sağlanan özel ağlar sayesinde, kötü amaçlı yazılımın farklı cihazlara bulaşmasını önleyebiliriz.
Bunun için, VMware Workstation'ın üst menüsündeki "VM" menüsüne tıklayıp "Ayarlar"ı seçmelisiniz.
Açılan pencerenin sol menüsünden "Ağ Adaptörü"nü seçerek "Özel" ayarını seçmelisiniz.
```

#### 11. Son Kullanıcı Sistemi Taklidi Yapın
```
Sisteminizde kötü amaçlı yazılım veya fidye yazılımı analizi yaptıktan sonra işletim sisteminiz fonksiyonel olarak etkilenebilir veya kullanılamaz hale gelebilir. 
Bir kötü amaçlı yazılımı çalıştırıp analiz ettikten sonra yeni bir kötü amaçlı yazılımı analiz etmek istediğinizde, işletim sisteminizin analiz ettiğiniz eski kötü amaçlı yazılımın yaptığı değişikliklerden etkilenmesini istemezsiniz.
Bu gibi durumlarda, sanallaştırma yazılımlarının Anlık Görüntü özelliğinden faydalanabilirsiniz.
Anlık Görüntü, Sanal Makinenizin bir anlık görüntüsünü almanızı ve daha sonra bu yedeklemeye geri dönebilmenizi sağlayan bir özelliktir.
Malware analizi için VM'mizi yapılandırdık ve analizde kullanacağımız uygulamaları içine kurduk. 
Bu aşamada, bir Anlık Görüntü alabilir ve temiz VM'nizle aynı analiz ortamına geçiş yapabilirsiniz.
Anlık görüntüler almak için, VMware Workstation uygulamasının üst menüsündeki "VM" menüsüne tıklayarak Anlık Görüntü Yöneticisi ekranına erişebilirsiniz, "Anlık Görüntü" -> "Anlık Görüntü Yöneticisi" seçeneklerine tıklayarak.
Daha sonra VM'nizin bir anlık görüntüsünü almak için "Anlık Görüntü Al" butonuna tıklayabilirsiniz. 
Anlık görüntü almak bu kadar kolaydır.
Açıklama bölümüne detaylı bilgi girmeniz, ihtiyacınız olan Anlık Görüntüyü kolayca bulmanızı sağlar. 
Bu nedenle, mümkün olduğunca açıklayıcı yorumlar girmenizi öneririm.
```

<hr/>

</br>


<h2> [Day-24] January 24, 2024 : Malware Analysis Fundamentals - Step 05 | [EN] </h2>

<h3> Dynamic Malware Analysis | Virtual Machine Creation </h3> 

#### 1. Install Virtualization Software
```
XXX
```

#### 2. Install Operating System
```
XXX
```

#### 3. Disable Anti-malware Solutions
```
XXX
```

#### 4. Rename Your Virtual Operating System
```
XXX
```

#### 5. Disable Automatic Updates
```
XXX
```

#### 6. Disable Hidden Extensions
```
XXX
```

#### 7. Show Hidden Files and Folders
```
XXX
```

#### 8. Disable ASLR (Address Space Layout Randomization)
```
XXX
```

#### 9. Disable Windows Firewall
```
XXX
```

#### 10. Mimic End-User System
```
XXX
```

#### 11. Mimic End-User System
```
XXX
```