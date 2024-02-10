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
"Before setting up a virtual operating system, we need to install virtualization software that will facilitate this."
Although there are some differences among them, any of the virtualization software will assist us in our dynamic analysis. 
You can install one of the following virtualization software:

• VMware Workstation
• VMware Fusion (for macOS)
• Oracle Virtualbox
```

#### 2. Install Operating System
```
For malware analysis, we need to make some configuration changes in our Virtual Machine.

To download Windows 10 ISO: https://www.microsoft.com/en-us/evalcenter/download-windows-10-enterprise
```

#### 3. Disable Anti-malware Solutions
```
You can open the Local Group Policy Editor application by searching for "edit group policy" in the Start menu. 
Alternatively, you can access the Local Group Policy Editor application by searching for "gpedit.msc" or via the "Search>Run" function in Windows.
To disable Windows Defender using the Local Group Policy Editor application, you need to navigate to the following policy:
“Computer Configuration > Administrative Templates > Windows Components > Microsoft Defender Antivirus”
Here, double-click on the "Turn off Microsoft Defender Antivirus" policy and set it to "Enabled."
Additionally, you should also disable the "Monitor file and program activity on your computer" policy under "Real-Time Protection."
```

#### 4. Rename Your Virtual Operating System
```
Some malware performs various checks to avoid running in analysis environments. 
One of these checks is verifying the host name. 
Since most sandboxes have host names like "Sandbox," "Malware," "Cuckoo," malware is programmed not to run on systems with these names.
Ensuring your VM appears like a regular user's system will help you evade anti-analysis techniques. 
Setting a random name as the host name will aid in bypassing these types of checks.
To change the device name, go to “Settings → System → About” and then click on the “Rename this PC” button.
Don’t forget to change your username as well!
```

#### 5. Disable Automatic Updates
```
The malware we will analyze may be exploiting vulnerabilities in the operating system. 
To ensure the malware can operate as normally as possible, we need to disable automatic updates on our virtual operating system.
You can disable automatic updates through group policy settings.
Open the Local Group Policy Editor application by searching for “edit group policy” in the Start menu. 
Alternatively, you can access the Local Group Policy Editor application by searching for “gpedit.msc” or via the “Search>Run” function in Windows.
Then, you should navigate to the following policy.
“Computer Configuration > Administrative Templates > Windows Components > Windows Update”
After reaching the relevant policy, you must set the "Configure Automatic Updates" policy to "Disabled."
```

#### 6. Disable Hidden Extensions
```
You might have seen attackers change file extensions to deceive their victims. How do they do it?
Windows operating systems are set by default to hide known file extensions. 
So, a file named "Chrome.exe" would appear simply as "Chrome" by default. 
Attackers name their malicious software "Photo.jpg.exe," causing the user to see the file as "Photo.jpg." 
When the user opens the file thinking it's an image, the malware begins to operate.
To avoid confusion during analysis, we need to ensure that extensions hidden by default are always shown.
To do this, open the application called "File Explorer" and click on "File" at the top menu, then click on "Change folder and search options" to access the settings menu.
Then, from the "View" tab, uncheck the "Hide extensions for known file types" option and save the settings.
```

#### 7. Show Hidden Files and Folders
```
Malware aims to prevent users from detecting its files by hiding them. 
Showing hidden files and directories by default will facilitate a more comfortable analysis.
Let's open the application called "File Explorer" and click on "File" in the top menu, then click on "Change folder and search options" to open the settings menu.
Next, from the "View" tab, select "Show hidden files, folders, and drives" and save the setting.
```

#### 8. Disable ASLR (Address Space Layout Randomization)
```
Windows' newer versions feature an anti-exploit security mechanism known as ASLR (Address Space Layout Randomization).
You can disable this setting with the help of the Registry Editor.
Open the Registry Editor application and access the following registry key.
“HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management”
Create a key of type “REG_DWORD” named "MoveImages".
These settings will ultimately disable the ASLR feature.
```

#### 9. Disable Windows Firewall
```
As we've done in previous steps, to prevent interference with the security mechanisms of the malware we are analyzing, we must disable the Windows Firewall.
Access the Windows Defender Firewall settings through the Control Panel.
You can use the search bar at the top of File Explorer to access these settings.
If you copy and search the following path into this search bar, it will take you to the Windows Defender Firewall settings.
"Control Panel\System and Security\Windows Defender Firewall\Customize"
After accessing the Defender Firewall settings, select the option "Turn off Windows Defender Firewall" and save.
This will disable the Firewall.
```

#### 10. Mimic End-User System
```
To avoid detection by anti-analysis techniques of the malware you are analyzing, it's crucial to make your VM resemble a normal end-user operating system as closely as possible.
Since there are no specific instructions or settings for this, how closely your analysis VM mimics a regular user's computer is entirely up to you.
To ensure similarity in your VM, you might consider the following suggestions:
• Installing browsers that are commonly preferred by end-users, such as Chrome and Firefox.
• Placing files in various directories that might draw the attacker's interest.
• Changing the desktop background.
• Downloading small applications through the browser to ensure the presence of some files in the Downloads directory.
• Change Network Settings
We need to prevent the malware from spreading to different devices via network connections. 
With the private networks provided by virtualization software, we can stop the malware from infecting other devices.
To do this, click on the "VM" menu in the top menu of VMware Workstation and select "Settings."
In the window that opens, select "Network Adapter" from the left menu and choose the "Private" setting.
```

#### 11. Mimic End-User System
```
"After conducting malware or ransomware analysis on your system, your operating system can become functionally compromised or unusable. 
You wouldn't want your operating system to be affected by the changes made by the malware you analyzed previously when you want to analyze a new piece of malware.
In such cases, you can benefit from the Snapshot feature of virtualization software.
A Snapshot is a feature that allows you to take an instantaneous image of your Virtual Machine and later revert back to this backup.
We have configured our VM for malware analysis and installed the applications we will use for analysis.
At this stage, you can take a Snapshot and switch to the same analysis environment as your clean VM.
To take snapshots, access the Snapshot Manager screen by clicking on the "VM" menu in the top menu of the VMware Workstation application, then click on "Snapshot" -> "Snapshot Manager."
Then you can click on the "Take Snapshot" button to take a snapshot of your VM.
Taking a snapshot is that easy.
Entering detailed information in the description section helps you easily find the Snapshot you need.
Therefore, I recommend entering as descriptive comments as possible."
```