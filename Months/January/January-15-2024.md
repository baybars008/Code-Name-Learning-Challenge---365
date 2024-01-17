<h2> [Day-15] January 15, 2024 : Hands-on Linux for DevOps & Cloud Engineers | [TR] </h2> 

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
```
![image](/Months/January/January-Images/January.png)
```
• OS-Level Virtualization (İşletim Sistemi Düzeyinde Sanallaştırma)
• namespaces (isim Alanları)
• C groups (C grupları)
• Container Orchestration (Konteyner Orkestrasyonu)
```
![image](/Months/January/January-Images/January-1.png)
```
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

#### 12. Learning Bash Fundamentals - Echo
```
#!/bin/bash
#
# This is a comment
#
echo "Hello everyone"
exit 1
echo "This will not be printed"
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını belirtir. Bu satıra "shebang" denir ve script dosyasının başında yer alır.

`# This is a comment`: Bu satır bir yorum satırıdır. Bash, `#` işareti ile başlayan satırları yorum olarak kabul eder ve bunları yürütmez. Yorum satırları, kodun okunabilirliğini artırmak ve açıklama eklemek için kullanılır.

`echo "Hello everyone"`: Bu satır, ekrana "Hello everyone" metnini yazdırır. `echo` komutu, kendisinden sonraki metni standart çıkışa (genellikle terminal ekranına) yazdırır.

`exit 1`: Bu komut, scriptin çalışmasını sonlandırır ve işletim sistemine `1` değerini dönüş kodu olarak verir. Dönüş kodları, bir scriptin başarıyla mı yoksa bir hata ile mi sonlandığını belirtmek için kullanılır. `0` genellikle başarıyı, diğer değerler ise çeşitli hata durumlarını temsil eder.

`echo "This will not be printed"`: Bu satır aslında ekrana "This will not be printed" metnini yazdırmak için kullanılır. Ancak, bu satırın üstündeki `exit 1` komutu nedeniyle bu satır asla çalıştırılmaz. `exit` komutu scriptin o noktada sonlanmasına sebep olduğu için, bundan sonraki komutlar yürütülmez.

Bu script, çalıştırıldığında sadece "Hello everyone" metnini yazdırır ve ardından hata kodu `1` ile sonlanır. "This will not be printed" metni asla yazdırılmaz.
```

#### 13. Learning Bash Fundamentals - GPU
```
#!/bin/bash
#
cpus=1
memory=1024
username="ec2-user"
echo "This host has ${cpus} CPU and ${memory} KB of memory"
echo "The active user is ${username}"
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`cpus=1`: Bu satırda `cpus` adında bir değişken oluşturulur ve bu değişkene `1` değeri atanır. Bu değişken, CPU sayısını temsil eder.

`memory=1024`: Bu satırda `memory` adında bir değişken oluşturulur ve bu değişkene `1024` değeri atanır. Bu değişken, bellek miktarını kilobayt cinsinden temsil eder.

`username="ec2-user"`: Bu satırda `username` adında bir değişken oluşturulur ve bu değişkene `"ec2-user"` değeri atanır. Bu değişken, kullanıcı adını temsil eder.

`echo "This host has ${cpus} CPU and ${memory} KB of memory"`: Bu satır, ekrana değişkenlerin değerlerini içeren bir mesaj yazdırır. `${cpus}` ve `${memory}` ifadeleri, `cpus` ve `memory` değişkenlerinin değerlerini temsil eder. Sonuç olarak bu satır, ekrana "This host has 1 CPU and 1024 KB of memory" yazdırır.

`echo "The active user is ${username}"`: Bu satır da benzer şekilde, `username` değişkeninin değerini içeren bir mesajı ekrana yazdırır. Sonuç olarak, "The active user is ec2-user" yazdırılır.

Bu script, çalıştırıldığında öncelikle bazı değişkenlere değerler atar ve sonra bu değerleri içeren mesajları ekrana yazdırır. Scriptin amacı, belirli sistem bilgilerini ve aktif kullanıcı adını göstermektir.
```

#### 14. Learning Bash Fundamentals - Arrays
```
#!/bin/bash
#
declare -a distros
distros[0]="Amazon Linux"
distros[1]="Ubuntu"
distros[2]="RedHat"
distros[3]="Debian"
distros[5]="Arch"

