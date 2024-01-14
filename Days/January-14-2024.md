<h2> [Day-14] January 14, 2024 : Malware Analysis Course | [TR] </h2> 

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
• Preprocessor>>hello_world.c
• Compiler>>hello_world.i
• Assembler>>hello_world.s
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

• Statik Analiz: Bu yöntem, zararlı yazılımın çalıştırılmasına gerek kalmadan, kodunun incelenmesiyle gerçekleştirilir. Statik analiz, zararlı yazılımın yapısını, kullanılan kodları ve potansiyel davranışlarını anlamaya yardımcı olur. Bu yaklaşımın avantajı, zararlı yazılımı çalıştırmadan önce güvenli bir şekilde analiz edebilme yeteneğidir. Dezavantajı ise, bazı karmaşık zararlı yazılımların gizli özelliklerinin ve davranışlarının sadece çalıştırıldığında ortaya çıkması nedeniyle bu özellikleri kaçırma riskidir.

• Dinamik Analiz: Dinamik analiz, zararlı yazılımın kontrollü bir ortamda (genellikle bir sanal makine içinde) çalıştırılmasını ve davranışlarının gözlemlenmesini içerir. Bu yöntem, zararlı yazılımın gerçekte ne yaptığını anlamak için kullanılır; ağ trafiği, dosya işlemleri ve sistem değişiklikleri gibi gerçek zamanlı etkilerini izler. Dinamik analizin avantajı, zararlı yazılımın aktif olarak neler yapabileceğini gözlemleyebilme yeteneğidir. Dezavantajı ise, bu analiz sırasında zararlı yazılımın bazı zararlı eylemleri gerçekleştirmesi ve bu sürecin daha riskli olmasıdır.

Her iki yöntemin de avantajları ve dezavantajları birbirine tamamlayıcı niteliktedir. Bu nedenle, kapsamlı bir zararlı yazılım analizi için genellikle her iki yöntemin birleştirilerek kullanılması önerilir. Bu, zararlı yazılımın daha derinlemesine anlaşılmasını ve etkili bir şekilde mücadele edilmesini sağlar.
```

#### 10. Dinamik Analiz Nedir?
```
Zararlı yazılımların sistem üzerindeki davranışlarını çalıştırarak inceleyen bir yaklaşım olan dinamik analiz anlatılmaktadır. Dinamik analizde, zararlı yazılımın sistemdeki etkilerini detaylı bir şekilde incelemek için kayıt defteri, dosya, ağ ve süreç olaylarını gözlemleyebilen uygulamalar kullanılır. Bu analiz sırasında özellikle dikkat edilmesi gereken bazı önemli olaylar şunlardır:

• Ağ Bağlantıları: Zararlı yazılımın ağ üzerinde kurduğu bağlantıları ve gerçekleştirdiği trafikleri incelemek, potansiyel zararlı aktiviteleri ve veri sızıntılarını tespit etmeye yardımcı olur.

• Dosya Olayları: Zararlı yazılımın oluşturduğu, değiştirdiği veya sildiği dosyaların izlenmesi, zararlı yazılımın ne tür etkiler bıraktığını anlamak için kritik öneme sahiptir.

• Süreç Olayları: Zararlı yazılımın sistemi nasıl etkilediği, hangi süreçleri başlattığı veya durdurduğu, bu olayların sistem üzerindeki genel etkileri analiz edilir.

• Kayıt Defteri Olayları: Zararlı yazılımın kayıt defterinde yaptığı değişiklikler, sistem konfigürasyonuna ve güvenlik ayarlarına potansiyel etkileri açısından incelenir.

Dinamik analiz, zararlı yazılımın gerçek zamanlı davranışlarını ve etkilerini anlamak için oldukça etkili bir yöntemdir. Bu yaklaşım, zararlı yazılımın potansiyel tehlikelerini ve sistem üzerindeki etkilerini detaylı bir şekilde ortaya çıkarmayı amaçlar.
```

#### 11. Statik Analiz ve Dinamik Analiz
```
Zararlı yazılım analizi yaparken hangi yaklaşımın kullanılacağının mevcut koşullara bağlı olduğunu vurgulamaktadır. Hızlı sonuçlar elde etmek istenildiğinde dinamik analiz tercih edilebilir, ancak zararlı yazılımın tam anlamıyla analiz edilmesi için hem statik hem de dinamik analizin birlikte kullanılması gerektiği belirtilmektedir.

Tek bir yaklaşımın zararlı yazılımı analiz etmek için yeterli olmayabileceği, her iki yaklaşımın birlikte kullanılmasının daha etkili sonuçlar doğuracağı üzerinde durulmuştur. Bu, statik ve dinamik analizlerin farklı koşullarda birbirine üstünlük sağladığı avantajlara dayanmaktadır.

Özellikle, bir Seviye 1-2 SOC analisti olarak çalışan biri, dinamik analizin yardımıyla hızlı bir şekilde C2 adresini (komuta ve kontrol sunucusu) tespit ederek harekete geçebilir. Dolayısıyla, her iki yaklaşımın da kendi avantajlarına göre farklı durumlar için uygulanabilir olduğu sonucuna varılır. Bu yaklaşımların birleştirilmesi, zararlı yazılımla mücadelede daha başarılı sonuçlar elde etmeye yol açar.

Zararlı yazılım analizi için kullanılan iki temel yöntem olan statik ve dinamik analizlerin özellikleri ve farkları ele alınmaktadır.

• . Statik Analiz:
  - Uzun zaman alır.
  - Zararlı yazılımın kapasitesini öğrenmek mümkündür.
  - Analiz sonucu detaylıdır.

