# Cuff Less Blood Pressure Estimation Dataset
Cuff-Less Blood Pressure Estimation Dataset 
Veriseti ve üretilmiş sonuca ilişkin araştırma
1. Araştırmanın amacı nedir?
1.1 Giriş:
Hipertansiyon, dünya genelinde önemli bir sağlık sorunudur ve birçok kalp-damar hastalığının başlıca risk faktörüdür. Kan basıncının doğru ve düzenli bir şekilde ölçülmesi, hipertansiyonun erken teşhis edilmesi ve yönetilmesi için kritik öneme sahiptir. Geleneksel yöntemlerden biri olan manşetli kan basıncı ölçümü, kullanıcılar tarafından rahatsızlık verici ve sınırlayıcı olarak algılanabilir. Bu nedenle, manşetsiz kan basıncı tahmini, daha rahat ve kullanıcı dostu bir alternatif olarak araştırılmaktadır. Cuff-Less Blood Pressure Estimation Dataset, bu alanda yapılan çalışmalara katkıda bulunmak amacıyla oluşturulan bir veri kümesidir. Bende bu veriseti üzerinde kod analizi ile modelleme üzerinden yapılan aşamaları anlatacağım ve grafiksel çıktılarıyla bu verileri karşılaştıracağım.
1.2 Veri Seti Oluşturma:
Cuff-Less Blood Pressure Estimation Dataset, büyük ölçekli bir çalışmanın ürünüdür ve çeşitli kaynaklardan toplanan verileri içerir. Veri seti, birçok farklı özelliği içeren çeşitli katılımcılardan elde edilen gerçek zamanlı verileri içerir. Bu özellikler arasında elektrokardiyografi (EKG) verileri, nabız dalgası verileri, hızlanma verileri ve solunum verileri bulunur. Her bir katılımcının, manşetli kan basıncı ölçümü sırasında toplanan bu verileri içeren bir referans etiketine sahiptir.
1.3 Araştırma Amacı:
Cuff-Less Blood Pressure Estimation Dataset, manşetsiz kan basıncı tahmini alanında çeşitli araştırmaların temelini oluşturmak için oluşturulmuştur. Bu veri kümesi, kan basıncını tahmin etmek için makine öğrenimi ve yapay zeka algoritmalarının geliştirilmesini teşvik eder. Araştırmacılar, bu veri kümesini kullanarak farklı algoritmaları test edebilir, yeni yöntemler geliştirebilir ve mevcut yöntemleri iyileştirebilirler. Ayrıca, manşetsiz kan basıncı tahmininde kullanılan sensörlerin doğruluğunu ve güvenilirliğini değerlendirmek için bu veri kümesini kullanabilirler.
Kod bölümünde, kan basıncı ölçümleriyle ilgili veri setini analiz etmektir. Bu analizde, kandaki oksijen seviyelerini ölçen bir sensör olan fotopletismografi (PPG) sinyalleri ve elektrokardiyografi (EKG) sinyalleri kullanılmıştır.
1.4 Sonuç:
Sonuç olarak, Cuff-Less Blood Pressure Estimation Dataset, manşetsiz kan basıncı tahmini konusunda yapılan araştırmalara büyük bir katkı sağlar. Bu veri kümesi, çeşitli algoritmaların geliştirilmesi ve değerlendirilmesi için bir platform sağlayarak, hipertansiyonun erken teşhis ve yönetimi için daha kullanıcı dostu ve rahat bir yöntem geliştirilmesine yönelik çalışmalara ilham verir. Ayrıca, veri kümesi, sensör teknolojilerinin geliştirilmesi ve doğruluklarının artırılması için temel bir referans kaynağı olarak hizmet eder. Bu veri kümesinin kullanılmasıyla elde edilecek bulgular, hipertansiyonun önlenmesi ve tedavisi için daha etkili stratejilerin geliştirilmesine katkıda bulunabilir.
2. Veriseti kaç gözlemden oluşmaktadır? Satır ve sütun sayısı nedir?
Bu alanda öncelikle kod üzerinden incelediğimiz verisetinin özellikleri bakımından inceleyelim:
•	Veri seti 1000 gözlem içermektedir. 
•	Her bir gözlem için 3 sinyal kaydedilmiştir: PPG, ECG ve kan basıncı (BP). 
•	Her sinyal 125 örnekten oluşmaktadır. 
•	Systolic Blood Pressure (SBP) ve Diastolic Blood Pressure (DBP) değerleri ayrı ayrı kaydedilmiştir.
Bu kod saır dizisinin 1 satır ve 1000 sütun içerdiği anlamına gelir.
3. Verisetinin kullanımı için özel izine ihtiyaç var mı?
Veri setinin kullanımı özel izne ihtiyaç duymamaktadır. Açık kaynaklıdır. Bu açık kaynak, kaynakça tarafında paylaşılmıştır.
X.XX Hangi tür veri yapıları kullanılmıştır?
Bu kodlarda dataset analiz kodu, makine öğrenmesi modelleme kodu ve derin öğrenme modelleme kodlarındaki veri yapılarını hepsini kapsayacak şekilde açıklayacağım.
Bu kod örneğinde aşağıdaki veri yapıları kullanılmıştır:
Numpy: Sayısal hesaplamalar yapmak için kullanılan bir kütüphanedir. Örneğin, matris işlemleri gibi sayısal operasyonlar numpy kullanılarak gerçekleştirilmiştir.
Pandas: Veri manipülasyonu için kullanılan bir kütüphanedir. Veri setlerini okumak, işlemek ve analiz etmek için kullanılır.
Seaborn: Veri görselleştirmesi için kullanılan bir kütüphanedir. Grafik ve görseller oluşturmak için seaborn kütüphanesi kullanılmıştır.
Scipy: Bilimsel hesaplama ve sinyal işleme için kullanılan bir kütüphanedir. Matematiksel işlemler, sinyal işleme algoritmaları ve dönüşümler gibi çeşitli işlemleri gerçekleştirmek için scipy kullanılmıştır.
Scikit-learn: Makine öğrenimi modellerini oluşturmak ve değerlendirmek için kullanılan bir kütüphanedir. Lineer regresyon, rastgele orman regresyonu gibi modellerin oluşturulması ve eğitilmesi için scikit-learn kullanılmıştır.
Matplotlib: Grafik ve görseller oluşturmak için kullanılan bir kütüphanedir. Verilerin görselleştirilmesi amacıyla matplotlib kullanılmıştır.
TensorFlow: Derin öğrenme modellerinin oluşturulması ve eğitimi için kullanılan bir kütüphanedir. Yapay sinir ağları ve derin öğrenme modeli oluşturmak için TensorFlow kullanılmıştır.
Bu veri yapıları, kodun farklı bölümlerinde farklı amaçlarla kullanılmıştır. Örneğin, numpy matris işlemleri için kullanılmışken, pandas veri manipülasyonu ve analizi için kullanılmıştır.