echo "${distros[@]}"
unset distros[3]
echo "-------------------"
echo "${distros[@]}"


declare -A commands
commands["ls"]="/bin"
commands["cat"]="/bin"

echo "The cat command is locaed in the ${commands[cat]} directory"
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`declare -a distros`: Bu satır, `distros` adında bir dizin (array) tanımlar. `-a` seçeneği, bu değişkenin bir dizin olduğunu belirtir.

`distros[0]="Amazon Linux"` vb.: Bu satırlar, `distros` dizinine sırasıyla "Amazon Linux", "Ubuntu", "RedHat", "Debian" ve "Arch" değerlerini atar. Dizinin sıfırdan başlayarak indislenmesine dikkat edin.

9. `echo "${distros[@]}"`: Bu satır, `distros` dizisinin tüm elemanlarını ekrana yazdırır. `[@]` işaretçisi, dizinin tüm elemanlarını temsil eder.

10. `unset distros[3]`: Bu satır `distros` dizisinin 3. indisindeki (Debian'ı temsil eden) elemanını kaldırır.

11. `echo "-------------------"`: Bu satır sadece görsel bir ayırıcı olan çizgiyi ekrana yazdırır.

12. `echo "${distros[@]}"`: Bu satır, `distros` dizisinin güncellenmiş halini (Debian olmadan) ekrana yazdırır.

13. `declare -A commands`: Bu satır, `commands` adında bir ilişkisel dizi (associative array) tanımlar. `-A` seçeneği, bu değişkenin bir ilişkisel dizi olduğunu belirtir.

14-15. `commands["ls"]="/bin"` vb.: Bu satırlar, `commands` ilişkisel dizisine komutların hangi dizinde bulunduğunu atar. Örneğin, `ls` komutunun `/bin` dizininde olduğunu belirtir.

16. `echo "The cat command is located in the ${commands[cat]} directory"`: Bu satır, `commands` ilişkisel dizisindeki "cat" komutunun konumunu ekrana yazdırır. Bu durumda "/bin" dizini yazdırılır.

Bu script, normal diziler ve ilişkisel diziler ile çalışmayı gösteren bir örnektir. İlk bölümde bir dizi tanımlanır, elemanlar atanır, bir eleman çıkarılır ve dizinin içeriği yazdırılır. İkinci bölümde ise bir ilişkisel dizi kullanılarak komutların hangi dizinde bulunduğu bilgisi saklanır ve bu bilgi ekrana yazdırılır.
```

#### 15. Learning Bash Fundamentals - if
```
#!/bin/bash
#
cpu=6

# single branch
if [ $cpu -gt 4 ]
then
	echo "Suitable for virtualization"
fi

echo
# else
if [ $cpu -gt 4 ]
then
	echo "Suitable for virtualization"
else
	echo "Your milage may vary when using virtual machines"
fi

# built in test if file exists
if [ -f /usr/local/engineering/akira ]
then
	echo "file exists"
else
	echo "the file does not exist"
fi
```
```
 `#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

Boş Satır: Bu boş satır okunabilirliği artırmak için kullanılır. Kod üzerinde hiçbir etkisi yoktur.

`cpu=6`: Bu satırda `cpu` adında bir değişken oluşturulur ve bu değişkene `6` değeri atanır. Bu değişken, CPU sayısını temsil ediyor gibi görünüyor.

Yorum Satırı (`# single branch`): Bu satır bir yorum satırıdır ve scriptin işleyişi üzerinde bir etkisi yoktur. Bu yorum, aşağıdaki `if` blokunun tek bir şube (branch) olduğunu belirtiyor.

İlk `if` Bloğu:
   - `if [ $cpu -gt 4 ]`: Bu ifade, `cpu` değişkeninin değerinin 4'ten büyük olup olmadığını kontrol eder. `-gt` "greater than" (daha büyük) anlamına gelir.
   - `then`: Eğer koşul doğruysa (cpu 4'ten büyükse), `then` ile başlayan blok çalıştırılır.
   - `echo "Suitable for virtualization"`: Eğer koşul doğruysa, bu mesaj ekrana yazdırılır.
   - `fi`: `if` blokunun sonunu belirtir.

Yorum Satırı (`# else`): Bu yorum, aşağıdaki `if` blokunun bir "else" şubesine sahip olduğunu belirtir.

İkinci `if` Bloğu:
   - Aynı koşulu kontrol eder (`if [ $cpu -gt 4 ]`).
   - Eğer koşul doğruysa (`then`), "Suitable for virtualization" mesajını yazdırır.
   - Eğer koşul yanlışsa (`else`), "Your mileage may vary when using virtual machines" mesajını yazdırır.
   - `fi`: `if` blokunun sonunu belirtir.


Yorum Satırı (`# built in test if file exists`): Bu yorum, aşağıdaki `if` blokunun bir dosyanın varlığını kontrol etmek için kullanıldığını belirtir.

Üçüncü `if` Bloğu:
   - `if [ -f /usr/local/engineering/akira ]`: Bu ifade, `/usr/local/engineering/akira` yoluyla belirtilen dosyanın var olup olmadığını kontrol eder. `-f` parametresi, belirtilen yolun bir dosya olup olmadığını test eder.
   - `then`: Eğer dosya varsa, `then` ile başlayan blok çalıştırılır.
   - `echo "file exists"`: Eğer dosya varsa, bu mesaj ekrana yazdırılır.
   - `else`: Eğer dosya yoksa, `else` ile başlayan blok çalıştırılır.
   - `echo "the file does not exist"`: Eğer dosya yoksa, bu mesaj ekrana yazdırılır.
   - `fi`: `if` blokunun sonunu belirtir.

Bu script, CPU sayısına göre belirli koşulları kontrol ederek farklı mesajlar yazdırır, ve ayrıca belirli bir dosyanın varlığını kontrol eder. Bu tür kontroller, scriptlerde yaygın olarak kullanılan yapısal öğelerdir ve sistem durumlarına veya dosya varlıklarına göre kararlar almak için kullanılırlar.
```

#### 16. Learning Bash Fundamentals - loops
```
#!/bin/bash
#
declare -a distros
distros[0]="Amazon Linux"
distros[1]="Ubuntu"
distros[2]="RedHat"
distros[3]="Debian"
distros[5]="Arch"


# print out each distro
for distro in "${distros[@]}"
do
	echo $distro
done

echo "----------------"

# print out each distro until you hit RedHat then stop
for distro in "${distros[@]}"
do
	if [ "$distro" = "RedHat" ]
	then
		break
	fi
	echo $distro
done

# while loop
echo "Count up"
count=0
while [ $count -lt 10 ]
do
	echo "$count"
	((count++))
done

echo "Count down"
# count backwards
count=10
while [ $count -gt 0 ]
do
	echo "$count"
	((count--))
	sleep 0.2
done

echo "blast off!"
```
```
 `#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`declare -a distros`: Bu satır, `distros` adında bir dizi (array) tanımlar. `-a` seçeneği, bu değişkenin bir dizin olduğunu belirtir.

`distros[0]="Amazon Linux"` vb.: Bu satırlar, `distros` dizisine sırasıyla "Amazon Linux", "Ubuntu", "RedHat", "Debian" ve "Arch" değerlerini atar. Dizinin sıfırdan başlayarak indislenmesine dikkat edin. İlginç olarak, `distros[4]` ataması yapılmamış ve bu indis atlanmış, doğrudan `distros[5]` ile "Arch" atanmış.

İlk `for` Döngüsü:
   - `for distro in "${distros[@]}"`: Bu satır, `distros` dizisinin tüm elemanları üzerinde döngü başlatır. `[@]` işaretçisi, dizinin tüm elemanlarını temsil eder.
   - `do`: Döngü içinde yapılacak işlemleri başlatır.
   - `echo $distro`: Her döngüde, `distro` değişkeninin değerini (dizinin o anki elemanını) ekrana yazdırır.
   - `done`: Döngünün sonunu belirtir.

`echo "----------------"`: Bu satır ekrana çizgi yazdırır, genellikle görsel bir ayırıcı olarak kullanılır.

İkinci `for` Döngüsü:
   - Aynı şekilde `distros` dizisi üzerinde döngü başlatır.
   - `if [ "$distro" = "RedHat" ]`: Eğer `distro` değişkeni "RedHat" ise,
   - `then`: Koşul doğruysa,
   - `break`: Döngüyü kır ve döngüden çık.
   - `fi`: `if` blokunun sonunu belirtir.
   - Eğer `distro` "RedHat" değilse, o elemanı ekrana yazdırır.
   - "RedHat" elemanına ulaştığında döngüden çıkar.

`echo "Count up"` ve Boş Satır: "Count up" mesajını ekrana yazdırır ve boş bir satır bırakır.

İlk `while` Döngüsü:
   - `count=0`: `count` adında bir değişken oluşturur ve `0` değerini atar.
   - `while [ $count -lt 10 ]`: `count` değişkeninin değeri 10'dan küçük olduğu sürece döngüyü çalıştırır. `-lt` "less than" (daha küçük) anlamına gelir.
   - `do`: Döngü içinde yapılacak işlemleri başlatır.
   - `echo "$count"`: Her döngüde, `count` değişkeninin değerini ekrana yazdırır.
   - `((count++))`: Her döngüde, `count` değişkenini 1 arttırır.
   - `done`: Döngünün sonunu belirtir.

`echo "Count down"`: "Count down" mesajını ekrana yazdırır.

İkinci `while` Döngüsü:
   - `count=10`: `count` değişkenine `10` değeri atanır.
   - `while [ $count -gt 0 ]`: `count` değişkeninin değeri 0'dan büyük olduğu sürece döngüyü çalıştırır. `-gt` "greater than" (daha büyük) anlamına gelir.
   - `do`: Döngü içinde yapılacak işlemleri başlatır.
   - `echo "$count"`: Her döngüde, `count` değişkeninin değerini ekrana yazdırır.
   - `((count--))`: Her döngüde, `count` değişkenini 1 azaltır.
   - `sleep 0.2`: Her döngüde, 0.2 saniye bekler. Bu, döngünün hızını yavaşlatır.
   - `done`: Döngünün sonunu belirtir.

`echo "blast off!"`: "blast off!" mesajını ekrana yazdırır.

Bu script, bir dizi üzerinde farklı `for` döngüleri kullanarak elemanları yazdırır, belirli bir koşul karşılandığında döngüden çıkma örneği sunar ve `while` döngüsü kullanarak sayım yapar. Bu script, döngü yapılarını ve koşul kontrollerini gösteren pratik bir örnektir.
```

#### 17. Learning Bash Fundamentals - switch
```
#!/bin/bash
#
echo "Enter a persons name?"
read user

case $user in
	akira)
		echo "I do not know them well"
		;;
	leilani)
		echo "We go way back"
		;;
	*)
		echo "I have no idea who ${user} is"
		;;
esac
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`echo "Enter a persons name?"`: Bu satır, kullanıcıya bir soru sorar: "Enter a persons name?". Bu metin, kullanıcıya görüntülenir.

`read user`: Bu satır, kullanıcıdan girdi bekler ve bu girdiyi `user` adlı değişkene atar. Kullanıcının girdiği değer `user` değişkeninde saklanır.

`case $user in`: Bu satır, `user` değişkeninin değerine göre farklı senaryoları işleyecek bir `case` yapısı başlatır. Bu yapı, birden çok olasılığı kontrol etmek için kullanılır.

`akira)` bloğu:
   - `akira)`: Eğer `user` değişkeninin değeri "akira" ise, bu blok çalıştırılır.
   - `echo "I do not know them well"`: Belirtilen metin ekrana yazdırılır.
   - `;;`: Bu işaret, `case` yapısındaki bu özel durumun sonunu belirtir.

`leilani)` bloğu:
   - `leilani)`: Eğer `user` değişkeninin değeri "leilani" ise, bu blok çalıştırılır.
   - `echo "We go way back"`: Belirtilen metin ekrana yazdırılır.
   - `;;`: Bu durumun sonunu belirtir.

`*)` joker bloğu:
   - `*)`: Eğer `user` değişkeninin değeri yukarıdakilerden hiçbiri değilse (yani herhangi başka bir değerse), bu blok çalıştırılır.
   - `echo "I have no idea who ${user} is"`: `user` değişkeninin değeri kullanılarak bir metin ekrana yazdırılır.
   - `;;`: Bu durumun sonunu belirtir.

`esac`: `case` yapısının sonunu belirtir. Bu, `case` bloğunun bittiğini ve scriptin devam edebileceğini gösterir.

Bu script, kullanıcıdan bir isim girmesini ister, girilen isme göre belirli durumları kontrol eder ve buna bağlı olarak farklı çıktılar üretir. `case` yapısı, birden çok olasılığı kolayca kontrol etmek için kullanışlı bir araçtır.
```

