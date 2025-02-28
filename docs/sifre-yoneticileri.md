<!-- NOTLAR 
 - Bu kategoride lokal ve bulut tabanlı şifre yöneticileri ayrı ayrı eklenebilir- tek bir tabloda belirtilebilir ancak lokal ve bulut tabanlı şifre yöneticilerinin farkı anlatılmalıdır. 
 - Tablo eklemeyi unutmayın 
 - Uygun görseller eklemeyi unutmayın.
 - İçerik kuralları ve ekleme yapmak sayfalarını ziyaret edebilirsiniz -->

# Şifre Yöneticileri

**Şifre yöneticileri** kullanıcıların güvenli bir şekilde şifrelerini saklama, yönetme veya otomatik doldurmalarına yarayan uygulamalardır. Saklanan tüm şifreler, güçlü şifreleme algoritmaları ile korunur. Bu, verilerin yetkisiz erişimlere karşı güvenli olmasını sağlar. Lokal veya bulut tabanlı çalışan şifre yöneticileri vardır.

* Lokal şekilde çalışan şifre yöneticileri, verileri yerel cihazınızda şifreleyerek saklar yine aynı cihazda şifrerelenmiş verileri çözümleyerek kullanır.
* Bulut tabanlı çalışan şifre yöneticileri yine lokal şekilde verileri şifreler ancak bu şifrelenmiş verileri uzakta bulunan bir sunucuda barındırır.

Bu durum, lokal şifre yöneticilerinin farklı cihazlarda senkronize bir şekilde çalışmamasına neden olur. Örneğin lokal çalışan bir şifre yöneticisine kaydettiğiniz şifre, telefonunuzda bulunan şifre yöneticisine gelmez. Senkronize çalışan bir şifre yöneticisi için bulut tabanlı çalışan alternatiflere yönelmeniz önerilir.

?> Örneğin MD5 algoritması ile şifrelenen `şifre123` şeklinde ki şifrenin çıktısı `8c8e8f3c1c1c1c1c1c1c1c1c1c1c1c1c` şeklinde gözükür. Bu şifre yalnızca şifre yöneticinize giriş yaptığınız zaman çözümlenir. Bu nedenle şifre yöneticisine koyduğunuz ana şifreye
güçlü bir şifre koymanız önemlidir.