• Dinamik Analiz:
  - Genellikle kısa sürede tamamlanır.
  - Yalnızca çalıştırıldığı sistem üzerindeki etkinlikler hakkında bilgi sağlar.
  - Analiz sonucu detaylı değildir.

Bu özet, her iki analiz yönteminin avantajlarını ve sınırlılıklarını vurgulamaktadır. Statik analiz, zararlı yazılımın daha derinlemesine incelenmesini sağlarken zaman alıcı olabilir; dinamik analiz ise daha hızlı sonuçlar verir ancak yalnızca zararlı yazılımın çalıştırıldığı sistemdeki etkilerini gözlemleyebilir ve daha az detaylı bilgi sunar. Bu nedenle, zararlı yazılım analizinde her iki yöntemin de uygun koşullara göre dengeli bir şekilde kullanılması önemlidir.
```

#### 12. AnyRun Kullanarak Dinamik Analiz
```
Zararlı yazılım analizinde hızlı ve etkili bir yöntem olarak sanal ortam hizmetleri ve ürünlerinden yararlanmanın önemi vurgulanmakta. Özellikle AnyRun isimli interaktif bir sanal ortamın (sandbox) zararlı yazılım analizi için nasıl kullanılabileceği ele alınıyor.

AnyRun, hızlı bir şekilde zararlı yazılım analizi yapmak isteyenler için kullanışlı bir araç olarak tanıtılıyor. Ücretsiz veya ücretli seçenekleri bulunan AnyRun'ın, ücretsiz kullanımında analizlerin herkes tarafından görülebilir olduğu, bu nedenle kişisel veri içeren dosyaların AnyRun'a yüklenmemesi gerektiği belirtiliyor. Ayrıca, ücretsiz planın kullanım süresi gibi bazı kısıtlamaları da bulunmakta.

AnyRun kullanarak zararlı yazılım analizi yapmanın ayrıntılarını ve bu yöntemle hangi tür çıktılar alınabileceğini incelemeyi öneriyor. Bu özet, AnyRun'ın zararlı yazılım analizi için nasıl bir araç olduğunu ve kullanımının potansiyel avantajlarını ve sınırlamalarını gösteriyor.

Güvenli bir inceleme ortamı kurduktan sonra güncelleme yapacağım.
```

#### 13. Kötü Amaçlı Yazılımları Daha Hızlı Analiz Etmek için araç listesi
```
Çeşitli siber güvenlik ve zararlı yazılım analizi araçları hakkında kısa açıklamalar bulunmaktadır:

• Anlyz: Siber güvenlik platformu, gerçek zamanlı tehdit tespiti ve analizi sağlar.
• Any.run: Interaktif çevrimiçi zararlı yazılım analiz hizmeti sunar.
• Comodo Valkyrie: Dosya analizi ve tehdit istihbaratı hizmetleri sağlayan bir sistemdir.
• Cuckoo: Açık kaynaklı otomatik zararlı yazılım analizi sistemi.
• Hybrid Analysis: Çeşitli analiz araçlarına sahip, kapsamlı bir zararlı yazılım analiz platformudur.
• Intezer Analyze: Genetik zararlı yazılım analizi yaparak, tehditleri tanımlar.
• SecondWrite Malware Deepview: Gelişmiş zararlı yazılım analizi ve tespiti yapar.
• Jevereg: Zararlı yazılım analizi için kullanılan bir araçtır.
• IObit Cloud: Bulut tabanlı güvenlik çözümleri sunar.
• BinaryGuard: Dinamik zararlı yazılım analizi sağlar.
• BitBlaze: Zararlı yazılım analizi için kullanılan bir dizi araç sunar.
• SandDroid: Android tabanlı zararlı yazılımları analiz eder.
• Joe Sandbox: Otomatik zararlı yazılım analizi ve raporlama sunar.
• AMAaaS: Zararlı yazılım analizi hizmeti sunan bir platform.
• IRIS-H: Siber güvenlik tehditlerini izleyen bir sistem.
• Gatewatcher Intelligence: Gelişmiş tehdit algılama ve analiz çözümleri sunar.
• Hatching Triage: Otomatik zararlı yazılım analizi için bir sandbox hizmetidir.
• InQuest Labs: Derinlemesine tehdit analizi ve araştırma sunar.
• Manalyzer: Dosya analizi için çevrimiçi bir araçtır.
• SandBlast Analysis: Check Point tarafından sunulan zararlı yazılım analiz hizmeti.
• SNDBOX: Otomatik zararlı yazılım analizi ve tehdit istihbaratı sağlar.
• firmware: Firmware analizi ve güvenlik değerlendirmesi için kullanılan araçlar.
• opswat: Bulut tabanlı tehdit algılama ve analiz hizmetleri.
• virusade: Zararlı yazılım analizi ve tehdit istihbaratı sağlayan bir platform.
• virustotal: Dosyaları ve URL'leri zararlı yazılım açısından tarayan popüler bir hizmet.
• malware config: Zararlı yazılım yapılandırmalarını analiz eden araçlar.
• malware hunter team: Zararlı yazılım araştırma ve analizi yapan bir ekip.
• virscan: Çevrimiçi zararlı yazılım tarama hizmeti.
• jotti: Çeşitli antivirüs motorları kullanarak dosya analizi yapan bir hizmet.