#### 18. Learning Bash Fundamentals - funchtions
```
#!/bin/bash
#


get_hostname() {
	echo $HOSTNAME
}

get_home() {
	echo $HOME
}

echo "Hello, I am $(get_hostname). I live in the $(get_home) directory."

echo

list_files() {
        echo "There are $# arguments"
	echo "Argument 1 is $1"
	ls -al $1
}

list_files $(get_home)
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`get_hostname()` fonksiyonu:
   - Bu bölüm, `get_hostname` adında bir fonksiyon tanımlar.
   - `echo $HOSTNAME`: Bu satır, `HOSTNAME` ortam değişkeninin değerini ekrana yazdırır. `HOSTNAME` genellikle mevcut bilgisayarın ağ adını içerir.

`get_home()` fonksiyonu:
   - `get_home` adında başka bir fonksiyon tanımlar.
   - `echo $HOME`: Bu satır, `HOME` ortam değişkeninin değerini ekrana yazdırır. `HOME`, kullanıcının ana dizin yolunu içerir.

`echo "Hello, I am $(get_hostname). I live in the $(get_home) directory."`: Bu satır, yukarıda tanımlanan iki fonksiyonu kullanarak bir mesaj yazdırır. `$(get_hostname)` ve `$(get_home)` ifadeleri, bu fonksiyonların çıktılarını alır ve mesaja ekler.

`list_files()` fonksiyonu:
   - `list_files` adında bir fonksiyon daha tanımlar.
   - `echo "There are $# arguments"`: Bu satır, fonksiyona verilen argüman sayısını yazdırır. `$#` özel bir değişkendir ve fonksiyona geçirilen argümanların sayısını temsil eder.
   - `echo "Argument 1 is $1"`: Bu satır, fonksiyona geçirilen ilk argümanın değerini yazdırır. `$1`, fonksiyona geçirilen ilk argümanı temsil eder.
   - `ls -al $1`: Bu satır, `$1` değişkenindeki dizindeki dosya ve klasörleri listeler. `ls -al`, dosyaları ayrıntılı ve gizli dosyalar dahil şekilde listeler.

