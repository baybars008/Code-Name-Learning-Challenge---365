<h2> [Day-15] January 15, 2024 : Malware Analysis Course | [TR] </h2> 

#### 1. Malware Analysis, SOC Analistlerine nasıl yardımcı olur?
```
Malware Analysis (Kötü Amaçlı Yazılım Analizi), SOC (Güvenlik Operasyon Merkezi) analistleri için son derece önemli bir beceridir. Stuxnet gibi karmaşık kötü amaçlı yazılımların varlığı ve etkileri, güvenlik analistlerinin bu alandaki bilgi ve yeteneklerinin ne kadar kritik olduğunu gösteriyor.

Bir güvenlik analistinin iş rutini incelendiğinde, analistlerin sık sık şüpheli dosya veya işlemlerle karşılaştığı görülecektir. Çoğu siber saldırıda kötü amaçlı yazılım kullanıldığı düşünüldüğünde, bu tür bilgilere sahip olmanın olağandışı olmadığını anlayabilirsiniz.

Bir Güvenlik Analisti olarak, bu dosyaların zararlı olup olmadığını analiz edebilmelisiniz; eğer zararlı ise, bu yazılımın amacını anlamalı ve komuta kontrol sunucularıyla nasıl iletişim kurduğunu anlamalısınız. Kötü amaçlı yazılım analizi, Güvenlik Analistleri için vazgeçilmez bir bilgi ve yetenektir.

Şüpheli dosyaları incelemek için birçok kötü amaçlı yazılım analizi yöntemi ve teknik bulunmaktadır. Bu eğitim serisinde, ihtiyacınıza en uygun teknikleri kullanarak kötü amaçlı yazılımları analiz edebilirsiniz.
```

#### 2. Kötü Amaçlı Yazılım Tanımı ve Kötü Amaçlı Yazılım Türleri
```
Malware, "MALicious softWARE" kelimelerinin birleşiminden türetilmiş bir terimdir ve kötü niyetli amaçlarla sistemlerin güvenliğini ve bütünlüğünü tehlikeye atan yazılımlara verilen isimdir.

Günümüzde siber tehdit aktörleri, kalıcılığı sağlama, sistemleri zarar verme veya fidye talepleri gibi çeşitli amaçlar için kötü amaçlı yazılımları kullanırlar. Bir SOC analisti olarak, şüpheli yazılımları analiz etmeli ve yazılımın gerçekten zararlı olup olmadığını anlamalısınız.

Programlama dillerinin hemen hemen hepsinde kötü amaçlı yazılımlarla karşılaşabilirsiniz. Kötü amaçlı yazılım analizi yapmak için tüm programlama dillerini bilmeye gerek yoktur, ancak programlamaya aşina olmak kötü amaçlı yazılım analizini kolaylaştırır (bazı durumlarda tersine mühendislik gibi konularda zorunludur).

Her geçen gün, siber tehdit aktörlerinin kendilerini geliştirdiklerini ve daha karmaşık kötü amaçlı yazılımlar geliştirdiklerini görüyoruz. Saldırganlar, kötü amaçlı yazılımlarının analizini daha da zorlaştırmak için çeşitli yöntemler kullanmaktadır.

Bu süreçte, güncel tehditlere karşı hazır olmak için kendimizi sürekli olarak geliştirmemiz gerekmektedir.

Bir SOC analisti olarak, günlük çalışma rutininizde birçok şüpheli dosya ile karşılaşacaksınız. Bu dosyalar, e-posta yoluyla gelmiş olabilir, kullanıcı cihazındaki antivirüs yazılımı tarafından tespit edilmiş olabilir veya transfer edilirken ağ güvenliği ürünleri tarafından tespit edilmiş olabilir.

Analiz sonucunda, dosyanın zararlı olup olmadığını bulabileceksiniz; eğer zararlı ise amacı, komuta ve kontrol sunucuları ve kötü amaçlı yazılımın türünü belirleyebileceksiniz.
```