Bu araçlar, zararlı yazılım tespiti ve analizi, tehdit istihbaratı, sistem güvenliği değerlendirmesi ve daha pek çok alanda kullanılıyor. Her biri, siber güvenlik alanında önemli bir rol oynayarak farklı özellikler ve yetenekler sunuyor.
```

<hr/>

</br>


<h2> [Day-14] January 14, 2024 : Malware Analysis Course | [TR] </h2> 

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
• Preprocessor>>hello_world.c
• Compiler>>hello_world.i
• Assembler>>hello_world.s
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

• Statik Analiz: Bu yöntem, zararlı yazılımın çalıştırılmasına gerek kalmadan, kodunun incelenmesiyle gerçekleştirilir. Statik analiz, zararlı yazılımın yapısını, kullanılan kodları ve potansiyel davranışlarını anlamaya yardımcı olur. Bu yaklaşımın avantajı, zararlı yazılımı çalıştırmadan önce güvenli bir şekilde analiz edebilme yeteneğidir. Dezavantajı ise, bazı karmaşık zararlı yazılımların gizli özelliklerinin ve davranışlarının sadece çalıştırıldığında ortaya çıkması nedeniyle bu özellikleri kaçırma riskidir.

• Dinamik Analiz: Dinamik analiz, zararlı yazılımın kontrollü bir ortamda (genellikle bir sanal makine içinde) çalıştırılmasını ve davranışlarının gözlemlenmesini içerir. Bu yöntem, zararlı yazılımın gerçekte ne yaptığını anlamak için kullanılır; ağ trafiği, dosya işlemleri ve sistem değişiklikleri gibi gerçek zamanlı etkilerini izler. Dinamik analizin avantajı, zararlı yazılımın aktif olarak neler yapabileceğini gözlemleyebilme yeteneğidir. Dezavantajı ise, bu analiz sırasında zararlı yazılımın bazı zararlı eylemleri gerçekleştirmesi ve bu sürecin daha riskli olmasıdır.

Her iki yöntemin de avantajları ve dezavantajları birbirine tamamlayıcı niteliktedir. Bu nedenle, kapsamlı bir zararlı yazılım analizi için genellikle her iki yöntemin birleştirilerek kullanılması önerilir. Bu, zararlı yazılımın daha derinlemesine anlaşılmasını ve etkili bir şekilde mücadele edilmesini sağlar.
```

#### 10. Dinamik Analiz Nedir?
```
Zararlı yazılımların sistem üzerindeki davranışlarını çalıştırarak inceleyen bir yaklaşım olan dinamik analiz anlatılmaktadır. Dinamik analizde, zararlı yazılımın sistemdeki etkilerini detaylı bir şekilde incelemek için kayıt defteri, dosya, ağ ve süreç olaylarını gözlemleyebilen uygulamalar kullanılır. Bu analiz sırasında özellikle dikkat edilmesi gereken bazı önemli olaylar şunlardır:

• Ağ Bağlantıları: Zararlı yazılımın ağ üzerinde kurduğu bağlantıları ve gerçekleştirdiği trafikleri incelemek, potansiyel zararlı aktiviteleri ve veri sızıntılarını tespit etmeye yardımcı olur.

• Dosya Olayları: Zararlı yazılımın oluşturduğu, değiştirdiği veya sildiği dosyaların izlenmesi, zararlı yazılımın ne tür etkiler bıraktığını anlamak için kritik öneme sahiptir.

• Süreç Olayları: Zararlı yazılımın sistemi nasıl etkilediği, hangi süreçleri başlattığı veya durdurduğu, bu olayların sistem üzerindeki genel etkileri analiz edilir.

• Kayıt Defteri Olayları: Zararlı yazılımın kayıt defterinde yaptığı değişiklikler, sistem konfigürasyonuna ve güvenlik ayarlarına potansiyel etkileri açısından incelenir.

Dinamik analiz, zararlı yazılımın gerçek zamanlı davranışlarını ve etkilerini anlamak için oldukça etkili bir yöntemdir. Bu yaklaşım, zararlı yazılımın potansiyel tehlikelerini ve sistem üzerindeki etkilerini detaylı bir şekilde ortaya çıkarmayı amaçlar.
```

#### 11. Statik Analiz ve Dinamik Analiz
```
Zararlı yazılım analizi yaparken hangi yaklaşımın kullanılacağının mevcut koşullara bağlı olduğunu vurgulamaktadır. Hızlı sonuçlar elde etmek istenildiğinde dinamik analiz tercih edilebilir, ancak zararlı yazılımın tam anlamıyla analiz edilmesi için hem statik hem de dinamik analizin birlikte kullanılması gerektiği belirtilmektedir.

Tek bir yaklaşımın zararlı yazılımı analiz etmek için yeterli olmayabileceği, her iki yaklaşımın birlikte kullanılmasının daha etkili sonuçlar doğuracağı üzerinde durulmuştur. Bu, statik ve dinamik analizlerin farklı koşullarda birbirine üstünlük sağladığı avantajlara dayanmaktadır.

Özellikle, bir Seviye 1-2 SOC analisti olarak çalışan biri, dinamik analizin yardımıyla hızlı bir şekilde C2 adresini (komuta ve kontrol sunucusu) tespit ederek harekete geçebilir. Dolayısıyla, her iki yaklaşımın da kendi avantajlarına göre farklı durumlar için uygulanabilir olduğu sonucuna varılır. Bu yaklaşımların birleştirilmesi, zararlı yazılımla mücadelede daha başarılı sonuçlar elde etmeye yol açar.

Zararlı yazılım analizi için kullanılan iki temel yöntem olan statik ve dinamik analizlerin özellikleri ve farkları ele alınmaktadır.

• . Statik Analiz:
  - Uzun zaman alır.
  - Zararlı yazılımın kapasitesini öğrenmek mümkündür.
  - Analiz sonucu detaylıdır.

• Dinamik Analiz:
  - Genellikle kısa sürede tamamlanır.
  - Yalnızca çalıştırıldığı sistem üzerindeki etkinlikler hakkında bilgi sağlar.
  - Analiz sonucu detaylı değildir.

Bu özet, her iki analiz yönteminin avantajlarını ve sınırlılıklarını vurgulamaktadır. Statik analiz, zararlı yazılımın daha derinlemesine incelenmesini sağlarken zaman alıcı olabilir; dinamik analiz ise daha hızlı sonuçlar verir ancak yalnızca zararlı yazılımın çalıştırıldığı sistemdeki etkilerini gözlemleyebilir ve daha az detaylı bilgi sunar. Bu nedenle, zararlı yazılım analizinde her iki yöntemin de uygun koşullara göre dengeli bir şekilde kullanılması önemlidir.
```

