# Git 
## Git Nedir?
Git versiyon konrolünü sağlayan bir sistemdir. Projelerinizin her adımının versiyonlarını alarak daha sonra bu aldığınız versiyonların kopyalarına geri dönülmesini sağlayabiliriz. Bunu yapmamızın amacı en son üzerinde çalıştığımız versiyonda bir aksilik olma durumunda daha önceki düzgün çalışan herhangi bir versiyondanki çalışmamıza dönüp, ordan devam edebiliriz. Yazılım geliştiriciler tarafından daha çok kullanılır ancak bilgisayar üzerinde yapacağınız herhangi bir makalede, projede, tezde uygulayıp kullanabilirsiniz. Kullanım alanı oldukça geniştir. Bu git sistemini Linux çekirdeğini yazan linus torvalds tarafından yazılımıştır. Açık kaynak kodlu bir özgür yazılım ürünüdür. Herhangi bir ücret ödemeden kurup kullanabilirsiniz. 
## Git Kurulumu?
Herhangi bir arama motoruna **_git donwnload_** yazarsanız, çıkan sonuçlar içinden git\'in resmi sayfası olan [git-scm.com](https://git-scm.com/downloads) web adresinden kullandığınız işletim sistemi için uygun olanı indirip bilgisayarınıza kurabilirsiniz. Windowsta kurulumdan sonra Git Bash, Git GUI ve Git CMD gibi üç ayrı git uygulaması kurulacaktır. Hepsi aynı işi yapmakla beraber Linux ortamında Terminal üzerinde çalışacağımızdan yazdığımız komutların düzgün çalışması için Windows ortamında **_Git Bash_** kullanarak komutları yazacağız. Linux ortamında kurulumun yapılıp, yapılmadığını öğrenmek için aşağıdaki komut sonucunda git programın hangi version kuruluysa görüntülenmesi gerekir.
<br>
```git --version```
## Git Yapılandırma?
Kurulumunu yaptığımız git programına ilk önce Kullanıcı adımızı(name) ve e-mailizi tanıtmamız gerekiyor. Bunu yapmamızın amacı git projemizde alınan versiyonların kimin tarafından alındığını belirmektir. Linux ortamında Terminalde yada windows ortamında ise Git Bash ekranında aşağıdaki komutları belirtilen sırada yazılması gerekir.
<br>
```git config --global user.name \"Kendi Adınızı Yazın\"```
<br>
```git config --global user.email \"Kendi E-mail Adresinizi Yazın\"```
<br>
Bundan sonra yazacağımız bütün komutların başına \'git\' yazıcaz. Git sisteminde tanımladığımız kullanıcı adını ve e-mail adresimizin doğru bir şekilde yazmışmıyız yada bunları görmek için aşağıdaki komutları yazmamız gerekir. 
<br>
```git config --global user.name```
<br>
```git config --global user.email```
<br>
## Git Projesi Oluşturma?
Git projesi oluşturmadan önce bilmemiz gerekli olan bir kaç Terminal ve Git Bash komutlarını öğrenelim. Bulunduğumuz mevcut dizinin tam adresini öğrenmek için aşağıdaki komutu yazmalıyız.
<br>
```pwd```
<br>
Bulunduğumuz dizindeki dosya ve klasörleri listelemek için:
<br>
```ls```
<br>
Bulunduğumuz dizindeki dosya ve klasörleri ayrıntılı bir şekilde listelemek için:
<br>
```ls -l```
<br>
Bulunduğumuz dizindeki gizli dosya ve klasörleri listelemek için:
<br>
```ls -a```
<br>
Bulunduğumuz dizin ve klasör adresini değiştirmek için bir alt klasör yada dizine geçme komutu:
<br>
```cd dizin_ismi_yolu```
<br>
Bulunduğumuz dizin ve klasör adresini değiştirmek için bir üst klasör yada dizine geçme komutu:
<br>
```cd ..```
<br>
Bulunduğumuz dizin ve klasör\'ün altında yeni bir klasör oluşturmak için yada işletim sistemin grafik aryüzünde sağ tıklayıp Yeni Klasör oluştur menüsünden aynı işlemi gerçekleştirebiliriz.
<br>
```mkdir klasör_ismi```
<br>
Bulunduğumuz dizin ve klasör\'ün altında yeni bir dosya oluşturmak için yada işletim sistemin grafik aryüzünde sağ tıklayıp Yeni Boş Dosya oluşturabiliriz.
<br>
```touch dosya_ismi```
<br>
Teminali yada Git Bash komut ekranını temizlemek için CTRL+L  yada aşağıdaki komutu yazmamız gerekiyor.
<br>
```clear```
<br>
Son olarak Terminal ve Git Bash komutlarından sonra Git proje dizini olduğunu belirtmek için aşağıdaki komutu yazıyoruz.
<br>
```git init```
<br>
Artık yukarıdaki komut ile git projemizi belirtmiş oluyoruz ve .git adında bir gizli dosya oluşması gerekli bunuda aşağıdaki komut ile görüntüleyebiliriz.
<br>
```ls -a```
<br>