`list_files $(get_home)`: Bu satır, `list_files` fonksiyonunu çağırır ve argüman olarak `get_home` fonksiyonunun çıktısını kullanır. Yani kullanıcının ana dizinindeki dosya ve klasörler listelenir.

Bu script, fonksiyon tanımları ve bu fonksiyonların nasıl kullanılacağını gösteren bir örnektir. Ayrıca, fonksiyonlara argüman geçirme ve bu argümanların nasıl kullanılacağı konusunda da bilgi verir.
```

#### 20. Learning Bash Fundamentals - backup (bash ile sistem yedeklemeyi otomatik hale getirme)
```
#!/bin/bash

# Check for the directory argument passed in
backup_dir=""
if [ -z $1 ]
then
	# set the directory to engineering if nothing was passed in
	backup_dir="/usr/local/engineering"
else
	backup_dir=$1
fi

# check the directory passed in exists
if [ ! -d $backup_dir ]
then
	echo "The $backup_dir directory does not exist. Backup halted"
	exit 1
fi

# archive name
backup_file_name=/tmp/engineering_$(date +%Y-%m-%d_%H%M%S).tar.gz

# get a count of the files in the directory to be backedup
function files_to_be_backed_up {
	find $backup_dir -type f | wc -l
}


# create the backup archive
echo "Backing up $(files_to_be_backed_up) files"
# send any errors to the backup.log file
tar -czf $backup_file_name $backup_dir 2> /tmp/backup.log