#### 12. AnyRun Kullanarak Dinamik Analiz
```
Zararlı yazılım analizinde hızlı ve etkili bir yöntem olarak sanal ortam hizmetleri ve ürünlerinden yararlanmanın önemi vurgulanmakta. Özellikle AnyRun isimli interaktif bir sanal ortamın (sandbox) zararlı yazılım analizi için nasıl kullanılabileceği ele alınıyor.

AnyRun, hızlı bir şekilde zararlı yazılım analizi yapmak isteyenler için kullanışlı bir araç olarak tanıtılıyor. Ücretsiz veya ücretli seçenekleri bulunan AnyRun'ın, ücretsiz kullanımında analizlerin herkes tarafından görülebilir olduğu, bu nedenle kişisel veri içeren dosyaların AnyRun'a yüklenmemesi gerektiği belirtiliyor. Ayrıca, ücretsiz planın kullanım süresi gibi bazı kısıtlamaları da bulunmakta.

AnyRun kullanarak zararlı yazılım analizi yapmanın ayrıntılarını ve bu yöntemle hangi tür çıktılar alınabileceğini incelemeyi öneriyor. Bu özet, AnyRun'ın zararlı yazılım analizi için nasıl bir araç olduğunu ve kullanımının potansiyel avantajlarını ve sınırlamalarını gösteriyor.

Güvenli bir inceleme ortamı kurduktan sonra güncelleme yapacağım.
```

#### 13. Kötü Amaçlı Yazılımları Daha Hızlı Analiz Etmek için araç listesi
```
Çeşitli siber güvenlik ve zararlı yazılım analizi araçları hakkında kısa açıklamalar bulunmaktadır:

• Anlyz: Siber güvenlik platformu, gerçek zamanlı tehdit tespiti ve analizi sağlar.
• Any.run: Interaktif çevrimiçi zararlı yazılım analiz hizmeti sunar.
• Comodo Valkyrie: Dosya analizi ve tehdit istihbaratı hizmetleri sağlayan bir sistemdir.
• Cuckoo: Açık kaynaklı otomatik zararlı yazılım analizi sistemi.
• Hybrid Analysis: Çeşitli analiz araçlarına sahip, kapsamlı bir zararlı yazılım analiz platformudur.
• Intezer Analyze: Genetik zararlı yazılım analizi yaparak, tehditleri tanımlar.
• SecondWrite Malware Deepview: Gelişmiş zararlı yazılım analizi ve tespiti yapar.
• Jevereg: Zararlı yazılım analizi için kullanılan bir araçtır.
• IObit Cloud: Bulut tabanlı güvenlik çözümleri sunar.
• BinaryGuard: Dinamik zararlı yazılım analizi sağlar.
• BitBlaze: Zararlı yazılım analizi için kullanılan bir dizi araç sunar.
• SandDroid: Android tabanlı zararlı yazılımları analiz eder.
• Joe Sandbox: Otomatik zararlı yazılım analizi ve raporlama sunar.
• AMAaaS: Zararlı yazılım analizi hizmeti sunan bir platform.
• IRIS-H: Siber güvenlik tehditlerini izleyen bir sistem.
• Gatewatcher Intelligence: Gelişmiş tehdit algılama ve analiz çözümleri sunar.
• Hatching Triage: Otomatik zararlı yazılım analizi için bir sandbox hizmetidir.
• InQuest Labs: Derinlemesine tehdit analizi ve araştırma sunar.
• Manalyzer: Dosya analizi için çevrimiçi bir araçtır.
• SandBlast Analysis: Check Point tarafından sunulan zararlı yazılım analiz hizmeti.
• SNDBOX: Otomatik zararlı yazılım analizi ve tehdit istihbaratı sağlar.
• firmware: Firmware analizi ve güvenlik değerlendirmesi için kullanılan araçlar.
• opswat: Bulut tabanlı tehdit algılama ve analiz hizmetleri.
• virusade: Zararlı yazılım analizi ve tehdit istihbaratı sağlayan bir platform.
• virustotal: Dosyaları ve URL'leri zararlı yazılım açısından tarayan popüler bir hizmet.
• malware config: Zararlı yazılım yapılandırmalarını analiz eden araçlar.
• malware hunter team: Zararlı yazılım araştırma ve analizi yapan bir ekip.
• virscan: Çevrimiçi zararlı yazılım tarama hizmeti.
• jotti: Çeşitli antivirüs motorları kullanarak dosya analizi yapan bir hizmet.

Bu araçlar, zararlı yazılım tespiti ve analizi, tehdit istihbaratı, sistem güvenliği değerlendirmesi ve daha pek çok alanda kullanılıyor. Her biri, siber güvenlik alanında önemli bir rol oynayarak farklı özellikler ve yetenekler sunuyor.
```

