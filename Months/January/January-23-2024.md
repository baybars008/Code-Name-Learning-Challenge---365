<h2> [Day-23] January 23, 2024 : Malware Analysis Temelleri - Adım 04 | [TR] </h2> 

<h3> Dinamik Kötü Amaçlı Yazılım Analizi | İhtiyaç Olan Araçlar Listesi </h3> 

#### 1. Sanallaştırma Yazılımı
```
"Kötü yazılımın faaliyetlerini inceleyebilmek için onu çalıştırmamız gerektiği için, dinamik analizi kendi sistemimiz üzerinde yapmak istemeyiz. 
Bu nedenle, bazı sanal sistemler üzerinde çalışmamıza yardımcı olan Sanallaştırma Yazılımlarından faydalanmalıyız.

Bu yazılımlar sayesinde, ana işletim sisteminizde farklı bir işletim sistemini kullanabilirsiniz. 
Doğru şekilde yapılandırıldıklarında, kötü amaçlı yazılım bu sanal işletim sisteminden kaçamaz ve analizlerinizi güvenli bir şekilde gerçekleştirebilirsiniz. 
Bu sanallaştırma yazılımları hakkında küçük bir not düşmek yararlı olacaktır. 
Bu sanal ortamlar temelde yazılım oldukları için, kötü amaçlı yazılımların bu sanal ortamlardan kaçmasına ve ana işletim sistemine kod yürütmesine olanak tanıyan çeşitli güvenlik açıkları ortaya çıkabilir. 
Bu nedenle, sanallaştırma yazılımınızı güncel tutmak hayati önem taşır.

Sıkça kullanılan bazı sanallaştırma yazılımları şunlardır;

• VMware Workstation
• VMware Fusion
• Oracle Virtualbox

İdeal izole dinamik analiz ortamı, tamamen ayrı bir fiziksel cihaz ve ayrı bir ağdan oluşur. 
Ancak, bu karmaşık ortamın kurulması hem çok maliyetlidir hem de başlangıç için gerekli değildir."
```

#### 2. Yardımcı Yazılımlar
```
"Kendi sanal işletim sisteminizi kurduktan sonra, dinamik analizde işinize yarayacak yazılımları yüklemeniz gerekecek. 
Örneğin, docx, xlsx gibi dosya uzantılarına sahip ofis dosyalarının dinamik analizini, sisteme Microsoft Office veya benzeri yazılımlar kurmadan yapamayız.

• Microsoft Office
• Adobe Reader
• Tarayıcı (Chrome, Firefox vb.)
• WinRAR
• Metin Düzenleyicileri (Notepad++, Sublime Text vb.)

Saldırganlar, dinamik analiz yöntemiyle oldukça aşinadır. 
Bu yüzden, kötü amaçlı faaliyetlerini ele geçirdikleri cihazlarda gerçekleştirmeden önce, kötü amaçlı yazılımın sanal bir işletim sisteminde çalışıp çalışmadığını belirleyebilmek için hedef sistemde sıklıkla kullanılan yazılımların kurulu olup olmadığını kontrol ederler."
```

#### 3. Hata ayıklayıcılar
```
"Hata ayıklayıcılar (debuggers), genellikle programcılar tarafından kodları test etmek ve hataları yakalamak için kullanılan yazılımlardır. 
Hata ayıklayıcılar, bir sürecin talimatlarını görmemize ve programın akışını değiştirmemize yardımcı olur.

Kötü yazılım analistleri, sıkça hata ayıklayıcıları kullanarak kötü amaçlı yazılımın çalışma yapısını öğrenir ve kötü yazılım kodlarında değişiklik yaparak bazı önleme mekanizmalarını devre dışı bırakır.

Örneğin, cihaz adı 'John' olmadığında çalışmayan bir kötü amaçlı yazılımı analiz etmek istiyorsunuz. 
Hata ayıklayıcı yardımıyla, bu kontrolün yapıldığı kodlarda değişiklik yaparak bu kontrolü devre dışı bırakabilir ve kötü amaçlı yazılımın çalışmaya devam etmesini sağlayabilirsiniz.

Bu eğitim başlangıç seviyesi konuları ele aldığı için, hata ayıklama hakkında detaylı bilgi vermeyeceğiz, ancak gelecekteki eğitimlerimizde bunları kullanacağımız için, şimdi hata ayıklayıcıları yüklemek işimizi kolaylaştıracak."

Kötü yazılım analistleri tarafından sıklıkla tercih edilen bazı hata ayıklayıcılar şunlardır:

• Ollydbg
• X64dbg
• Windbg
• Radare2
```

#### 4. Ağ İzleme Araçları
```
"Kötü amaçlı yazılımın kurduğu ağ bağlantıları, iletişim kurduğu adresler ve bu adreslerle nasıl iletişim kurduğu gibi bilgiler, kötü yazılım analizinin sonucu olarak raporlanmalıdır."

Kötü amaçlı yazılımın ağ aktivitelerini tespit etmek için bazı yazılımlara ihtiyacımız var. Bunlardan bazıları şunlardır:

• Wireshark
• Fiddler
• Burp Suite
```

