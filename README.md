# Akıllı Bankacılık - Müşteri Kayıp (Churn) Tahmini Projesi

## Proje Hakkında
Bu proje, bir bankanın müşteri verilerini kullanarak müşterilerin bankayı terk etme (churn) olasılıklarını tahmin etmeyi amaçlayan bir veri bilimi çalışmasıdır. Makine öğrenmesi algoritmaları (LightGBM, XGBoost, CatBoost) kullanılarak müşterilerin davranışları analiz edilmiş ve riskli müşterilerin önceden tespit edilmesi hedeflenmiştir.

## Veri Seti ve Gizlilik Uyarısı
**Önemli:** Veri seti ING Hubs Türkiye Datathon kapsamında özel olarak sağlandığı için gizlilik nedeniyle paylaşılmamıştır. Projenin metodolojisi ve model çıktıları notebook içerisinde detaylandırılmıştır.

Kodları çalıştırmak için kendi veri setinizi veya benzer yapıdaki açık kaynak verileri kullanabilirsiniz. Kod yapısı, `load_data()` fonksiyonu sayesinde farklı veri kaynaklarına kolayca adapte edilebilir.

## Kullanılan Teknolojiler
- **Python**: Veri analizi ve modelleme dili.
- **Pandas & NumPy**: Veri manipülasyonu.
- **Matplotlib & Seaborn**: Veri görselleştirme.
- **Scikit-Learn**: Veri ön işleme ve metrik değerlendirme.
- **Boosting Algoritmaları**: LightGBM, XGBoost, CatBoost.

## Kurulum ve Çalıştırma
Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. **Gereksinimleri Yükleyin:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Notebook'u Çalıştırın:**
   `Smart_Banking_Churn_Prediction.ipynb` dosyasını Jupyter Notebook veya JupyterLab ile açarak hücreleri sırasıyla çalıştırın.
   > **Not:** Veri setinin `veri_bilimi_final_projesi` klasöründe veya Colab kullanıyorsanız Drive'da uygun yolda olduğundan emin olun.

## Proje Akışı
1. **Veri Yükleme ve Ön İşleme:** Eksik verilerin doldurulması, aykırı değer analizi.
2. **Özellik Mühendisliği (Feature Engineering):** Yeni özniteliklerin türetilmesi (örn. verimlilik oranları, yaş grupları).
3. **Modelleme:** Farklı algoritmaların eğitilmesi ve hiperparametre optimizasyonu.
4. **Değerlendirme:** Model performanslarının (ROC-AUC, Accuracy) karşılaştırılması.
5. **İş Görüsü ve Finansal Etki:** Modelin bankaya kazandıracağı potansiyel değerin analizi.

## Sonuç
Geliştirilen "Final Ensemble" modeli, tekil modellere göre daha kararlı ve yüksek başarı oranı (ROC-AUC ~0.75) sergilemiştir. Model, bankanın müşteri tutma stratejilerini optimize etmesine yardımcı olacak önemli içgörüler sunmaktadır.