4. Veri ön işlemede hangi işlemler yapılmış?
Örneğin kayıp veri var mı? Varsa hangi metodla çözülmüş.
Bu kod örneğinde veri ön işleme adımları aşağıdaki gibi yapılmıştır:
1.	Veri yükleme: İlk adımda, scipy.io.loadmat fonksiyonu kullanılarak MATLAB formatındaki veri dosyası (*.mat) yüklenmiştir (ek olarak csv uzantılı verisetide bulunmaktadır).
2.	Veri boyutlarına bakma: Yüklenen veri dosyasının boyutları incelenmiştir. shape fonksiyonu kullanılarak veri boyutları kontrol edilmiştir.
3.	Veri dönüşümü: Örneğin, EKG (ECG), kan basıncı (BP), nabız (PPG) gibi sinyal verileri, daha sonra kullanılmak üzere uygun veri yapılarına dönüştürülmüştür. Numpy'nin reshape fonksiyonu kullanılarak sinyal verileri sütun vektörlerine dönüştürülmüştür.
4.	Kayıp veri işleme: Bu kod örneğinde kayıp veri işlemi açıkça görülmemektedir. Ancak, kayıp verilerin nasıl işlendiği veya yerine konulduğu, veri yüklemesi veya veri dönüşümü adımlarının dışında gerçekleştirilmiş olabilir. Veri ön işleme adımlarının tamamının bu örnekte gösterilmediğini unutmayın, çünkü kodda tam olarak görünmeyebilir.
5. Hangi veri analizi ya da madencilik yöntemi, hangi amaçla uygulanmıştır?
Bu kod örneğinde, veri analizi ve makine öğrenimi yöntemleri kullanılarak kan basıncı (BP) verilerinin tahmin edilmesi amaçlanmıştır. İşlemlerin genel akışı aşağıdaki gibi olmuştur:
1.	Veri yüklenmiş ve boyutları kontrol edilmiştir.
2.	Veri öncesi işlemler yapılarak PPG (nabız), EKG (ECG) ve BP (kan basıncı) sinyal verileri uygun veri yapılarına dönüştürülmüştür.
3.	Veri analizi ve görselleştirme yapılmıştır. Örneğin, sinyal verileri grafiklerle gösterilmiş ve SBP (sistolik kan basıncı) ile DBP (diyastolik kan basıncı) değerleri karşılaştırılmıştır.
4.	Sinyaller arasındaki çapraz korelasyon hesaplanmış ve sonuçlar görselleştirilmiştir.
5.	Sinyal verileri üzerinde DCT (Discrete Cosine Transform) işlemi uygulanmıştır.
6.	Makine öğrenimi yöntemleri kullanılarak kan basıncı tahmini yapılmıştır. Linear Regression ve Random Forest Regressor modelleri kullanılmıştır. K-Fold Cross Validation ile modelin performansı değerlendirilmiştir.
7.	Ayrıca, derin öğrenme (neural network) kullanılarak da kan basıncı tahmini yapılmıştır. Birçok katmanlı sinir ağı (multi-layer perceptron) modeli oluşturulmuş ve eğitilmiştir.
8.	Son olarak, modelin performansı ölçülmüş ve hata değerleri hesaplanmıştır.
9.	Bu kod örneğindeki amaç, nabız (PPG) verilerini kullanarak kan basıncını tahmin etmek ve farklı makine öğrenimi yöntemlerinin performansını değerlendirmektir.
6. Hangi kütüphanelerden yararlanılmıştır?
Bu kodda aşağıdaki kütüphanelerden yararlanılmıştır:
numpy: Sayısal hesaplamalar için kullanılan bir kütüphane.
pandas: Veri manipülasyonu ve analizi için kullanılan bir kütüphane.
seaborn: Veri görselleştirmesi için kullanılan bir kütüphane.
scipy: Bilimsel hesaplama işlemleri ve MATLAB dosyalarını okumak için kullanılan bir kütüphane.
sklearn (scikit-learn): Makine öğrenimi modelleri ve metrikleri için kullanılan bir kütüphane.
sklearn.linear_model: Doğrusal regresyon modeli için 
sklearn.ensemble: Rastgele orman regresyon modeli için 
sklearn.model_selection: Çapraz doğrulama ve veri bölümlemesi için 
warnings: Uyarı mesajlarını yönetmek için kullanılan bir kütüphane.
matplotlib: Grafik çizimi ve görselleştirme için kullanılan bir kütüphane (matplotlib.pyplot).
os: Sistem işlemleri için kullanılan bir kütüphane.
Bu kütüphaneler, veri işleme, veri analizi, veri görselleştirme, makine öğrenimi modelleri ve sistem işlemleri gibi çeşitli işlemleri gerçekleştirmek için kullanılmıştır.





X.XX Hangi sonuçlara ulaşılmış? Sonuçlar nasıl ifade edilmiş (görsel, tablo,metin..)

 ![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/c13677f3-b895-44a9-a99d-a31da58b10e2)

##plotting sample ppg, ecg and bp signals
##using a sample size of 125
fig, ax = plt.subplots(3,1, figsize=(9,12), sharex=True)

ax[0].set_title('PPG graph', fontsize=16)
ax[0].set_ylabel('Signal Value')
ax[0].plot(ppg[:125])

ax[1].set_title('ECG graph', fontsize=16)
ax[1].set_ylabel('Signal Value')
ax[1].plot(ecg[:125])

ax[2].set_title('Blood Pressure (BP) graph', fontsize=16)
ax[2].set_ylabel('Signal Value')
ax[2].set_xlabel('Sample size')
ax[2].plot(bp[:125])


 