<hr/>

</br>

<h2> [Day-14] January 14, 2024 : Malware Analysis Course | [TR] </h2> 

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

~# START
~# Preprocessor >> hello_world.c
~# Compiler     >> hello_world.i
~# Assembler    >> hello_world.s
~# END
~# Executable   >> hello_world.exe
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

• Statik Analiz: Bu yöntem, zararlı yazılımın çalıştırılmasına gerek kalmadan, kodunun incelenmesiyle gerçekleştirilir. Statik analiz, zararlı yazılımın yapısını, kullanılan kodları ve potansiyel davranışlarını anlamaya yardımcı olur. Bu yaklaşımın avantajı, zararlı yazılımı çalıştırmadan önce güvenli bir şekilde analiz edebilme yeteneğidir. Dezavantajı ise, bazı karmaşık zararlı yazılımların gizli özelliklerinin ve davranışlarının sadece çalıştırıldığında ortaya çıkması nedeniyle bu özellikleri kaçırma riskidir.

• Dinamik Analiz: Dinamik analiz, zararlı yazılımın kontrollü bir ortamda (genellikle bir sanal makine içinde) çalıştırılmasını ve davranışlarının gözlemlenmesini içerir. Bu yöntem, zararlı yazılımın gerçekte ne yaptığını anlamak için kullanılır; ağ trafiği, dosya işlemleri ve sistem değişiklikleri gibi gerçek zamanlı etkilerini izler. Dinamik analizin avantajı, zararlı yazılımın aktif olarak neler yapabileceğini gözlemleyebilme yeteneğidir. Dezavantajı ise, bu analiz sırasında zararlı yazılımın bazı zararlı eylemleri gerçekleştirmesi ve bu sürecin daha riskli olmasıdır.

Her iki yöntemin de avantajları ve dezavantajları birbirine tamamlayıcı niteliktedir. Bu nedenle, kapsamlı bir zararlı yazılım analizi için genellikle her iki yöntemin birleştirilerek kullanılması önerilir. Bu, zararlı yazılımın daha derinlemesine anlaşılmasını ve etkili bir şekilde mücadele edilmesini sağlar.
```

#### 10. Dinamik Analiz Nedir?
```
Zararlı yazılımların sistem üzerindeki davranışlarını çalıştırarak inceleyen bir yaklaşım olan dinamik analiz anlatılmaktadır. Dinamik analizde, zararlı yazılımın sistemdeki etkilerini detaylı bir şekilde incelemek için kayıt defteri, dosya, ağ ve süreç olaylarını gözlemleyebilen uygulamalar kullanılır. Bu analiz sırasında özellikle dikkat edilmesi gereken bazı önemli olaylar şunlardır:

• Ağ Bağlantıları: Zararlı yazılımın ağ üzerinde kurduğu bağlantıları ve gerçekleştirdiği trafikleri incelemek, potansiyel zararlı aktiviteleri ve veri sızıntılarını tespit etmeye yardımcı olur.
• Dosya Olayları: Zararlı yazılımın oluşturduğu, değiştirdiği veya sildiği dosyaların izlenmesi, zararlı yazılımın ne tür etkiler bıraktığını anlamak için kritik öneme sahiptir.
• Süreç Olayları: Zararlı yazılımın sistemi nasıl etkilediği, hangi süreçleri başlattığı veya durdurduğu, bu olayların sistem üzerindeki genel etkileri analiz edilir.
• Kayıt Defteri Olayları: Zararlı yazılımın kayıt defterinde yaptığı değişiklikler, sistem konfigürasyonuna ve güvenlik ayarlarına potansiyel etkileri açısından incelenir.

Dinamik analiz, zararlı yazılımın gerçek zamanlı davranışlarını ve etkilerini anlamak için oldukça etkili bir yöntemdir. Bu yaklaşım, zararlı yazılımın potansiyel tehlikelerini ve sistem üzerindeki etkilerini detaylı bir şekilde ortaya çıkarmayı amaçlar.
```

#### 11. Statik Analiz ve Dinamik Analiz
```
Zararlı yazılım analizi yaparken hangi yaklaşımın kullanılacağının mevcut koşullara bağlı olduğunu vurgulamaktadır. Hızlı sonuçlar elde etmek istenildiğinde dinamik analiz tercih edilebilir, ancak zararlı yazılımın tam anlamıyla analiz edilmesi için hem statik hem de dinamik analizin birlikte kullanılması gerektiği belirtilmektedir.

Tek bir yaklaşımın zararlı yazılımı analiz etmek için yeterli olmayabileceği, her iki yaklaşımın birlikte kullanılmasının daha etkili sonuçlar doğuracağı üzerinde durulmuştur. Bu, statik ve dinamik analizlerin farklı koşullarda birbirine üstünlük sağladığı avantajlara dayanmaktadır.

Özellikle, bir Seviye 1-2 SOC analisti olarak çalışan biri, dinamik analizin yardımıyla hızlı bir şekilde C2 adresini (komuta ve kontrol sunucusu) tespit ederek harekete geçebilir. Dolayısıyla, her iki yaklaşımın da kendi avantajlarına göre farklı durumlar için uygulanabilir olduğu sonucuna varılır. Bu yaklaşımların birleştirilmesi, zararlı yazılımla mücadelede daha başarılı sonuçlar elde etmeye yol açar.