#### 5. Süreç İzleme Araçları
```
"Kötü yazılım analizi için çalıştırdığımız program için yeni bir süreç oluşturulur. 
Bu süreçleri izlemek için süreç izleme araçlarını kullanmalıyız.

Windows zaten “Görev Yöneticisi” adında bir süreç izleme aracı ile gelir. 
Ancak, diğer süreç izleme araçları, kullanım ve özellikler açısından kötü yazılım analizi için daha yararlıdır.

Dinamik kötü yazılım analizi için oluşturacağımız sanal işletim sistemine aşağıdaki süreç izleme araçlarını yükleyebilirsiniz."

• Process Hacker
• Process Explorer (SysInternals)
• Procmon (SysInternals)
```

#### 6. Dosya Etkinliği İzleme Araçları
```
“Dinamik analizde izlenmesi gereken ilk faaliyetlerden biri dosya aktiviteleridir. 
Kötü amaçlı yazılım, işletim sisteminden bilgi toplamak için dosyaları okuyabilir, kötü amaçlı yazılımın diğer bileşenlerini dosya sistemine yazabilir ve devamlılığını sağlamak için kendisini başlangıç klasörüne taşıyabilir. 
Bu ve benzeri nedenlerle kötü amaçlı yazılım dosya sisteminde çeşitli aktivitelerde bulunabilir. 
Kötü yazılım analizi raporunda bu aktiviteleri tespit edip belirtmemiz gerekmektedir.”

Dosya aktivitelerini görmek için aşağıdaki araçları kullanabilirsiniz.

• Sysmon
```

#### 7. Diğer Araçlar
```
• SysInternal Tools
• CFF Explorer
• PEView
• TriDNet
• BinText
• PEiD
• Regshot
• HashMyFiles
```

<hr/>

</br>


<h2> [Day-23] January 23, 2024 : Malware Analysis Fundamentals - Step 04 | [EN] </h2>

<h3> Dynamic Malware Analysis | List of Needed Vehicles </h3> 

#### 1. Virtualization Software
```
"To examine the activities of malware, we need to run it, which is why we do not want to perform dynamic analysis on our own system. 
Therefore, we should make use of Virtualization Software that assists us in operating on some virtual systems.

Thanks to these software, you can use a different operating system on your main operating system. 
When configured correctly, the malware cannot escape from this virtual operating system, and you can carry out your analyses safely. 
It's useful to make a note about these virtualization software. 
Since these virtual environments are fundamentally software, various security vulnerabilities may emerge, allowing malware to escape these virtual environments and execute code on the main operating system. 
Hence, keeping your virtualization software updated is of vital importance.

Some frequently used virtualization software includes;

• VMware Workstation
• VMware Fusion
• Oracle Virtualbox

The ideal isolated dynamic analysis environment consists of an entirely separate physical device and a separate network. 
However, setting up this complex environment is both very costly and not necessary for beginners."
```

#### 2. Utility Software
```
"After setting up your own virtual operating system, you will need to install software that will be useful for dynamic analysis. 
For instance, we cannot perform dynamic analysis of office files with extensions like docx, xlsx without installing Microsoft Office or similar software on the system.

• Microsoft Office
• Adobe Reader
• Browser (Chrome, Firefox, etc.)
• WinRAR
• Text Editors (Notepad++, Sublime Text, etc.)

Attackers are quite familiar with the dynamic analysis method. 
Therefore, before carrying out malicious activities on the devices they compromise, they check whether the target system has commonly used software installed to determine if the malware can operate in a virtual operating system."
```

#### 3. Debuggers
```
"Debuggers are software tools commonly used by programmers to test code and catch errors. 
Debuggers help us see the instructions of a process and modify the flow of a program.

Malware analysts frequently use debuggers to understand the operational structure of malware and disable certain prevention mechanisms by making changes in the malware code.

For example, you want to analyze malware that does not operate when the device name is not 'John.' 
With the help of a debugger, you can modify the code where this check is performed, disable this control, and enable the malware to continue operating.

Since this training covers beginner-level topics, we won't go into detailed information about debugging. However, since we will use them in future trainings, installing debuggers now will make our work easier."

Some debuggers commonly preferred by malware analysts include:

• Ollydbg
• X64dbg
• Windbg
• Radare2
```

#### 4. Network Monitoring Tools
```
"Information such as the network connections established by the malware, the addresses it communicates with, and how it communicates with these addresses should be reported as a result of malware analysis."

To detect the network activities of malware, we need certain software. Some of these are:

• Wireshark
• Fiddler
• Burp Suite
```

#### 5. Process Monitoring Tools
```
"For malware analysis, a new process is created for the program we run. 
We should use process monitoring tools to monitor these processes.

Windows already comes with a process monitoring tool called 'Task Manager'. 
However, other process monitoring tools are more useful for malware analysis in terms of usability and features.

For the virtual operating system we will create for dynamic malware analysis, you can install the following process monitoring tools."

• Process Hacker
• Process Explorer (SysInternals)
• Procmon (SysInternals)
```

#### 6. File Activity Monitoring Tools
```
"One of the first activities that should be monitored in dynamic analysis is file activities. 
Malicious software can read files to gather information from the operating system, write other components of the malware to the file system, and move itself to the startup folder to ensure its persistence. 
For these and similar reasons, malware can engage in various activities within the file system. 
In malware analysis reports, we need to detect and document these activities."

To observe file activities, you can use the following tool:

• Sysmon
```

#### 7. Other Tools
```
• SysInternal Tools
• CFF Explorer
• PEView
• TriDNet
• BinText
• PEiD
• Regshot
• HashMyFiles
```