## Git Deposuna(Repository) Proje Dosyalarını Ekleme?
Git Deposu(Repository) proje dosyalarının git tarafından saklandığı yerdir. Dosyaların geçiş alanına(staging area) eklemek için aşağıdaki komutu yazıyoruz.
<br>
```git add .```
<br>
Nokta yerine dosyaların ismini teker yazabiliriz yada nokta işaret yazarak projedeki tüm dosyaları geçiş alanına ekliyoruz. Bunları geçiş bölgesinden git deposuna eklemek için aşağıdaki komutu Terminal yada Git Bash programında yazıyoruz.
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
Bu komut'tan sonra git deposuna projemizin bir kopyasını oluşturuyoruz. Aldığımız bu versiyonları listelemek için:
<br>
```git log```
<br>
bu komut sonunda aldığımız bütün versiyonları listelemesi gerekir.
## Git Projemizde Yapılan Değişiklikleri Listeleme ve Git Deposuna(Repository) Ekleme?
Git projemizde herhangi bir değişikler varsa listelemek için:
<br>
```git status```
<br>
eğer projemizde bir değişiklik varsa aşağıdaki komutları sırasıyla Git Bash yada Terminal ortamına yazarak git deposuna projemizi eklenmiş olacaktır. Bir önceki konuda Git Deposuna(Repository) Ekleme komutlar açıklamıştık.
<br>
```git add .```
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
```git log```
<br>
```git status```
<br>
## Git İş Akışı?
|  Çalışma Dizini | ==>add==> | Geçiş Bölgesi | ==>commit==> | Git Deposu |
| --- | --- | --- | --- | --- |
| (Working Directory) | ==>add==> | (Staging Area) | ==>commit==> | Git Repository |
                 
<br>
 Git'in iş akışını 
 ```git add .``` 
 komutu ile çalışma dizininde bulunan dosya ve klasörleri Geçiş bölgesine ekliyoruz, daha sonra 
 ```git commit -m "Mesajımızı yazıyoruz"``` 
 ikinci işlemi uyguluyarak geçiş bölgesine gönderdiğimiz bu dosya ve klasörlerimizi Git Deposuna göndermiş oluyoruz. Geçiş Bölgesi, bize yaptığımız değişikleri kontrol etme imkanı sağlıyor.

## Git Değişiklik(diff) yapma?
 Yapılan değişikliklerden sonra
 <br>
```git status```
<br>
komutu ile değişikliğin yapıldığını görüntüleriz. Bu sorgulamanın sonucunda aynı zamanda hangi komutları uygulayabileceğimiz git sistemi bize görüntülüyor. Satır satır yapılan değişikleri görüntülüyoruz. Kırmızı renkteki satırları sildiğimiz, yeşil renkte gösterilen satırlar değiştirilmiş olan satırlardır.
 <br>