Zararlı yazılım analizi için kullanılan iki temel yöntem olan statik ve dinamik analizlerin özellikleri ve farkları ele alınmaktadır.

• . Statik Analiz:
  - Uzun zaman alır.
  - Zararlı yazılımın kapasitesini öğrenmek mümkündür.
  - Analiz sonucu detaylıdır.

• Dinamik Analiz:
  - Genellikle kısa sürede tamamlanır.
  - Yalnızca çalıştırıldığı sistem üzerindeki etkinlikler hakkında bilgi sağlar.
  - Analiz sonucu detaylı değildir.

Bu özet, her iki analiz yönteminin avantajlarını ve sınırlılıklarını vurgulamaktadır. Statik analiz, zararlı yazılımın daha derinlemesine incelenmesini sağlarken zaman alıcı olabilir; dinamik analiz ise daha hızlı sonuçlar verir ancak yalnızca zararlı yazılımın çalıştırıldığı sistemdeki etkilerini gözlemleyebilir ve daha az detaylı bilgi sunar. Bu nedenle, zararlı yazılım analizinde her iki yöntemin de uygun koşullara göre dengeli bir şekilde kullanılması önemlidir.
```

#### 12. AnyRun Kullanarak Dinamik Analiz
```
Zararlı yazılım analizinde hızlı ve etkili bir yöntem olarak sanal ortam hizmetleri ve ürünlerinden yararlanmanın önemi vurgulanmakta. Özellikle AnyRun isimli interaktif bir sanal ortamın (sandbox) zararlı yazılım analizi için nasıl kullanılabileceği ele alınıyor.

AnyRun, hızlı bir şekilde zararlı yazılım analizi yapmak isteyenler için kullanışlı bir araç olarak tanıtılıyor. Ücretsiz veya ücretli seçenekleri bulunan AnyRun'ın, ücretsiz kullanımında analizlerin herkes tarafından görülebilir olduğu, bu nedenle kişisel veri içeren dosyaların AnyRun'a yüklenmemesi gerektiği belirtiliyor. Ayrıca, ücretsiz planın kullanım süresi gibi bazı kısıtlamaları da bulunmakta.

AnyRun kullanarak zararlı yazılım analizi yapmanın ayrıntılarını ve bu yöntemle hangi tür çıktılar alınabileceğini incelemeyi öneriyor. Bu özet, AnyRun'ın zararlı yazılım analizi için nasıl bir araç olduğunu ve kullanımının potansiyel avantajlarını ve sınırlamalarını gösteriyor.

Güvenli bir inceleme ortamı kurduktan sonra güncelleme yapacağım.
```

#### 13. Kötü Amaçlı Yazılımları Daha Hızlı Analiz Etmek için araç listesi
```
Kötü amaçlı yazılım tespiti, tehdit istihbaratı, sistem güvenliği değerlendirmesi ve diğer birçok alanda çeşitli siber güvenlik ve kötü amaçlı yazılım analiz araçları kullanılmaktadır. Her araç, benzersiz özellikler ve yetenekler sunarak siber güvenlikte önemli bir rol oynar.

• Anlyz: Siber güvenlik platformu, gerçek zamanlı tehdit tespiti ve analizi sağlar.
• Any.run: Interaktif çevrimiçi zararlı yazılım analiz hizmeti sunar.
• Comodo Valkyrie: Dosya analizi ve tehdit istihbaratı hizmetleri sağlayan bir sistemdir.
• Cuckoo: Açık kaynaklı otomatik zararlı yazılım analizi sistemi.
• Hybrid Analysis: Çeşitli analiz araçlarına sahip, kapsamlı bir zararlı yazılım analiz platformudur.
• Intezer Analyze: Genetik zararlı yazılım analizi yaparak, tehditleri tanımlar.
• SecondWrite Malware Deepview: Gelişmiş zararlı yazılım analizi ve tespiti yapar.
• Jevereg: Zararlı yazılım analizi için kullanılan bir araçtır.
• IObit Cloud: Bulut tabanlı güvenlik çözümleri sunar.
• BinaryGuard: Dinamik zararlı yazılım analizi sağlar.
• BitBlaze: Zararlı yazılım analizi için kullanılan bir dizi araç sunar.
• SandDroid: Android tabanlı zararlı yazılımları analiz eder.
• Joe Sandbox: Otomatik zararlı yazılım analizi ve raporlama sunar.
• AMAaaS: Zararlı yazılım analizi hizmeti sunan bir platform.
• IRIS-H: Siber güvenlik tehditlerini izleyen bir sistem.
• Gatewatcher Intelligence: Gelişmiş tehdit algılama ve analiz çözümleri sunar.
• Hatching Triage: Otomatik zararlı yazılım analizi için bir sandbox hizmetidir.
• InQuest Labs: Derinlemesine tehdit analizi ve araştırma sunar.
• Manalyzer: Dosya analizi için çevrimiçi bir araçtır.
• SandBlast Analysis: Check Point tarafından sunulan zararlı yazılım analiz hizmeti.
• SNDBOX: Otomatik zararlı yazılım analizi ve tehdit istihbaratı sağlar.
• firmware: Firmware analizi ve güvenlik değerlendirmesi için kullanılan araçlar.
• opswat: Bulut tabanlı tehdit algılama ve analiz hizmetleri.
• virusade: Zararlı yazılım analizi ve tehdit istihbaratı sağlayan bir platform.
• virustotal: Dosyaları ve URL'leri zararlı yazılım açısından tarayan popüler bir hizmet.
• malware config: Zararlı yazılım yapılandırmalarını analiz eden araçlar.
• malware hunter team: Zararlı yazılım araştırma ve analizi yapan bir ekip.
• virscan: Çevrimiçi zararlı yazılım tarama hizmeti.
• jotti: Çeşitli antivirüs motorları kullanarak dosya analizi yapan bir hizmet.
```

<hr/>

</br>


<h2> [Day-14] January 14, 2024 : Malware Analysis Course | [EN] </h2> 

#### 1. How does Malware Analysis help SOC Analysts?
```
Malware Analysis (Malicious Software Analysis) is a crucial skill for SOC (Security Operations Center) analysts. The existence and effects of complex malware like Stuxnet highlight the critical nature of knowledge and skills in this area for security analysts. In their routine, analysts often encounter suspicious files or processes. Given that most cyber attacks involve malware, it's understandable that having this knowledge is essential. As a Security Analyst, one must be able to analyze whether these files are malicious; if they are, it's important to understand the purpose of this software and how it communicates with command and control servers. Malware analysis is an indispensable skill for Security Analysts. There are many methods and techniques for analyzing suspicious files, and this training series allows you to analyze malware using the most suitable techniques for your needs.
```

#### 2. Malware Definition and Types of Malware
```
Malware, derived from "MALicious softWARE," refers to software designed to harm system security and integrity. Modern cyber threat actors use malware for various purposes like ensuring persistence, causing system damage, or demanding ransom. As a SOC analyst, it's crucial to analyze suspicious software and determine its maliciousness. Knowledge of programming languages aids in malware analysis, although not all are required. With cyber threats evolving, analysts constantly need to update their skills to tackle increasingly complex malware. SOC analysts frequently encounter suspicious files in daily routines, coming via email, detected by antivirus software, or identified by network security products. Analysis helps in determining the nature of these files, their objectives, command and control servers, and malware types.
```

#### 3. Malware Types
``` 
Malware, or "MALicious softWARE," encompasses various software types designed with malicious intent, jeopardizing system security and integrity. Cyber threat actors use malware for objectives like maintaining persistence, damaging systems, or making ransom demands. As a SOC analyst, identifying the type of malware is crucial, as it informs about its potential impact and the threat it poses.

