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