Lokal şekilde çalışan şifre yöneticilerinde [**senkronizasyon araçları**](https://guvendekal.org/#/senkronizasyon) sayesinde şifrelerinizi diğer cihazlarda senkronize edebilirsiniz ancak bu ekstra yapılandırmalar kurmanıza neden olacaktır.

Şifre yöneticisi kullanmanız [**güvenlik**](https://guvendekal.org/#/guvenlik) açısından iyi bir tercih olacaktır. Çünkü şifre yöneticileri farklı hesaplarınızda farklı ve güvenli şifreler kullanmanıza olanak sağlayacaktır. Bugün çoğu kullanıcı çoğu hesabına benzer şifreler koymaktadır bu da herhangi bir veri ihlalinde sızan hesap bilgilerinin başka site/uygulamalarda denenerek o hesaplara erişilebileceği anlamına gelir.

## Önerilenler Tablosu

| Şifre Yöneticisi | Açık Kaynak | Çalışma Şekli         | Platform Desteği         |
|-------------------|:-------------:|:-----------------------:|:--------------------------:|
| <img src="docs/images/keepassxc.png" alt="KeepassXC" style="width: 30px; height: 30px; vertical-align: middle; display: inline-block;"> <span style="vertical-align: middle; display: inline-block;"> [KeepassXC](https://keepassxc.org/) </span> | <span style="color: green;">✓</span>        | Lokal                 | <i class="fa-solid fa-globe"></i> <i class="fa-brands fa-windows"></i> <i class="fa-brands fa-apple"></i> <i class="fa-brands fa-linux"></i> |
| <img src="docs/images/bitwarden.png" alt="Bitwarden" style="width: 30px; height: auto; vertical-align: middle; display: inline-block;"> <span style="vertical-align: middle; display: inline-block;"> [Bitwarden](https://bitwarden.com/) </span> | <span style="color: green;">✓</span>        | Bulut                 | <i class="fa-solid fa-globe"></i> <i class="fa-brands fa-windows"></i> <i class="fa-brands fa-apple"></i> <i class="fa-brands fa-linux"></i> <i class="fa-brands fa-android"></i> <i class="fa-brands fa-app-store-ios"></i> |
| <img src="docs/images/vaultwarden.png" alt="Vaultwarden" style="width: 30px; height: 30px; vertical-align: middle; display: inline-block;"> <span style="vertical-align: middle; display: inline-block;"> [Vaultwarden](https://github.com/dani-garcia/vaultwarden ) </span> | <span style="color: green;">✓</span>        | Self-host             | <i class="fa-brands fa-windows"></i> <i class="fa-brands fa-apple"></i> <i class="fa-brands fa-linux"></i> <i class="fa-brands fa-android"></i> <i class="fa-brands fa-app-store-ios"></i> |
| <img src="docs/images/kwalletmanager.png" alt="KWalletManager" style="width: 30px; height: auto; vertical-align: middle; display: inline-block;"> <span style="vertical-align: middle; display: inline-block;"> [KWalletManager](https://apps.kde.org/kwalletmanager5/) </span> | <span style="color: green;">✓</span>        | Lokal                 | <i class="fa-solid fa-globe"></i> <i class="fa-brands fa-linux"></i> |

### <span style="display: inline-block; vertical-align: middle;"><img src="docs/images/keepassxc.png" alt="KeepassXC" style="width: 50px; height: auto;"> </span> <span style="display: inline-block; vertical-align: middle;"> KeepassXC

[**KeepassXC**](https://keepassxc.org/), açık kaynak ve ücretsiz şekilde geliştirilen şifre yöneticisidir. Lokal şekilde çalışan KeepasXC, [**Keepass**](https://keepass.info/)'ın forkudur. Keepass'ın aksine Linux ve Mac platformlarındada desteklemektedir. Aynı zamanda bazı eklentilerde varsayılan olarak KeepassXC'de bulunmaktadır. KeepassXC'de ekstra olarak platformlar arasında senkronizasyon yapmanıza yarayan servisler mevcuttur.

KeepassXC tarafından Android'de kullanmak için [**KeepassDX**](https://play.google.com/store/apps/details?id=com.kunzisoft.keepass.free) yada [**Keepass2Android**](https://play.google.com/store/apps/details?id=keepass2android.keepass2android), IOS'ta kullanmak için [**Strongbox**](https://apps.apple.com/us/app/strongbox-password-manager/id897283731) yada [**Keepassium**](https://apps.apple.com/us/app/keepassium-keepass-passwords/id1435127111) önerilir.

### <span style="display: inline-block; vertical-align: middle;"><img src="docs/images/bitwarden.png" alt="Bitwarden" style="width: 50px; height: auto;"> </span> <span style="display: inline-block; vertical-align: middle;"> Bitwarden

Bulut tabanlı çalışan [**Bitwarden**](https://bitwarden.com/) açık kaynaklı ve ücretsiz bir şifre yönetici uygulamasıdır. Neredeyse bütün platformlarda uygulamaları ve bütün tarayıcılarda eklentileri bulunur ve senkronize şekilde çalışmaktadır.

Bitwarden'da tüm veriler kullanıcı cihazında şifrelenir ve şifre çözümlenir; bu da herhangi bir veri ihlali yada çalınma durumlarında, hırsızların eline sadece şifrenin hash değerlinin geçeceği anlamına gelir. Bitwarden'in ücretli ve ücretsiz sürümleri bulunur. Bitwarden'in ücretli sürümü TOTP, gelişmiş 2FA seçenekleri, 1 GB şifreli dosya saklama gibi ek özellikler sunar.

### <span style="display: inline-block; vertical-align: middle;"><img src="docs/images/vaultwarden.png" alt="Vaultwarden" style="width: 50px; height: auto;"> </span> <span style="display: inline-block; vertical-align: middle;"> Vaultwarden

Kullanıcıların, Bitwarden'in sunucuları yerine kendi sunucularında şifrelerini barındırmaya yarayan [**Vaultwarden**](https://github.com/dani-garcia/vaultwarden) Rust ile yazılmıştır- ki bu da sunucu tarafında daha az açık anlamına gelir-.

Vaultwarden'in kendi sunucunda barındırılabilmesi nedeniyle verilerin tamamen kullanıcı tarafından kontrol edilmesini sağlar. Parola ve hassas bilgiler üçüncü taraf bir hizmet sağlayıcıya emanet edilmez.

?> Bitwarden tarafında herhangi bir veri ihlali yaşanırsa, çalınacak veriler zaten şifrelenmiş veriler olacaktır.

Vaultwarden, internet bağlantısı olmadan da kullanılabilir. Sunucuya lokal ağ üzerinden erişilebilir ve çevrimdışı çalışmaya devam edebilir.

### <span style="display: inline-block; vertical-align: middle;"><img src="docs/images/kwalletmanager.png" alt="KWalletManager" style="width: 50px; height: auto;"> </span> <span style="display: inline-block; vertical-align: middle;"> KWalletManager

KWalletManager, açık kaynaklı, lokal olarak ve sadece Linux sistemleri üzerinde çalışan bir şifre yöneticisid.r. Listedeki diğer şifre yöneticilerinden farkı ise sadece Linux sistemlerinde desteklenmesi ve daha çok Plasma masaüstü ortamında tercih edilmesidir. KDE ekibi tarafından geliştirilen KWalletManager tamamen çevrimdışı çalışmakla beraber kullanması da oldukça basittir. Ayrıca KWalletManager, KDE ekibinin yapmış olduğu KWallet sistemini altyapı olarak kullanmaktadır.

Uygulamalarınızı KWalletManager ile rahatlıkla eşleyebilir ve böylece şifrelerinizi kaydetmeniz daha da kolaylaşır. KWalletManager'ı birçok repo'dan indirebileceğiniz gibi tercihe bağlı olarak [Flathub](https://flathub.org/apps/org.kde.kwalletmanager5) üzerinden de indirebilirsiniz.