#### 3. Malware Türleri
``` 
Komuta ve kontrol sunucularının isimleri ve kullandıkları yöntemler değişse de kötü amaçlı yazılımların amaçları belirli kategoriler içinde bulunur. Bu sayede, kötü amaçlı yazılımın kategorisini söyleyerek başka bir kişiyi ne hakkında bilgilendirebileceğinizi basitçe iletebilirsiniz.

Örneğin, incelediğiniz yazılımın bir tuş kaydedici (keylogger) olduğunu söylerseniz, herkes bu yazılımın klavyede basılan tuşları kaydeden bir yazılım olduğunu bilecektir. Bu önemli başlangıç bilgisini üst yönetim veya saldırganın hedefi hakkında fikir vermek için kullanabilir ve ardından detaylı analiz raporunu takip edebilirsiniz.

Bahsettiğimiz gibi, kötü amaçlı yazılımlar işlevleri/amaçları/karakteristikleri doğrultusunda türlerine ayrılırlar. Kötü amaçlı yazılığı analiz ettikten sonra, bu türlerden biriyle eşleştireceksiniz. Bu nedenle bu türlerin neler olduğunu bilmelisiniz.

Bazı kötü amaçlı yazılım türleri ve açıklamaları şunlardır:

• Arka kapı (Backdoor): Malware'ın kurulu olduğu cihazda bir arka kapı bırakarak saldırganın bu arka kapı aracılığıyla sisteme erişmesine izin verir. Örneğin, kabukla bağlantılı bir ağ bağlantısı açarak saldırganın bu bağlantı üzerinden sisteme erişmesini sağlar.

• Reklam yazılımı (Adware): Genellikle indirilen yazılımlarla gelir ve istenmeyen reklamların cihazda görüntülenmesine neden olur. Tüm reklam yazılımları zararlı olmasa da bazıları varsayılan arama motorunu değiştirir.

• Fidye yazılımı (Ransomware): Son birkaç yıldır dünya gündeminde olan bir kötü amaçlı yazılım türüdür. Tüm dosyaları şifreleyerek ve dışa aktararak insanlardan fidye talep eder.

• Virüs (Virus): Vahşi doğada görülen ilk kötü amaçlı yazılım türlerinden biridir. Bu nedenle günlük yaşamda sık sık "virüs" terimi yerine kullanılır. Virüsler kendilerini kopyalama özelliğine sahiptir ve diğer dosyalara bulaşarak kalıcılık sağlarlar.

• Solucan (Worm): Bu tür kötü amaçlı yazılım, enfekte cihazlardan diğer cihazlara yayıldığı için "solucan" olarak adlandırılır. MS17-010 zafiyetini kullanarak yayılan WannaCry, dünya genelinde panik yarattı.

• Kök kit (Rootkit): Kendisini gizleyen ve cihazda yüksek düzeyde yetki sağlayarak çalışan bir kötü amaçlı yazılım türüdür.

• Uzaktan Erişim Truva Atı (RAT - Remote Access Trojan): Cihaz üzerinde tehdit aktörüne tam kontrol sağlayan bir kötü amaçlı yazılım türüdür.

• Bankacılık yazılımı (Banking malware): Bankacılık uygulamalarını hedef alan ve kurbandan para çalmasına neden olan bir tür kötü amaçlı yazılımdır.

• Tuş kaydedici (Keylogger): Basılan tuşları kaydeden ve bu bilgiyi saldırgana ileten bir tür kötü amaçlı yazılımdır.

Bir kötü amaçlı yazılım birden fazla özelliği içerebileceği için, bir kötü amaçlı yazılım birden fazla türe ait olabilir. Örneğin, WannaCry kötü amaçlı yazılımı hem solucan hem de fidye yazılımı özelliklerini içerir.
```

#### 4. Malware Analyst Neleri Bilmesi Gerekir?
```
Kötü amaçlı yazılım analizi, dışarıdan kolay gibi görünebilecek bir konu olabilir, ancak esasen birçok farklı yönüyle uzmanlık gerektiren bir alandır. Kötü amaçlı yazılım analizi, kendi başına ayrı bir alan olmasına rağmen, bazı Tier 3 SOC Analistleri (Konu Uzmanları), kariyerlerini sadece kötü amaçlı yazılım analizine odaklarlar. Kötü amaçlı yazılım analizi ayrı bir alan olsa da, güvenlik analistleri günlük çalışma rutinlerinde sıklıkla kullanır.

Kötü amaçlı yazılımı doğru ve başarılı bir şekilde analiz edebilmek için birçok konuda temel bilgilere sahip olmak gereklidir.
```