```git diff```
<br>
eğer projemizde bir değişiklik varsa aşağıdaki komutları sırasıyla Git Bash yada Terminal ortamına yazarak git deposuna projemizi eklenmiş olacaktır. Bir önceki konuda Git Deposuna(Repository) Ekleme komutlar açıklamıştık.
<br>
```git add .```
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
```git log```
<br>
```git status```
<br>
```git diff```
<br>
En son komuttan sonra herhangi bir değişiklik olmadığını komut ekranında yazacaktır. Yapılan değişiklerden sonra:
<br>
```git add .```
<br>
```git diff```
<br>
Komutları yazılırsa yine bir değişiklik olmadığını komut ekranında yazacktır. Ancak burda Çalışma dizini(Working Directory) ile Geçiş Bölgesini(Staging Area) karşılaştırmasını yapıyor. Eğer Geçiş Bölgesi(Staging Area) ile Git Deposu(Git Repository) arasındaki değişikliği görmek istiyorsak:
<br>
```git diff --staged```
<br>
Bundan sonra Git Deposuna(Git Repository) yapılan değişikleri kaydetmek için, aşağıdaki komutu yazıyoruz.
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
## Git Projesindeki Dosyayı Silmek?
### 1-Birinci Silme Yöntemi:
Dosya silmek için iki yöntem var. Birinci yöntem direkt İşletim sisteminin grafik rayüzünde dosyanın üzerinde sağ tıklayarak elle silmek ikinci olarakta Git Bash komutu ile silebiliriz. Elle dosyayı sildikten sonra silme geçiş bölgesine kaydetmek için iki komut var.
<br>
```git add .```
<br>
yada:
<br>
```git rm dosya_ismi.dosya_uzantısı```
<br>
Bundan sonra geçiş bölgesinden, git deposuna commit etmek için:
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
### 2-İkinci Silme Yöntemi:
İkinci olarak ilk başta dosyayı silip geçiş bölgesine kaydetmek için aşağıdaki komutu çalıştırıyoruz:
<br>
```git rm dosya_ismi.dosya_uzantısı```
<br>
<br>
Bundan sonra geçiş bölgesinden, git deposuna commit etmek için:
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
En son iletilmiş olan projenin  durmunu ve iletilip iletilmeğini görmek için:
<br>
```git log```
<br>
```git status```
<br>
### 3-Klasör olarak Silme Yöntemi:
Klasörle ve altındaki kayıtlı dosyaları silmek için, aşağıdaki komutları yazıyoruz. Burada dosya silmeden farklı olarak -r parametresi var. Bunun anlamı rekürsif olarak klasör altındaki bütün dosya ve klasörlerin hepsini siler:
<br>
```git rm -r Klasör_ismi```
<br>
Bundan sonra git projemizi son haliyle geçiş bölgesinden, git deposuna commit etmek için:
<br>
```git commit -m "Mesajımızı yazıyoruz"```
<br>
## Git Projesinde Hataları ve Değişiklikleri Geri Alma?
### 1-Çalışma Dizininde:
Eğer yaptığımız hata yada geri alacağımız değişiklikler çalışma klasörü içerisinde ise geri getirmek için:
<br>
```git status```
<br>
bu komutu yazdığımızda bize değişikleri geri almak için bize aşağıdaki komutu yazmamız gerektiğini komut ekranında yazacaktır.
<br>
```git checkout -- dosyanın_ismi.uzantısı```
<br>
### 2-Geçiş Bölgesinde:
Aşağıdaki add komutu ile geçiş bölseine gönderdiğimiz değişikleri:
<br>
```git add .```
<br>
status komutunu yapılan değişikleri görüntülemeye yarar:
<br>
```git status```
<br>
bu komutu yazdığımızda bize değişikleri geri almak için bize aşağıdaki komutu yazmamız gerektiğini komut ekranında yazacaktır.
<br>
```git reset HEAD dosyanın_ismi.uzantısı```
<br>
Bu sefer çalışma dizinindende yaptığımız değişikleri geri almamız gerkir bunun için:
<br>
```git checkout -- dosyanın_ismi.uzantısı```
<br>
Değişikliklerin geri alınıp alınmadığını görmek için aşağıdaki komutu kullanabiliriz:
<br>
```git status```
<br>
## Git Versiyon Değiştirme?
Git log komutu ile ekranda daha önce commit ettiğimiz git projemizin versiyonları ve bilgileri gözükecektir.
<br>
```git log```
<br>
 Bu versiyon bilgileri içerisinde turuncu renkte gözüken hash kodu var. Bu hash kodu benzersiz olduğu için git projesinin versiyon değişikliğinde kullanılacaktır. İsterseniz hash kodunun ilk 7 karekterini kullanabiliriz. Aşağıdaki komut ile herhangi bir versiyondaki dosyanın o versiyondaki son haline dönülmesini sağlar.
<br>
```git checkout hash_kodu -- dosya_ismi.dosyanın_uzantısı```
<br>
Eğer bu versiyondaki tüm dosyaların son haline dönülmesi isteniyorsa, dosya ismi yerine nokta ifadesi kullanılmalı.
<br>
```git checkout hash_kodu -- .```
<br>