For instance, identifying a piece of software as a keylogger immediately informs others that it records keystrokes. This initial identification can guide decisions for upper management or help understand the attacker's target, followed by a detailed analysis report.

Malware types include:

- Backdoor: Allows attackers access through a hidden backdoor.
- Adware: Delivers unwanted ads, sometimes changing default search engines.
- Ransomware: Encrypts files, demanding ransom for access.
- Virus: Self-replicating malware that spreads to other files.
- Worm: Self-replicating malware spreading across networks.
- Rootkit: Hides its presence while maintaining privileged access.
- Remote Access Trojan (RAT): Provides threat actors full control over the device.
- Banking Malware: Targets banking applications to steal money.
- Keylogger: Records keystrokes and sends them to attackers.

Malware can exhibit multiple characteristics, fitting into more than one category. For example, WannaCry combines worm and ransomware traits.
```

#### 4. What Does a Malware Analyst Need to Know?
```
Malware analysis might appear straightforward from the outside, but it's actually a complex field requiring expertise in various aspects. Although it's a distinct area, some Tier 3 SOC Analysts (Subject Matter Experts) dedicate their careers solely to malware analysis. Despite being a separate field, security analysts frequently utilize it in their daily routines. Successfully analyzing malware requires foundational knowledge in many areas.
```

#### 5. Operating System Fundamentals and Architecture
```
Malware operates within operating systems, so malware analysts must have a solid understanding and knowledge of these systems. Malware typically leverages features offered by the operating system to elevate privileges, conduct reconnaissance, and ensure persistence. For example, in Windows operating systems, malware may use features like Task Scheduler, Services, and Registry to maintain persistence. Besides the operating system features, knowledge of APIs, System Calls (Syscalls), Memory Architecture, and other lower-level topics is vital for effective malware analysis. More focus on these subjects will be provided in the "Static Malware Analysis" training.
```

#### 6. Assembly Language and Programming
```
Have you ever wondered what happens when you compile programming languages while developing software? Or how processors run these various languages? Processors understand only 0s and 1s; anything else is meaningless to them. When you compile a program in languages like C/C++, Python, Java, Ruby, Go, compilers translate your code into 0s and 1s that the processor can understand. When a program is launched, these 0s and 1s are sent from memory to the processor to be executed. The lowest-level programming language you can see, apart from 0s and 1s, is Assembly, where each instruction directly corresponds to 0s and 1s. A program written in C is first translated to Assembly, then to 0s and 1s. Compiled malware can be easily converted to Assembly, but translating it further is not as easy or precise, so analyses are often done in Assembly. Software that translates machine code into Assembly is called a "Disassembler." In static code analysis training, we will also focus on the basics of "Assembly" Language.

~# START
~# Preprocessor >> hello_world.c
~# Compiler     >> hello_world.i
~# Assembler    >> hello_world.s
~# END
~# Executable   >> hello_world.exe
```

#### 7. Network Protocols and Fundamentals
```
Malware often exhibits network activity for purposes like data exfiltration, connecting to command and control servers, or downloading secondary payloads. Understanding this network traffic during malware analysis is crucial to grasp the malware's intent. Therefore, it's essential for malware analysts to have fundamental knowledge of networking.
```

#### 8. Cryptography
```
While many technologies use cryptography for security, attackers also utilize it to make detection difficult and block access. Modern ransomware, for example, employs cryptography to encrypt files, preventing access to them until a ransom is paid. During malware analysis, encountering cryptography is a common occurrence.
```

#### 9. Which Approach to Choose When Analyzing Malware?
```
In cybersecurity defense, malware analysis is a common task, involving two main approaches: Static and Dynamic Analysis.