# check for backup archive
if [ -f $backup_file_name ]
then
	echo "Backup succeeded!"
else
	echo "Backup failed!"
fi
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

`backup_dir=""`: Bu satır, `backup_dir` adında bir değişken oluşturur ve boş bir değer atar.

`if` Bloğu:
   - `if [ -z $1 ]`: Bu ifade, scripte verilen ilk argümanın (`$1`) boş olup olmadığını kontrol eder. `-z` testi, bir string'in boş olup olmadığını sorgular.
   - Eğer argüman boşsa, `backup_dir` değişkenine `/usr/local/engineering` değerini atar.
   - Eğer argüman boş değilse, `backup_dir` değişkenine bu argümanın değerini atar.

İkinci `if` Bloğu:
   - `if [ ! -d $backup_dir ]`: Bu ifade, `backup_dir` değişkeninin bir dizin olup olmadığını kontrol eder. `! -d` testi, belirtilen yolun bir dizin olmadığını sorgular.
   - Eğer belirtilen dizin yoksa, bir hata mesajı yazdırır ve scripti `exit 1` komutu ile hata koduyla sonlandırır.

`backup_file_name=/tmp/engineering_$(date +%Y-%m-%d_%H%M%S).tar.gz`: Bu satır, yedekleme dosyasının adını oluşturur. `date` komutu ile tarih ve saat bilgisi alınır ve bu, dosya adının bir parçası olur.

