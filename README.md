# kirik_kalpli_olan_sayfa
git clone https://github.com/kirik_kalpli_sayfa/kirik_kalpli_olan_sayfa
git clone https://github.com/kirik_kalpli_sayfa/kirik_kalpli_olan_sayfa.git
...
başlık: Kod Alanları için Hızlı Başlangıç
giriş: '5 dakika içinde {% data options.product.prodname_codespaces %} ürününü deneyin.'
allowTitleToDifferFromFilename: true
ürün: '{% data reusables.gated-features.codespaces %}'
sürümler:
  fpt: '*'
  geek: '*'
tür: hızlı başlangıç
konular:
  - Kod alanları
yönlendirme_gönderen:
  - /codespaces/codespaces-hızlı başlangıç
---

## Tanıtım

Bu kılavuzda, bir [şablon deposundan](https://github.com/2percentsilk/haikus-for-codespaces) bir kod alanı oluşturacak ve kod alanında size sunulan bazı temel özellikleri keşfedeceksiniz.

Bu hızlı başlangıçtan, bir kod alanı oluşturmayı, çalışan uygulamanızı görüntülemek için iletilen bir bağlantı noktasına bağlanmayı, bir kod alanında sürüm kontrolünü kullanmayı ve kurulumunuzu uzantılarla kişiselleştirmeyi öğreneceksiniz.

{% data options.product.prodname_codespaces %}'nin tam olarak nasıl çalıştığı hakkında daha fazla bilgi için, "[Deep dalış {% data Varis.product.prodname_codespaces %}](/codespaces/getting-started/deep-dive) adlı yardımcı kılavuza bakın. "

## Kod alanınızı oluşturma

1. [şablon deposuna](https://github.com/2percentsilk/haikus-for-codespaces) gidin ve **Bu şablonu kullan**'ı seçin.

2. Deponuza bir ad verin, tercih ettiğiniz gizlilik ayarını seçin ve **Bu şablondan depo oluştur**'a tıklayın.

3. Yeni oluşturulan havuzun ana sayfasına gidin. Depo adı altında, **{% octicon "code" aria-label="Kod simgesi" %} Code** açılır menüsünü kullanın ve **Kod Alanları** sekmesinde, {% octicon "artı öğesini tıklayın. " aria-label="Artı simgesi" %} **Yeni kod alanı**.

  ![Yeni kod alanı düğmesi](/assets/images/help/codespaces/new-codespace-button.png)

## Uygulamayı çalıştırma

Kod alanınız oluşturulduktan sonra, deponuz otomatik olarak ona klonlanacaktır. Artık uygulamayı çalıştırabilir ve bir tarayıcıda başlatabilirsiniz.

1. Bu örnek bir Node.js projesi kullandığından, terminalde `npm run dev` yazarak uygulamayı başlatın. Bu komut, package.json dosyasındaki 'dev' betiğini çalıştırır ve örnek depoda tanımlanan web uygulamasını başlatır.
   
   ![npm terminalde dev çalıştırma](/assets/images/help/codespaces/codespaces-npm-run-dev.png)

    Farklı bir uygulama türü ile takip ediyorsanız, o proje için ilgili başlatma komutunu girin.

2. Uygulamanız başladığında, kod alanı uygulamanın üzerinde çalıştığı bağlantı noktasını tanır ve bağlanabilmeniz için bu bağlantı noktasını iletmeniz için bir istem görüntüler.

  ![Port yönlendirme tostu](/assets/images/help/codespaces/quickstart-port-toast.png)

3. Çalışan uygulamanızı yeni bir sekmede görüntülemek için **Tarayıcıda Aç**'a tıklayın.

## Uygulamayı düzenleyin ve değişiklikleri görüntüleyin

1. Kod alanınıza geri dönün ve `haikus.json` dosyasını Dosya Gezgini'nde çift tıklatarak açın.

2. Uygulamayı kendi haiku'nuzla kişiselleştirmek için ilk haiku'nun "metin" alanını düzenleyin.

3. Tarayıcınızda çalışan uygulama sekmesine geri dönün ve değişikliklerinizi görmek için yenileyin.
   
  {% octicon "ampul" aria-label="Ampul simgesi" %} Sekmeyi kapattıysanız, Bağlantı Noktaları panelini açın ve çalışan bağlantı noktası için **Tarayıcıda aç** simgesini tıklayın.
  ![Port Yönlendirme Paneli](/assets/images/help/codespaces/quickstart-forward-port.png)

## Değişikliklerinizi taahhüt etmek ve zorlamak

Artık birkaç değişiklik yaptığınıza göre, değişiklikleri işlemek ve uzaktan kumandaya geri göndermek için entegre terminali veya kaynak görünümünü kullanabilirsiniz.

{% data reusables.codespaces.source-control-display-dark %}
1. Değişikliklerinizi aşamaya eklemek için değiştirdiğiniz dosyanın yanındaki **+** veya birden fazla dosyayı değiştirdiyseniz ve hepsini aşamaya geçirmek istiyorsanız **Değişiklikler**'in yanındaki **+** seçeneğini tıklayın.
![Aşama düğmesi vurgulanmış olarak kaynak denetimi yan çubuğu](/assets/images/help/codespaces/codespaces-commit-stage.png)
1. Yaptığınız değişikliği açıklayan bir taahhüt mesajı yazın.
![Taahhüt mesajı içeren kaynak denetimi yan çubuğu](/assets/images/help/codespaces/codespaces-commit-commit-message.png)  
1. Aşamalı değişikliklerinizi uygulamak için kaynak denetimi yan çubuğunun üstündeki onay işaretine tıklayın.
![Onay işareti simgesini tıklayın](/assets/images/help/codespaces/codespaces-commit-checkmark-icon.png)  
    Yaptığınız değişiklikleri zorlayabilirsiniz. Bu, bu değişiklikleri uzak depodaki yukarı akış şubesine uygular. Henüz bir çekme isteği oluşturmaya hazır değilseniz veya {% data Varis.product.prodname_dotcom %} üzerinde bir çekme isteği oluşturmayı tercih ediyorsanız bunu yapmak isteyebilirsiniz.
1. Kenar çubuğunun üst kısmındaki üç noktayı (**...**) tıklayın.
![Görünüm ve Diğer İşlemler için Üç Nokta düğmesi](/assets/images/help/codespaces/source-control-ellipsis-button-nochanges.png)
1. Açılır menüde **Push**'a tıklayın.

## Uzantı ile kişiselleştirme

Bir kod alanı içinde Visual Studio Code Marketplace'e erişebilirsiniz. Bu örnekte, temayı değiştiren bir uzantı yükleyeceksiniz, ancak iş akışınız için yararlı olan herhangi bir uzantıyı yükleyebilirsiniz.

1. Sol kenar çubuğunda, Uzantılar simgesini tıklayın.

2. Arama çubuğuna 'fairyfloss' yazın ve Fairyfloss uzantısını yükleyin.

  ![Uzantı ekle](/assets/images/help/codespaces/add-extension.png)

3. Listeden seçerek 'fairyfloss' temasını seçin.

  ![peri ipi temasını seçin](/assets/images/help/codespaces/fairyfloss.png)

4. Tema ve klavye bağlamaları gibi mevcut kod alanında editör kurulumunuzda yaptığınız değişiklikler, [Ayarlar Senkronizasyonu](https://code.visualstudio.com/docs/editor/settings-sync) aracılığıyla otomatik olarak herhangi biriyle senkronize edilir. açtığınız diğer kod alanları ve GitHub hesabınızda oturum açmış tüm Visual Studio Code örnekleri.

## Sonraki adımlar

Bir kod alanında ilk uygulamanızı başarıyla oluşturdunuz, kişiselleştirdiniz ve çalıştırdınız, ancak keşfedilecek daha çok şey var! {% data options.product.prodname_codespaces %} ile sonraki adımlarınızı atmanız için bazı yararlı kaynakları burada bulabilirsiniz.
  - [Derin dalış](/codespaces/getting-started/deep-dive): Bu hızlı başlangıç, {% data options.product.prodname_codespaces %} ürününün bazı özelliklerini sundu. Derin dalış, bu alanlara teknik açıdan bakar.
  - [{% data options.product.prodname_codespaces %} için projenizi kurma](/codespaces/getting-started-with-codespaces): Bu kılavuzlar, projenizi {% data options.product.prodname_codespaces kullanacak şekilde ayarlama hakkında bilgi sağlar. %} belirli dillerle
  - [Projeniz için {% data options.product.prodname_codespaces %} yapılandırması](/codespaces/setting-up-your-codespace/configuring-codespaces-for-your-project): Bu kılavuz, projeniz için özel bir yapılandırma oluşturmaya ilişkin ayrıntılar sağlar. Projeniz için {% data options.product.prodname_codespaces %}.

## Daha fazla okuma

- [Kuruluşunuz için {% data options.product.prodname_codespaces %} etkinleştiriliyor](/codespaces/managing-codespaces-for-your-organization/eneasing-codespaces-for-your-organization)
- [Kuruluşunuzdaki {% data options.product.prodname_codespaces %} için faturalandırmayı yönetme](/codespaces/managing-codespaces-for-your-organization/managing-billing-for-codespaces-in-your-organizasyonunuz)