#### 5. İşletim Sistemi Temelleri ve Mimarisi
```
Kötü amaçlı yazılım, işletim sistemlerinde çalıştığı için, kötü amaçlı yazılım analistlerinin işletim sistemleri konusunda sağlam bir anlayış ve bilgiye sahip olmaları gerekmektedir.

Kötü amaçlı yazılım genellikle işletim sistemi tarafından sunulan özellikleri kullanır, ayrıcalıklarını artırır, keşif yapar ve kalıcılığı sağlar. Windows işletim sistemleri üzerinde bir örnek vermek gerekirse, kötü amaçlı yazılım, Görev Zamanlayıcı, Hizmetler, Kayıt Defteri gibi işletim sistemi özelliklerini kalıcılığı sağlamak için kullanır.

İşletim sisteminin özelliklerinin yanı sıra, API'ler, Sistem Çağrıları (Syscalls), Bellek Mimarisi ve daha düşük seviye konular da başarılı kötü amaçlı yazılım analizi için önemlidir. Bu konulara daha fazla odaklanacağız "Statik Kötü Amaçlı Yazılım Analizi" eğitiminde.
```

#### 6. Assembly Dili ve Programlama
```
Eğer yazılım geliştirdiyseniz, yazdığınız programlama dillerini derlediğinizde neler olduğunu hiç merak ettiniz mi? Ya da birçok programlama dili olduğunda işlemcilerin bu dilleri nasıl çalıştırdığını merak ettiniz mi?

İşlemciler sadece 0 ve 1'leri anlar. 0 ve 1 haricindeki tüm veriler işlemcilere anlamsızdır. C/C++, Python, Java, Ruby, Go gibi dillerde herhangi bir programı derlediğinizde, derleyiciler yazdığınız kodları işlemcinin anlayabileceği 0 ve 1'lere çevirirler. Bir programı başlattığınızda, bu 0 ve 1'ler bellek üzerinden işlemciye gönderilir ve çalıştırılır.

0 ve 1'leri dikkate almadığımızda görebileceğiniz en düşük seviye programlama dili Assembly'dir. Her talimatın doğrudan bir 0 ve 1 karşılığı vardır. C ile yazılmış bir programı derlediğinizde önce Assembly diline çevrilir ve ardından 0 ve 1'lere dönüştürülür.

Derlenmiş kötü amaçlı yazılımlar kolayca Assembly diline dönüştürülebilir. Ancak Assembly dilinden sonraki seviyeye çevirmek çok da kolay ve kesin değildir, bu nedenle analizler genellikle Assembly dilinde yapılır. Makine kodlarını Assembly diline çeviren yazılıma "Disassembler" denir.

Statik kod analizi eğitiminde, "Assembly" Dilinin temellerine de odaklanacağız.

START
Preprocessor>>hello_world.c
Compiler>>hello_world.i
Assembler>>hello_world.s
END
Executable>>hello_world.exe
```

#### 7. Ağ Protokolleri ve Temelleri
```
Kötü amaçlı yazılım genellikle bilgi ele geçirmek, komuta kontrol sunucusuna bağlanmak veya ikincil yükleri indirmek amacıyla ağ etkinliği gösterir. Kötü amaçlı yazılımı analiz ederken bu ağ trafiğini anlamak, kötü amaçlı yazılımın amacını anlamamız için son derece önemlidir.

Bu nedenle, kötü amaçlı yazılım analistlerinin temel ağ bilgisine sahip olmaları gerekmektedir.
```

#### 8. Kriptografi
```
Birçok teknoloji, güvenlik sağlamak için kriptografiyi kullanırken, saldırganlar da tespiti zorlaştırmak ve erişimi engellemek gibi amaçlarla kriptografiyi kullanır.

Günümüzde popüler fidye yazılımları, dosyaları şifreleyerek dosyalara erişimi fidye ödenmedikçe engellemek için kriptografiyi kullanır.

Kötü amaçlı yazılım analizi sırasında sıklıkla kriptografi ile karşılaşırız.
```

