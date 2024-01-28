<h2> [Day-21] January 21, 2024 : Malware Analysis Temelleri - Adım 02 | [TR] </h2> 

<h3> Dinamik Kötü Amaçlı Yazılım Analizi </h3> 

#### 1. Dinamik kötü amaçlı yazılım analizi nedir?
```
"Dinamik kötü yazılım analizi yöntemi, kötü amaçlı yazılımın güvenli ortamlarda çalıştırılıp incelendiği bir analiz metodudur. Bu yöntemde, güvenli ortamlarda ağ ve dosya gibi faaliyetlerin incelenmesi yoluyla kötü amaçlı yazılımın davranışının analiz edilmesi amaçlanır.

SOC analistleri tarafından, statik analiz metoduna göre daha hızlı analiz yapılabilmesi sebebiyle genellikle ilk tercih edilen bir yöntemdir. Statik Analiz ve Dinamik Analiz yöntemleri hakkında blog yazımızı burada bulabilirsiniz.

Dinamik analizi otomatikleştirmek için çeşitli sandbox çözümleri mevcuttur. Sandbox'lar, kötü amaçlı yazılımı kendi izole ortamlarında çalıştırır ve analiz sonuçlarını otomatik olarak sunar. Bu sandbox çözümleri, SOC analistleri için hayati öneme sahiptir."
```

#### 2. Dinamik Analizin Avantajları
```
"Dinamik analiz metodunun bazı avantajları şunlardır;
• Statik analiz metoduna göre çok daha hızlı sonuçlar üretir,
• Sandbox'lar ile otomatik analiz yapabilirsiniz,
• Statik analize göre daha az teknik bilgi gerektiren bir analiz yöntemidir, bu yüzden başlangıç seviyesindekiler kolaylıkla öğrenebilir."
```

#### 3. Dinamik Analizin Dezavantajları
```
"Dinamik analiz yönteminin bazı dezavantajları şunlardır;
• Kötü amaçlı yazılımın davranışı farklı sistemlerde değişebileceği için, kötü amaçlı yazılımın tam kapasitesini belirleyemezsiniz.
• Genellikle, gelişmiş kötü amaçlı yazılımları yalnızca dinamik analiz yöntemiyle analiz edemezsiniz, bu tür durumlarda hem dinamik hem de statik analiz yöntemlerini birlikte kullanmanız gerekebilir."
```

<hr/>

</br>


<h2> [Day-21] January 21, 2024 : Malware Analysis Fundamentals - Step 02 | [EN] </h2>

<h3> Dynamic Malware Analysis </h3> 

#### 1. What is dynamic malware analysis?
```
"Dynamic malware analysis is a method where malicious software is executed and examined in secure environments. This method aims to analyze the behavior of the malware by examining activities such as network and file operations in these secure environments.

For SOC analysts, this method is often the first choice as it allows for quicker analysis compared to the static analysis method. You can find our blog post about Static and Dynamic Analysis methods here.

Various sandbox solutions are available to automate dynamic analysis. Sandboxes run the malicious software in their isolated environments and automatically provide analysis results. These sandbox solutions are of vital importance to SOC analysts."
```

#### 2. Advantages of Dynamic Analysis
```
"Some advantages of the dynamic analysis method include:
• It produces much faster results compared to the static analysis method,
• You can perform automated analysis with sandboxes,
• It requires less technical knowledge compared to static analysis, making it easier for beginners to learn."
```

#### 3. Disadvantages of Dynamic Analysis
```
"Some disadvantages of the dynamic analysis method include:
• Since the behavior of malicious software can vary across different systems, you might not be able to determine its full capabilities.
• Often, you cannot analyze advanced malicious software with only the dynamic analysis method; in such cases, you may need to use both dynamic and static analysis methods together."
```