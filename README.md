# Git Nedir?
Git versiyon konrolünü sağlayan bir sistemdir. Projelerinizin her adımının versiyonlarını alarak daha sonra bu aldığınız versiyonların kopyalarına geri dönülmesini sağlayabiliriz. Bunu yapmamızın amacı en son üzerinde çalıştığımız versiyonda bir aksilik olma durumunda daha önceki düzgün çalışan herhangi bir versiyondanki çalışmamıza dönüp, ordan devam edebiliriz. Yazılım geliştiriciler tarafından daha çok kullanılır ancak bilgisayar üzerinde yapacağınız herhangi bir makalede, projede, tezde uygulayıp kullanabilirsiniz. Kullanım alanı oldukça geniştir. Bu git sistemini Linux çekirdeğini yazan linus torvalds tarafından yazılımıştır. Açık kaynak kodlu bir özgür yazılım ürünüdür. Herhangi bir ücret ödemeden kurup kullanabilirsiniz. 
# Git Kurulumu?
Herhangi bir arama motoruna **_git donwnload_** yazarsanız, çıkan sonuçlar içinden git\'in resmi sayfası olan [git-scm.com](https://git-scm.com/downloads) web adresinden kullandığınız işletim sistemi için uygun olanı indirip bilgisayarınıza kurabilirsiniz. Windowsta kurulumdan sonra Git Bash, Git GUI ve Git CMD gibi üç ayrı git uygulaması kurulacaktır. Hepsi aynı işi yapmakla beraber Linux ortamında Terminal üzerinde çalışacağımızdan yazdığımız komutların düzgün çalışması için Windows ortamında **_Git Bash_** kullanarak komutları yazacağız. Linux ortamında kurulumun yapılıp, yapılmadığını öğrenmek için aşağıdaki komut sonucunda git programın hangi version kuruluysa görüntülenmesi gerekir.
<br>
```git --version```
# Git Yapılandırma?
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
# Git Projesi Oluşturma?
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

# Git Deposuna(Repository) Proje Dosyalarını Ekleme?
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
# Git Projemizde Yapılan Değişiklikleri Listeleme ve Git Deposuna(Repository) Ekleme?
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
# Git İş Akışı?
|  Çalışma Dizini | ==>add==> | Geçiş Bölgesi | ==>commit==> | Git Deposu |
| --- | --- | --- | --- | --- |
| (Working Directory) | ==>add==> | (Staging Area) | ==>commit==> | Git Repository |
                 
<br>
 Git'in iş akışını ```git add .``` komutu ile çalışma dizininde bulunan dosya ve klasörleri Geçiş bölgesine ekliyoruz, daha sonra ```git commit -m "Mesajımızı yazıyoruz"``` ikinci işlemi uyguluyarak geçiş bölgesine gönderdiğimiz bu dosya ve klasörlerimizi Git Deposuna göndermiş oluyoruz. Geçiş Bölgesi, bize yaptığımız değişikleri kontrol etme imkanı sağlıyor.