`files_to_be_backed_up` Fonksiyonu:
   - Bu bölüm, `files_to_be_backed_up` adında bir fonksiyon tanımlar.
   - Fonksiyon, `find` komutu ile `backup_dir` içindeki tüm dosyaları bulur ve `wc -l` ile dosya sayısını hesaplar.

Yedekleme Arşivi Oluşturma:
   - Bu satır, yedeklenecek dosya sayısını yazdırır.
   - `tar -czf $backup_file_name $backup_dir 2> /tmp/backup.log`: `tar` komutu ile belirtilen dizindeki dosyaları sıkıştırıp arşivler. Herhangi bir hata `/tmp/backup.log` dosyasına yönlendirilir.

Yedekleme Arşivini Kontrol Etme:
   - `if [ -f $backup_file_name ]`: Bu ifade, yedekleme dosyasının başarıyla oluşturulup oluşturulmadığını kontrol eder.
   - Eğer dosya varsa, yedeklemenin başarılı olduğunu belirten bir mesaj yazdırır.
   - Eğer dosya yoksa, yedeklemenin başarısız olduğunu belirten bir mesaj yazdırır.

Bu script, belirtilen bir dizini yedeklemek için kullanılır. Eğer scripte bir dizin yolu argümanı verilmezse, varsayılan olarak `/usr/local/engineering` dizini kullanılır. Yedekleme işlemi, `tar` komutu ile gerçekleştirilir ve yedekleme sırasında oluşabilecek hatalar bir log dosyasına yazılır. Ayrıca, yedekleme işlemi başarılı olup olmadığı da kontrol edilir. Bu script, argümanların kullanımı, koşullu ifadeler, fonksiyon tanımları ve dosya/dizin işlemleri gibi bash scripting'in temel konularını kapsar.
```
   #### 20--1. Buna ek olarak bir crontab yapısı ile süreci otomatik hale getirebilirsiniz.
```
`crontab` (cron table), Unix ve Unix-benzeri işletim sistemlerinde zaman tabanlı görev planlaması için kullanılan bir araçtır. "Cron" adı, "chronos" (Yunanca'da "zaman") kelimesinden türetilmiştir. `crontab` dosyaları, sistemde düzenli aralıklarla otomatik olarak çalıştırılması gereken scriptlerin ve komutların zamanlamasını tanımlar.

`crontab` ile ilgili ana konular şunlardır:

**Crontab Dosyaları**: Her kullanıcının kendi `crontab` dosyası olabilir. Bu dosyalar, kullanıcının belirlediği zamanlarda çalıştırılacak komutları içerir.

**Sözdizimi**: Bir `crontab` girdisi beş alan içerir: dakika (0 - 59), saat (0 - 23), ayın günü (1 - 31), ay (1 - 12 veya isimler), haftanın günü (0 - 7, hem 0 hem de 7 Pazar anlamına gelir). Bu alanların ardından çalıştırılacak komut gelir.

   Örnek:

   30 08 * * * /home/user/backup.sh

   Bu örnek, her gün saat 08:30'da `backup.sh` scriptini çalıştırır.

3. **Yönetim Komutları**:
   - `crontab -e`: Kullanıcının crontab dosyasını düzenlemek için kullanılır.
   - `crontab -l`: Mevcut crontab dosyasını görüntüler.
   - `crontab -r`: Kullanıcının crontab dosyasını siler.

4. **Sistem Genelinde Cron İşleri**: Sistemin kendisi de kendi cron işlerini çalıştırabilir. Bu işler genellikle `/etc/crontab` dosyasında veya `/etc/cron.*` dizinlerinde tanımlanır.

`crontab`, otomatik yedeklemeler, rapor oluşturma, sistem güncellemeleri gibi düzenli olarak gerçekleştirilmesi gereken görevler için sıkça kullanılır. Bu mekanizma, sistem yöneticileri ve geliştiriciler için oldukça değerli bir araçtır.
```

#### 21. Learning Bash Fundamentals - system info (bash ile sistem bilgilerini görüntüleme)
```
#!/bin/bash

# host
user=$(whoami)
active_user_count=$(users | wc -w)
hostname=$(uname -n)
disk_used=$(df -Ph | grep xvda1 | awk '{print $4}' | tr -d '\n')
release=$(cat /etc/system-release)

# AWS IMDSv1
instance_id=$(curl -s http://169.254.169.254/latest/meta-data/instance-id)
ami_id=$(curl -s http://169.254.169.254/latest/meta-data/ami-id)

# system metrics
memory1=$(cat /proc/meminfo | grep MemAvailable | awk '{print $2}')
memory2=$(cat /proc/meminfo | grep MemTotal | awk '{print $2}')
swap_in_use=$(free | tail -n 1 | awk '{print $3}')
all_processes=$(ps -Afl | wc -l)

# time of day
hour=$(date +"%H")
if [ $hour -lt 12  -a $hour -ge 0 ]
then
	time="morning"
elif [ $hour -lt 17 -a $hour -ge 12 ]
then
	time="afternoon"
else
	time="evening"
fi

#System uptime
uptime=$(cat /proc/uptime | cut -f1 -d.)
up_days=$((uptime/60/60/24))
up_hours=$((uptime/60/60%24))
up_mins=$((uptime/60%60))
up_secs=$((uptime%60))

#System load
load1=$(cat /proc/loadavg | awk {'print $1'})
load5=$(cat /proc/loadavg | awk {'print $2'})
load15=$(cat /proc/loadavg | awk {'print $3'})

echo "

:'######::'##::::'##::::'###::::'##:::::::'##:::::::'########:'##::: ##::'######:::'########:::::::::::'#######:::'#######::'########:
'##... ##: ##:::: ##:::'## ##::: ##::::::: ##::::::: ##.....:: ###:: ##:'##... ##:: ##.....:::::::::::'##.... ##:'##.... ##: ##.....::
 ##:::..:: ##:::: ##::'##:. ##:: ##::::::: ##::::::: ##::::::: ####: ##: ##:::..::: ##::::::::::::::::..::::: ##: ##::::..:: ##:::::::
 ##::::::: #########:'##:::. ##: ##::::::: ##::::::: ######::: ## ## ##: ##::'####: ######:::'#######::'#######:: ########:: #######::
 ##::::::: ##.... ##: #########: ##::::::: ##::::::: ##...:::: ##. ####: ##::: ##:: ##...::::........::...... ##: ##.... ##:...... ##:
 ##::: ##: ##:::: ##: ##.... ##: ##::::::: ##::::::: ##::::::: ##:. ###: ##::: ##:: ##::::::::::::::::'##:::: ##: ##:::: ##:'##::: ##:
. ######:: ##:::: ##: ##:::: ##: ########: ########: ########: ##::. ##:. ######::: ########::::::::::. #######::. #######::. ######::
:......:::..:::::..::..:::::..::........::........::........::..::::..:::......::::........::::::::::::.......::::.......::::......:::

Good $time $user"

echo "
===========================================================================
- Hostname............: ${hostname}
- Instance ID.........: ${instance_id}
- AMI ID..............: ${ami_id}
- Release.............: ${release}
- Users...............: Currently ${active_user_count} User(s) logged on
===========================================================================
- Current user........: ${user}
- Load................: ${load1}, ${load5}, ${load15} (1, 5, 15 min)
- Memory used.........: ${memory1} KB / ${memory2} KB
- Swap in use.........: ${swap_in_use} KB
- Processes...........: ${all_processes} running
- System uptime.......: ${up_days} days ${up_hours} hours ${up_mins} minutes ${up_secs} seconds
- Disk space /........: ${disk_used} remaining
===========================================================================
"
```
```
`#!/bin/bash`: Bu satır, scriptin hangi yorumlayıcı tarafından çalıştırılacağını belirtir. Burada `/bin/bash` yolu ile bash yorumlayıcısı kullanılacağını gösterir. Bu satıra "shebang" denir ve script dosyasının en başında yer alır.

**Host Bilgileri**:
   - `user=$(whoami)`: Şu anda giriş yapmış olan kullanıcının adını alır ve `user` değişkenine atar.
   - `active_user_count=$(users | wc -w)`: Sisteme giriş yapmış olan aktif kullanıcı sayısını hesaplar.
   - `hostname=$(uname -n)`: Sistemin ağ adını alır.
   - `disk_used=$(df -Ph | grep xvda1 | awk '{print $4}' | tr -d '\n')`: `xvda1` cihazının kullanılan disk alanını hesaplar.

**AWS IMDSv1 Bilgileri**:
   - `instance_id=$(curl -s http://169.254.169.254/latest/meta-data/instance-id)`: AWS EC2 instance ID'sini alır.
   - `ami_id=$(curl -s http://169.254.169.254/latest/meta-data/ami-id)`: AWS EC2 instance'ının AMI ID'sini alır.

**Sistem Metrikleri**:
   - `memory1=$(cat /proc/meminfo | grep MemAvailable | awk '{print $2}')`: Mevcut kullanılabilir belleği alır.
   - `memory2=$(cat /proc/meminfo | grep MemTotal | awk '{print $2}')`: Toplam sistem belleğini alır.
   - `swap_in_use=$(free | tail -n 1 | awk '{print $3}')`: Kullanılan swap alanını hesaplar.
   - `all_processes=$(ps -Afl | wc -l)`: Sistemde çalışan toplam süreç sayısını hesaplar.

**Zamanı Belirleme**:
   - Bu blok, günün saatine göre zaman dilimini (`morning`, `afternoon`, `evening`) belirler ve `time` değişkenine atar.

**Sistem Çalışma Süresi**:
   - Bu blok, sistem çalışma süresini gün, saat, dakika ve saniye cinsinden hesaplar.

**Sistem Yükü**:
   - Bu blok, sistemin son 1, 5 ve 15 dakikadaki ortalama yükünü hesaplar.

**Ekrana Bilgi Yazdırma**:
   - Bu blok, önce bir ASCII sanatı ve ardından kullanıcıya iyi zamanlar dileyen bir mesaj yazdırır.

**Detaylı Sistem Bilgilerini Yazdırma**:
   - Bu blok, yukarıda hesaplanan tüm sistem bilgilerini formatlı bir şekilde ekrana yazdırır.

Bu script, sistem ve AWS EC2 instance bilgilerini toplayıp bunları detaylı bir şekilde ekrana yazdırır. Sistem yöneticileri ve kullanıcılar için yararlı bir kaynak sağlayarak, sistem durumu hakkında hızlı bir genel bakış sunar.
```

<hr/>

</br>

<h2> [Day-15] January 15, 2024 : Hands-on Linux for DevOps & Cloud Engineers | [EN] </h2>  

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
```
![image](/Months/January/January-Images/January.png)
```
• OS-Level Virtualization
• namespaces
• C groups
• Container Orchestration
```
![image](/Months/January/January-Images/January-1.png)
```
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
   ◇ Multi: Infrastructure and services are accessed and served through two or more cloud providers.
```

