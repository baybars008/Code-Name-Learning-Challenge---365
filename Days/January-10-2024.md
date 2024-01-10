<h2> [Day-1] January 1, 2024 : Hands-on Linux for DevOps & Cloud Engineers | [TR] </h2> 

</br>

<h3> Introduction to Linux </h3> 

</br>

#### 1. Introduction to Linux
```
What is Linux?
Linus Benedict Torvalds Linux işletim sistemi çekirdeğinin geliştiricisi ve proje yöneticisi.
Linux üç temel yapıdan oluşur:
• Kernel: İşletim sisteminin temel kuruluşu.
• Applications: Kullanabileceğiniz yazılımlar için görevleri gerçekleştirmek.
• System Userspace: Sistem için idari katman Görevleri
```

#### 2. What is Linux used for?
```
Linux tercih etmek için altı madde:
• Security: Linux güvenli bir çekirdek ve işletim sistemidir.
• Free and Openb-Source: Linux çekirdeği ücretsiz olarak dağıtılmaktadır.
• Stability: Linux çekirdeği ve işletim sistemi kararlı bir yapıdadır.
• Development: Linux harika bir geliştirme platformudur.
• Batteries Included: Linux, ihtiyacınız olan çoğu şeye önceden yüklenmiş olarak gelir.
• Runs Everywhere: Linux sayısız platforma taşındı.
```

#### 3. Why use Linux
``` 
Yaygın Linux kullanım örnekleri:
• CLoud Computing: Linux, Bulut Sağlayıcıları için temel altyapıdır.
• Internet: Linux interneti çalıştırır.
• Mobile: Linux mobil cihazların %85'inde kullanılıyor.
• IoT: Linux loT cihazlarında kullanılmaktadır.
• Super Computing: Linux, kutudan çıktığında ihtiyacınız olan çoğu şeyle önceden yüklenmiş olarak gelir.
• Virtualization: Sanallaştırma Linux üzerinde birinci sınıf bir vatandaştır.
```
</br>

<h3> Overview of DevOps and Cloud Fundamentals </h3> 

</br>

#### 1. Introduction to DevOps
```
• Devoops terimi iki kelimeden oluşan bir karışımdır: Geliştirme ve operasyonlar.
• 2009 yılında Patrick Dubols tarafından dile getirilmiştir.
• Ancak devops fikri ve öntemleri, toyata'nın öncü olduğu yalın üretim sisteminden ödünç alınmıştır.
   ◇ (Yalın üretim nedir: Yalın üretimimizi bir çekme sistemine göre üretimimize ve işimize uyguluyoruz; bu da yalnızca sipariş verdiğiniz ürünü ürettiğimiz anlamına geliyor. Bu sayede, her şeyi zamanında üretebilir, sorunsuz bir iş akışı üretiriz.)
```

#### 2. Devops'da akıllıca adlandırılmış üç ana kavram vardır.
```
• Systems and Flow: Sistemin hızı.
• Feedback: Amaç, iyileştirme göz önünde bulundurularak sıkı geri bildirim döngüleridir.
• Continuous Experimentation and Learning: Başarısızlıktan ders alın ve sistemi değiştirmeye devam edin.
```

#### 3. Devops neden uygulanmalı?
```
• Technical Benefits (Teknik Faydalar)
• Cultural Benefits (Kültürel Faydalar)
• Business Improvements (İş İyileştirmeleri)
```

#### 4. DevOps İlkeleri
```
• Culture(kültür): strateji
• Automation(otomasyon): Cephanelikdeki en önemli araç.
• Lean(Yalın): Sisteminizdeki akışın kontrolü.
• Measurement (ölçüm): Sisteminizin durumunu anlama eylemi.
• Sharing (paylaşım): Paylaşım, açıklığı ve şeffaflığı teşvik eder.
```

#### 5. Devops neden uygulanmalı?
```
• Technical Benefits (Teknik Faydalar)
• Cultural Benefits (Kültürel Faydalar)
• Business Improvements (İş İyileştirmeleri)
```

#### 6. DevOps Terminolojileri
```
Bir ton teknik bilgi var fakat sadece yaygın 10 tanesini ele aldım.
• Configuration Management (Konfigürasyon Yönetim)
• Infrastructure as Code (Kod Olarak Altyapı)
• Continuous Integration (Sürekli Entegrasyon)
• Continuous Delivery (Sürekli Teslimat)
• Continuous Deployment (Sürekli Dağıtım)
• Continuous Monitoring (Sürekli İzleme)
• Mean Time To Recovery (Ortalama İyileşme Süresi) 
• Idempotent (Etkisiz -- Bir metodun bir defa çağrıldığında alınan sonuç ile birden fazla kez çağrıldığında alınan sonuç aynı ise bu bir idempotent metottur.)
• Imperative (Zorunluluk)
• Declarative (Bildirimsel)
```

#### 7. DevOps Pipeline (DevOps Boru Hattı)
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
![Alt text](all-images/image.png)
• OS-Level Virtualization (İşletim Sistemi Düzeyinde Sanallaştırma)
• namespaces (isim Alanları)
• C groups (C grupları)
• Container Orchestration (Konteyner Orkestrasyonu)
![Alt text](main/all-images/image-1.png)
• Kubernetes
• Manages discovery (Keşfi Yönetir)
• Batteries included (Piller Dahildir)
• Open-Source
```

<hr/>

</br>

<h2> [Day-1] January 1, 2024 : Hands-on Linux for DevOps & Cloud Engineers | [EN] </h2> 

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