#### 9. Kötü Amaçlı Yazılımları Analiz Ederken Hangi Yaklaşımı Seçilmeli?
```
Siber güvenlik savunma alanında çalışanların sıklıkla karşılaştığı bir görev olan zararlı yazılım analizi ve bu analizin iki farklı yaklaşımı ele alınmaktadır: Statik Analiz ve Dinamik Analiz.

Statik Analiz: Bu yöntem, zararlı yazılımın çalıştırılmasına gerek kalmadan, kodunun incelenmesiyle gerçekleştirilir. Statik analiz, zararlı yazılımın yapısını, kullanılan kodları ve potansiyel davranışlarını anlamaya yardımcı olur. Bu yaklaşımın avantajı, zararlı yazılımı çalıştırmadan önce güvenli bir şekilde analiz edebilme yeteneğidir. Dezavantajı ise, bazı karmaşık zararlı yazılımların gizli özelliklerinin ve davranışlarının sadece çalıştırıldığında ortaya çıkması nedeniyle bu özellikleri kaçırma riskidir.

Dinamik Analiz: Dinamik analiz, zararlı yazılımın kontrollü bir ortamda (genellikle bir sanal makine içinde) çalıştırılmasını ve davranışlarının gözlemlenmesini içerir. Bu yöntem, zararlı yazılımın gerçekte ne yaptığını anlamak için kullanılır; ağ trafiği, dosya işlemleri ve sistem değişiklikleri gibi gerçek zamanlı etkilerini izler. Dinamik analizin avantajı, zararlı yazılımın aktif olarak neler yapabileceğini gözlemleyebilme yeteneğidir. Dezavantajı ise, bu analiz sırasında zararlı yazılımın bazı zararlı eylemleri gerçekleştirmesi ve bu sürecin daha riskli olmasıdır.

Her iki yöntemin de avantajları ve dezavantajları birbirine tamamlayıcı niteliktedir. Bu nedenle, kapsamlı bir zararlı yazılım analizi için genellikle her iki yöntemin birleştirilerek kullanılması önerilir. Bu, zararlı yazılımın daha derinlemesine anlaşılmasını ve etkili bir şekilde mücadele edilmesini sağlar.
```

#### 10. DevOps Pipeline (DevOps Boru Hattı)
```
Dağıtım yaşam döngüleri, yazılım geliştirme için kullanılır.
Pipeline, yazılımı bir yerden bir yere taşıyan süreç ve araçtır. Genellikle altı aşamaya ayrılır. Bunlar:
• Planning(Planlama): Projeleri ve yol haritalarını planlayın.
• Develop (Geliştirmek): Bu, kod yazdığınız aşamadır.
• Build (İnşa etmek): Kod bir yapıtın içine yerleştirilir.
• Test: Oluşturulan eserin test edilmesi.
• Release (Serbest Bırak): Kod üretime hazır hale gelmeden önce son kontrol.
• Monitor (Monitör): Metrikler ve veri toplama aşaması.
```

#### 8. Containers and Container Orchestrations (Konteynerler ve Konteyner Orkestrasyonları)
```
• Container Architecture (Konteyner Mimarisi)
!\[Alt text\](all-images/image.png)
• OS-Level Virtualization (İşletim Sistemi Düzeyinde Sanallaştırma)
• namespaces (isim Alanları)
• C groups (C grupları)
• Container Orchestration (Konteyner Orkestrasyonu)
!\[Alt text\](all-images/image-1.png)
• Kubernetes
• Manages discovery (Keşfi Yönetir)
• Batteries included (Piller Dahildir)
• Open-Source
```

#### 9. Benefits of Cloud Computing (Bulut Bilişimin Faydaları)
```
• Different Technologies (Farklı Teknolojiler)
• Scaling Resources (Ölçeklendirme Kaynakları): Hizmetlerinizin ölçeklendirilmesini otomatikleştirebilirsiniz.
• Cost Savings (Maliyet Tasarufu): Talep üzerine fiyatlandırma ile yalnızca kullandığınız kadar ödersiniz.
• Global Reach (Küresel Erişim): Uygulamanızı saniyeler içinde dünya çapında çalıştırabilirsini
```

#### 10. Cloud Computing Service Models (Bulut Bilişim Hizmet Modelleri)
```
Overview of DevOps and Cloud Computing (DevOps ve Bulut Bilişime Genel Bakış)
• Three Service Models (Üç Hizmet Modeli)
   ◇ IaaS -- Infrastructure as a Service (Hizmet Olarak Altyapı)
   ◇ PaaS -- Platform as a Service (Hizmet Olarak Platform)
   ◇ SaaS -- Software as a Service (Hizmet Olarak Yazılım)
```

#### 11. Cloud Computing Deployment Models (Bulut Bilişim Dağıtım Modelleri)
```
• Four Deployment Models (Dört Dağıtım Modeli)
   ◇ Public: Altyapı ve hizmetlere internet üzerinden erişilmektedir.
   ◇ Hybrid: Özel ve kamu modellerinin kombinasyonu.
   ◇ Private: Altyapı ve hizmetlere özel bir veri merkezinden erişilir ve hizmet verilir.
   ◇ Multi: Altyapı ve hizmetlere iki veya daha fazla bulut sağlayıcısı üzerinden erişilir ve hizmet sunulur.
```

<hr/>

</br>

