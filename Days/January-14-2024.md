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