• Static Analysis: This method involves examining the code of malware without running it. It helps understand the structure, code used, and potential behaviors of malware. The advantage is safe analysis without execution. However, it might miss some complex characteristics only visible when run.

• Dynamic Analysis: Involves running malware in a controlled environment (like a virtual machine) and observing its behavior. It's used to understand what the malware actually does, tracking real-time effects such as network traffic, file operations, and system changes. The advantage is observing active capabilities of the malware. However, it's riskier as it involves running the malware.

Both methods complement each other's advantages and disadvantages. Therefore, combining both is often recommended for comprehensive malware analysis, enabling a deeper understanding and effective response.
```

#### 10. What is Dynamic Analysis?
```
Dynamic analysis, an approach to studying malware behavior on a system by running it, involves using applications that can observe registry, file, network, and process events to examine the impact of malware on the system. Important aspects to focus on during this analysis include:

- Network Connections: Inspecting the connections and traffic generated by malware helps in identifying potentially harmful activities and data leaks.
- File Events: Monitoring the files created, altered, or deleted by malware is critical for understanding its impact.
- Process Events: Analyzing how malware affects the system, which processes it starts or stops, and the overall impact of these events.
- Registry Events: Investigating changes made by malware to the registry, assessing potential effects on system configuration and security settings.

Dynamic analysis is an effective method for understanding the real-time behaviors and effects of malware, aiming to reveal in detail the potential dangers and impacts on the system.
```
Static Analysis and Dynamic Analysis
#### 11. Statik Analiz ve Dinamik Analiz
```
The choice of approach in malware analysis depends on current conditions. Dynamic analysis is preferred for quick results, but a comprehensive analysis requires both static and dynamic methods. Relying on a single approach might not be sufficient; using both can yield more effective outcomes due to their respective advantages in different situations. For instance, a Level 1-2 SOC analyst might quickly identify the C2 (command and control) server address using dynamic analysis. Thus, each approach is applicable in different scenarios, and their combination leads to more successful outcomes in combating malware. This discussion highlights the characteristics and differences between the two main methods used in malware analysis: static and dynamic analysis.

• Static Analysis:
  - Takes a long time.
  - Enables understanding of malware capacity.
  - Detailed analysis results.

• Dynamic Analysis:
  - Usually completed quickly.
  - Provides information only about activities on the system where it's run.
  - Analysis results are not detailed.

This summary highlights the advantages and limitations of both methods. Static analysis allows in-depth examination but is time-consuming; dynamic analysis offers quicker results but only observes effects on the system where the malware is executed, providing less detail. Thus, using both methods in a balanced way depending on the situation is important for malware analysis.
```

#### 12. Dynamic Analysis Using AnyRun
```
The significance of utilizing virtual environment services and products, such as AnyRun, for quick and effective malware analysis is emphasized. AnyRun, an interactive sandbox, is introduced as a useful tool for those seeking rapid malware analysis. It offers both free and paid options. In its free usage, analyses are visible to all, so it's advised not to upload files containing personal data. The free plan also has certain limitations like usage duration. The summary suggests exploring how to use AnyRun for malware analysis and what types of outputs can be obtained, highlighting AnyRun's potential advantages and limitations in malware analysis.

I will update once I have established a safe review environment.
```

#### 13. List of tools to Analyze Malware Faster
```
Various cybersecurity and malware analysis tools are used for malware detection, threat intelligence, system security assessment, and many other areas. Each tool plays a significant role in cybersecurity, offering unique features and capabilities.

• Anlyz: A cybersecurity platform providing real-time threat detection and analysis.
• Any.run: Offers interactive online malware analysis services.
• Comodo Valkyrie: A system that provides file analysis and threat intelligence services.
• Cuckoo: An open-source automated malware analysis system.
• Hybrid Analysis: A comprehensive malware analysis platform with a variety of analysis tools.
• Intezer Analyze: Identifies threats through genetic malware analysis.
• SecondWrite Malware Deepview: Conducts advanced malware analysis and detection.
• Jevereg: A tool used for malware analysis.
• IObit Cloud: Provides cloud-based security solutions.
• BinaryGuard: Offers dynamic malware analysis.
• BitBlaze: A suite of tools for malware analysis.
• SandDroid: Analyzes Android-based malware.
• Joe Sandbox: Provides automated malware analysis and reporting.
• AMAaaS: A platform offering malware analysis services.
• IRIS-H: Monitors cybersecurity threats.
• Gatewatcher Intelligence: Offers advanced threat detection and analysis solutions.
• Hatching Triage: A sandbox service for automated malware analysis.
• InQuest Labs: Provides in-depth threat analysis and research.
• Manalyzer: An online tool for file analysis.
• SandBlast Analysis: A malware analysis service offered by Check Point.
• SNDBOX: Provides automated malware analysis and threat intelligence.
• firmware: Tools used for firmware analysis and security assessment.
• opswat: Cloud-based threat detection and analysis services.
• virusade: A platform providing malware analysis and threat intelligence.
• virustotal: A popular service scanning files and URLs for malware.
• malware config: Tools analyzing malware configurations.
• malware hunter team: A team conducting malware research and analysis.
• virscan: An online malware scanning service.
• jotti: A service analyzing files using various antivirus engines.
```

<hr/>

</br>