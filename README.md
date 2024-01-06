# Python ile Muz Meyvesi Gelişim Evreleri Sınıflandırması: CNN, Transfer Learning ve Yapay Sinir Ağı

Bu proje, muz meyvesinin farklı gelişim evrelerini sınıflandırmak için kullanılan bir yapay zeka modelini içermektedir. CNN, Transfer Learning ve Yapay Sinir Ağı (ANN) yaklaşımları kullanılarak geliştirilmiştir.

## Proje Ne İşe Yarar?

Bu proje, muz meyvesinin görsel verilerini kullanarak, meyvenin farklı gelişim evrelerini sınıflandırmak için bir model içerir. Bu, ürün kalitesini değerlendirmek veya üretim süreçlerini optimize etmek için kullanılabilir.

## Neden Faydalıdır?

- Tarım endüstrisinde, meyve gelişim evrelerini otomatik olarak sınıflandırma imkanı sunar.
- Ürün kalitesini artırabilir ve iş süreçlerini optimize edebilir.
- Makine öğrenimi ve görüntü sınıflandırma konularında ilgilenenler için eğitim amacı taşır.

## Nasıl Kullanılır?

Bu proje, Google Colab üzerinde Python kullanılarak geliştirilmiştir. Aşağıda projeyi çalıştırmak için adımları bulabilirsiniz:

1. **Google Colab Girişi:**
   - [Google Colab](https://colab.research.google.com/)'a gidin ve Google hesabınıza giriş yapın.

2. **Projeyi Ekleme:**
   - Sol üst köşede bulunan "Dosya" menüsünden "Yeni Notebook" seçeneğini kullanarak yeni bir Colab Notebook oluşturun.
   - GitHub'dan kopyaladığınız kodu Colab Notebook içine ekleyin.
  
3. **Veri Setini Yükleme:**
   - Google Drive'ınıza gidin ve veri setinizi yükleyin veya sürükleyip bırakın.

4. **Veri Seti Yolu Belirleme:**
   - Kodun aşağıdaki satırında yüklediğiniz dosyanın yolunu değiştirin.

      DATA = '/gdrive/MyDrive/odev_dosya/Banana_Ripeness_Classification'
     
4. **Proje Hiperparametreleri ve Açıklamaları:**
   
   - Eğitim Verisi:
      Daha fazla eğitim verisi genellikle daha iyi genelleme sağlar ancak bu, daha uzun eğitim süreleri gerektirebilir.
     
   - Test ve Validation Veri Oranları:
      Veri setinizin boyutuna ve bütünlüğüne bağlı olarak, test ve validation için ayrılan veri oranlarını değiştirebilirsiniz. Daha büyük bir test seti, modelin gerçek performansını daha iyi                            değerlendirmenize yardımcı olabilir.
     
   Örnek olarak koddaki "test_size=0.2" değeri veri setinin %80'i Eğitim %20'si Test olarak kullanır.
     
   - epochs: Daha fazla epoch, modelin eğitim setine daha fazla adapte olmasını sağlar, ancak aşırı uyum riskini artırabilir.
   epochs=10

   - batch_size: Daha büyük batch size, daha hızlı eğitim süresine neden olabilir, ancak daha fazla bellek kullanabilir. Küçük batch size, modelin daha güncel bilgilerle eğitilmesine yardımcı olabilir, ancak             eğitim süresini uzatabilir.
   batch_size=32

   - dropout_orani: Düşük bir dropout oranı, modelin daha fazla öğrenmesine izin verebilir, ancak aşırı uyum riskini artırabilir. Yüksek bir dropout oranı, modelin genellemesini artırabilir ancak modelin öğrenme       kapasitesini azaltabilir.
   dropout_orani=0.5
     
   - verbose: Eğitim sırasında ne kadar çıktı almak istediğinize bağlı olarak bu değeri ayarlayabilirsiniz. Daha fazla çıktı, eğitim sürecini daha ayrıntılı olarak gösterir, ancak fazla detay bazen karışıklığa          neden olabilir.
   verbose=0