<h2> \[Day-10\] January 10, 2024 : Hands-on Linux for DevOps & Cloud Engineers | \[EN\] </h2> 

</br>

<h3> Introduction to Linux </h3> 

</br>

#### 1. Introduction to Linux
```
What is Linux?
Linus Benedict Torvalds is the developer and project manager of the Linux operating system kernel. Linux is comprised of three fundamental components:
• Kernel: The core foundation of the operating system.
• Applications: Software tools to perform various tasks.
• System Userspace: The administrative layer of tasks for the system.
```

#### 2. What is Linux used for?
```
There are six key reasons to choose Linux:

• Security: Linux is a secure kernel and operating system.
• Free and Open-Source: The Linux kernel is distributed free of charge.
• Stability: The Linux kernel and operating system are stable.
• Development: Linux is an excellent platform for development.
• Batteries Included: Linux comes preloaded with most things you need.
• Runs Everywhere: Linux has been ported to numerous platforms.
```

#### 3. Why use Linux
``` 
Common uses of Linux include:

• Cloud Computing: Linux forms the fundamental infrastructure for Cloud Providers.
• Internet: Linux powers the internet.
• Mobile: Linux is used in 85% of mobile devices.
• IoT: Linux is employed in IoT devices.
• Super Computing: Linux comes preloaded with most of the necessities right out of the box.
• Virtualization: Virtualization is a first-class citizen on Linux.
```

#### 4. Principles of DevOps
```
• Culture: Strategy for fostering an inclusive and productive work environment.
• Automation: The most crucial tool in the arsenal.
• Lean: Controlling the flow within your system for efficiency.
• Measurement: The act of understanding the status of your system.
• Sharing: Encourages openness and transparency within teams and processes.
```

#### 5. Why Should DevOps be Implemented?
```
• Technical Benefits: Advantages that enhance the technological aspects.
• Cultural Benefits: Improvements in the work culture and team dynamics.
• Business Improvements: Enhancements that positively impact business operations and outcomes.
```

#### 6. DevOps Terminologies
```
There's a wealth of technical knowledge, but I've focused on just the common 10 terms.

• Configuration Management: Managing settings and configurations of software and hardware.
• Infrastructure as Code: Managing and provisioning infrastructure through code instead of manual processes.
• Continuous Integration: Merging all developers' working copies to a shared mainline several times a day.
• Continuous Delivery: Automatically preparing code changes for release to production.
• Continuous Deployment: Automatically releasing developer changes from the repository to production.
• Continuous Monitoring: Ongoing process of detecting and resolving issues within a system.
• Mean Time To Recovery: Average time to recover from a system failure.
• Idempotent: A method that produces the same result whether called once or multiple times.
• Imperative: Specifying a sequence of operations to perform.
• Declarative: Specifying the desired state, without detailing the steps to achieve it.
```

#### 7. DevOps Pipeline
```
Deployment life cycles are used in software development. 
The pipeline is the process and tool for moving software from one place to another. 
It is generally divided into six stages:
• Planning: Plan projects and roadmaps.
• Develop: This is the stage where you write the code.
• Build: The code is placed into a build.
• Test: Testing the created build.
• Release: The final check before the code is ready for production.
• Monitor: The stage of collecting metrics and data.
```

#### 8. Containers and Container Orchestrations
```
• Container Architecture
!\[Alt text\](all-images/image.png)
• OS-Level Virtualization
• namespaces
• C groups
• Container Orchestration
!\[Alt text\](all-images/image-1.png)
• Kubernetes
• Manages discovery
• Batteries included
• Open-Source
```

#### 9. Benefits of Cloud Computing
```
• Different Technologies
• Scaling Resources: You can automate the scaling of your services.
• Cost Savings: With pay-as-you-go pricing, you only pay for what you use.
• Global Reach: You can run your application worldwide in seconds.
```

#### 10. Cloud Computing Service Models
```
Overview of DevOps and Cloud Computing
• Three Service Models
   ◇ IaaS -- Infrastructure as a Service
   ◇ PaaS -- Platform as a Service
   ◇ SaaS -- Software as a Service
```

#### 11. Cloud Computing Deployment Models
```
• Four Deployment Models
   ◇ Public: Infrastructure and services are accessed over the internet.
   ◇ Hybrid: A combination of private and public models.
   ◇ Private: Infrastructure and services are accessed and served from a private data center.
   ◇ Multi: Infrastructure and services are accessed and served through two or more cloud providers.](January-11-2024.md)