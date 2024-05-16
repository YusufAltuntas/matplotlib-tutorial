[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YusufAltuntas/matplotlib-tutorial/blob/main/matplotlib-turkce-dok%C3%BCmentasyon.ipynb#scrollTo=POmgIxkNmsOD)
![Logo](/matplotlibicon.jpg)


# **Matplotlib Eğitim Yol Haritamız:**

1. **Matplotlib Nedir ve Neden Kullanılır?** 

   - Matplotlib'in temel tanımı ve önemi
   - Veri görselleştirmenin önemi ve Matplotlib'in rolü

2. **Matplotlib Kurulumu**
   - Matplotlib'in kurulumu ve bağımlılıkları

3. **Temel Matplotlib Kavramları**
   - `Figure` ve `Axes` objeleri
   - Grafiklerin bileşenleri: başlık, eksen etiketleri, renkler, şekiller

4. **Temel Grafik Türleri**
   - Çizgi Grafikleri
   - Scatter (Nokta) Grafikleri
   - Bar (Sütun) Grafikleri
   - Histogramlar
   - Pasta Grafikleri

5. **Grafiklerin Özelleştirilmesi**
   - Renkler ve renk paletleri
   - Çizgi stilleri ve genişlikleri
   - Eksenlerin özelleştirilmesi: etiketler, aralıklar, dönüşler
   - Grafik boyutları ve çözünürlük

6. **Birden Fazla Grafik**
   - Birden fazla alt grafik oluşturma: subplot'lar
   - Grafiklerin yan yana veya üst üste yerleştirilmesi

7. **Metin ve Annotasyon Ekleme**
   - Grafiklere metin ekleme
   - Önemli noktaları vurgulamak için annotasyonlar kullanma

8. **Grafiklerin Kaydedilmesi**
   - Grafiklerin farklı dosya formatlarında kaydedilmesi (PNG, JPEG, PDF)

9. **Grafiklerin İleri Seviye Özellikleri**
   - Renk haritaları ve renk ölçekleri
   - 3D Grafikler
   - Animasyonlar

10. **Gerçek Dünya Uygulamaları ve Örnekler**
    - Gerçek veri setlerinin görselleştirilmesi
    - Bilimsel verilerin görselleştirilmesi
    - İşleme verileri görselleştirme

**Uygulama ve Proje:**
- Matplotlib kullanarak bir veri setini görselleştirme ve analiz etme projesi

Bu yol haritası, Matplotlib'i temel seviyeden ileri seviyeye kadar öğrenmenizi sağlayacak adımları içerir. Her bir konuyu anlamak ve uygulamak için örneklerle desteklenmiş detaylı bir açıklama sağlanacaktır. Hazırsanız, ilk konuya, "Matplotlib Nedir ve Neden Kullanılır?" başlayabiliriz.

## **1) Matplotlib Nedir ve Neden Kullanılır?**

Matplotlib, Python programlama dilinde güçlü ve esnek veri görselleştirme araçları sağlayan bir kütüphanedir. Bilimsel ve mühendislik uygulamalarından, veri analizine, web uygulamalarından eğitim materyallerine kadar geniş bir kullanım alanına sahiptir. İşte Matplotlib'in ana özellikleri ve neden kullanılması gerektiği hakkında birkaç önemli nokta:

1. **Esneklik ve Güçlü Özellikler:** Matplotlib, çeşitli grafik türlerini oluşturmak için kapsamlı bir araç seti sunar. Basit çizgi grafiklerinden karmaşık 3D grafiklere kadar geniş bir yelpazede grafikler oluşturabilirsiniz.

2. **Platform Bağımsızlık:** Matplotlib, Linux, Windows ve macOS gibi farklı işletim sistemlerinde çalışabilir. Bu, geliştirme sürecinde ve uygulamaların dağıtımında büyük bir esneklik sağlar.

3. **Geniş Kullanıcı Tabanı ve Topluluk Desteği:** Matplotlib, geniş bir kullanıcı tabanına sahiptir ve bu da belgelendirme, yardım forumları ve örnek kodlar açısından zengin bir topluluğun varlığı anlamına gelir. Bu topluluk sayesinde sorunlarınıza hızlıca çözüm bulabilir ve yeni teknikler öğrenebilirsiniz.

4. **Duyarlılık:** Matplotlib, interaktif grafikler oluşturmak için kullanılabilir. Bu, veri analizi ve görselleştirme iş akışınızı daha etkileşimli hale getirir ve verilerinizin daha derinlemesine keşfedilmesini sağlar.

5. **Genişletilebilirlik:** Matplotlib, temel işlevselliğini genişletmek için birçok eklenti ve araç içerir. Örneğin, çeşitli veri analizi kütüphaneleriyle entegrasyonu kolaylaştıran ek paketler bulunmaktadır.

Matplotlib'in bu özellikleri, veri görselleştirme süreçlerinizde size büyük bir esneklik ve güç sağlar. Şimdi, Matplotlib'in nasıl kurulacağını öğrenmek için bir sonraki adıma geçebiliriz.

## 2) **Kütüphane Kurulumu**

Matplotlib.pyplot modülü, Matplotlib kütüphanesinin en yaygın kullanılan araçlarından biridir. Bu modülü kullanarak grafikleri oluşturabilir, özelleştirebilir ve görselleştirebiliriz. Şimdi, Matplotlib.pyplot modülünün kurulumunu ele alalım:

1. **Matplotlib.pyplot Modülünün Kurulumu:**

   Matplotlib.pyplot modülünü kurmak için, öncelikle Python ve pip kurulu olmalıdır. Python kurulu değilse [Python'un resmi web sitesinden](https://www.python.org/downloads/) en son sürümü indirip kurabilirsiniz. 

   Ardından, Matplotlib.pyplot modülünü kurmak için terminal veya komut istemcisinde şu komutu çalıştırın:

   ```
   pip install matplotlib
   ```

   Bu komut, Matplotlib kütüphanesini ve Matplotlib.pyplot modülünü yükleyecektir.

2. **Kurulumun Kontrol Edilmesi:**

   Matplotlib.pyplot modülünün başarıyla kurulduğunu doğrulamak için Python etkileşimli kabuğunu (Python REPL) veya bir Jupyter Notebook açabilir ve aşağıdaki komutları kullanarak kontrol edebilirsiniz:

   ```python
   import matplotlib.pyplot as plt
   print(plt.__version__)
   ```

   Bu komut, yüklü Matplotlib sürümünü yazdıracaktır.

Matplotlib.pyplot modülünün başarıyla kurulduğunu gördüğünüzde, artık bu modülü kullanarak veri görselleştirmesi yapmaya başlayabilirsiniz. Şimdi, Jupyter Notebook'ta örnek kodlarla uygulamalı öğrenme adımına geçebiliriz.

## 3. **Temel Matplotlib Kavramları**
   - `Figure` ve `Axes` objeleri
   - Grafiklerin bileşenleri: başlık, eksen etiketleri, renkler, şekiller

### **3.1 `Figure` ve `Axes` Objeleri:**

- **Figure (Şekil)**: Bir figür, Matplotlib'de oluşturulan tüm grafiklerin temel konteyneridir. Yani, bir figür, grafik penceresini veya çıktı alanını temsieder. Bir figür, birden çok alt grafik (axes) içerebilir ve bu alt grafikler figürün içinde konumlandırılır. Genellikle, bir figür oluşturulduğunda, üzerinde çalışılacak alt grafiklerin yerleştirileceği bir çerçeve sağlar.

- **Axes (Eksenler)**: Axes, bir figür içindeki tek bir grafik alanını temsil eder. Bu, verilerin çizildiği ve manipüle edildiği ana alandır. Axes, x eksenini (yatay), y eksenini (dikey) ve isteğe bağlı olarak z eksenini içerebilir. Axes içinde veri görselleştirmesi oluşturmak için çeşitli fonksiyonlar kullanılabilir. Örneğin, çizgi grafiği çizmek için `plot()` veya histogram oluşturmak için `hist()` fonksiyonları kullanılabilir.

**!!!** Figür bir fotoğraf çerçevesi, axes'ler de çerçevenin içine koyulacak fotoğraflardır. Basitçe böyle anlatabiliriz.

![Figure ve Axes Objeleri](https://www.earthdatascience.org/images/earth-analytics/plot-data/fig-1-plot.png)


```python
import matplotlib.pyplot as plt

# Bir Figure oluşturma
fig = plt.figure()

# Bir Axes oluşturma ve bu Axes'i Figure içine yerleştirme
ax = fig.add_subplot(111)  # 1 satır, 1 sütun, 1. subplot
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_6_0.png)
    



```python
# Figür boyutunu figsize parametresi ile ayarlıyoruz. Varsayılan olarak 640x480 dir
plt.figure()
plt.figure(figsize=(12, 8))
plt.show()
```


    <Figure size 640x480 with 0 Axes>



    <Figure size 1200x800 with 0 Axes>


### **3.2 Grafiklerin Bileşenleri: Başlık, Eksen Etiketleri, Renkler, Şekiller:**
  - **Başlık (Title):**
    - Grafik başlığı, grafiğin içeriğini açıklayan metin.
    - `plt.title()` fonksiyonu ile eklenir.
  - **Eksen Etiketleri (Axis Labels):**
    - X ve Y eksenlerinin adlarıdır.
    - `plt.xlabel()` ve `plt.ylabel()` fonksiyonları ile eklenir.
  - **Eksenler (Axes):**
    - Grafikte verilerin yer aldığı koordinat düzlemleri.
    - X ve Y eksenleri, veri aralığını gösterir.
    - `plt.xlim()` ve `plt.ylim()` fonksiyonları ile eksen aralıklarbelirlenebilir.
  - **Renkler (Colors):**
    - Grafikteki çizgi, nokta, sütun, alan vb. öğelerin renkleri.
    - Renkler genellikle hexadecimal kodlarla veya renk isimleriyle belirtilir.
    
     Matplotlib'te kullanılabilecek renk kodları şunlardır:
    - 'b' : mavi (blue)
    - 'g' : yeşil (green)
    - 'r' : kırmızı (red)
    - 'c' : turkuaz (cyan)
    - 'm' : magenta
    - 'y' : sarı (yellow)
    - 'k' : siyah (black)
    - 'w' : beyaz (white)
 
Bu renk kodları, Matplotlib'te çeşitli grafiklerin renklerini belirtmek için kullanılabilir.
  - **Şekiller (Shapes):**
    - Özel şekiller, grafikte belirli noktalara veya aralıklara vurgu yapmak için kullanılabilir.
    - Örneğin, `plt.fill_between()` veya `plt.annotate()` fonksiyonlarıyla eklenir.
    - Not: Bu aslında matplotlib.pyplot'ta doğrudan bir kavram değildir, ancak çeşitli fonksiyonlarla grafiğe şekil ekleyebiliriz.


```python
import matplotlib.pyplot as plt

# Veri oluşturma
x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

# Bir Figure oluşturma
fig = plt.figure()

# Bir Axes oluşturma ve bu Axes'i Figure içine yerleştirme
ax = fig.add_subplot(111)  # 1 satır, 1 sütun, 1. subplot

# Veriyi çizme
ax.plot(x, y, color='blue')

# Başlık ve eksen etiketlerini ekleme
ax.set_title('Çizgi Grafiği Örneği')
ax.set_xlabel('X Ekseni')
ax.set_ylabel('Y Ekseni')

plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_9_0.png)
    


## **4) Temel Grafik Türleri**

### **4.1 Çizgi (plot) Grafikleri:**
   - **Tanım:** Çizgi grafikleri, veri noktaları arasındaki ilişkiyi görselleştirmek için kullanılır. Basitçe, veri noktaları bir çizgiyle birbirine bağlanır ve bu çizgi, veri setindeki değerler arasındaki ilişkiyi görsel olarak temsil eder. Çizgi grafiği oluşturmak için plt.plot() fonksiyonu kullanılır.
   
   - **Syntax:**
     ```python
     plt.plot(x, y, linestyle='-', color='blue', marker='o', markersize=5)
     ```
   - **Parametreler:**
     - `x`: X eksenindeki veri noktaları.
     - `y`: Y eksenindeki veri noktaları.
     - `linestyle`: Çizgi stili (örneğin, '-', '--', ':', '-.').
     - `color`: Çizgi rengi.
     - `marker`: Nokta işareti tipi.
     - `markersize`: Nokta işareti boyutu.


```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

plt.plot(x, y, linestyle='-', color='blue', marker='o', markersize=5)
plt.title('Çizgi Grafik Örneği')
plt.xlabel('X Ekseni')
plt.ylabel('Y Ekseni')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_12_0.png)
    


### **4.2 Scatter (Nokta) Grafikleri:**
   - **Tanım:** Nokta grafikleri, iki değişken arasındaki ilişkiyi görselleştirmek için kullanılır.
   - **Syntax:**
     ```python
     plt.scatter(x, y, color='red', marker='o', s=50)
     ```
   - **Parametreler:**
     - `x`: X eksenindeki veri noktaları.
     - `y`: Y eksenindeki veri noktaları.
     - `color`: Nokta rengi.
     - `marker`: Nokta işareti tipi.
     - `s`: Nokta boyutu.
     - `edgecollors`: Noktaların kenar rengi.
     - `alpha`: Saydamlık ve opaklık.

Scatter grafiğinde kullanabileceğiniz çeşitli markerlar (işaretleyiciler) vardır ve bu markerlar veri noktalarını temsil etmek için kullanılır. Matplotlib kütüphanesinde, scatter grafiği çiziminde kullanılabilen bazı yaygın marker türleri şunlardır:

1. **'o'**: Yuvarlak marker. Veri noktalarını yuvarlak şekilde işaretler.

2. **'s'**: Kare marker. Veri noktalarını kare şeklinde işaretler.

3. **'^'**: Üçgen marker. Veri noktalarını üçgen şeklinde işaretler.

4. **'D'**: Elmas marker. Veri noktalarını elmas şeklinde işaretler.

5. **'+'**: Artı işareti marker. Veri noktalarını artı işareti şeklinde işaretler.

6. **'x'**: Çarpı işareti marker. Veri noktalarını çarpı işareti şeklinde işaretler.

7. **'.'**: Nokta marker. Veri noktalarını küçük nokta olarak işaretler.

8. **','**: Virgül marker. Veri noktalarını küçük virgül olarak işaretler.  


```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

plt.scatter(x, y, color='red', marker='o', s=50)
plt.title('Nokta Grafik Örneği')
plt.xlabel('X Ekseni')
plt.ylabel('Y Ekseni')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_14_0.png)
    


### **4.3 Bar (Sütun) Grafikleri:**
   - **Tanım:** Sütun grafikleri, kategorik verilerin karşılaştırılmasında kullanılır. Her bir sütun, farklı kategorileri veya grupları temsil eder.
   - **Syntax:**
     ```python
     plt.bar(categories, values, color='green')
     ```
   - **Parametreler:**
     - `categories`: Sütunların kategorileri.
     - `values`: Her bir kategorinin değerleri.
     - `color`: Sütun rengi.
     - `width`: Sütun genişliğini kontrol eder.
     - `edgecolor`: Sütunların kenarlık rengini belirler.
     - `linewidth`: Sütunların kenarlık kalınlığını belirler.


```python
import matplotlib.pyplot as plt

categories = ['A', 'B', 'C', 'D', 'E']
values = [10, 15, 7, 10, 5]

plt.bar(categories, values, color='green', width=0.8 , edgecolor="blue")
plt.title('Sütun Grafik Örneği')
plt.xlabel('Kategoriler')
plt.ylabel('Değerler')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_16_0.png)
    


* Bölgelere göre satış miktarını gösteren bir "bar" grafiği oluşturalım.


```python
import numpy as np
import pandas as pd
np.random.seed(0)

data = {
    "Yil": np.arange(2010, 2021),
    "Satiş": np.random.randint(100, 500, 11),
    "Masraf": np.random.randint(50,400, 11)
}

df = pd.DataFrame(data)

regions = ["Kuzey", "Güney", "Doğu", "Bati"]
df["Bölge"] = np.random.choice(regions, df.shape[0])
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Yil</th>
      <th>Satiş</th>
      <th>Masraf</th>
      <th>Bölge</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2010</td>
      <td>272</td>
      <td>292</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2011</td>
      <td>147</td>
      <td>342</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2012</td>
      <td>217</td>
      <td>137</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2013</td>
      <td>292</td>
      <td>120</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2014</td>
      <td>423</td>
      <td>138</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2015</td>
      <td>351</td>
      <td>364</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2016</td>
      <td>295</td>
      <td>243</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>7</th>
      <td>2017</td>
      <td>459</td>
      <td>89</td>
      <td>Bati</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2018</td>
      <td>109</td>
      <td>137</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>9</th>
      <td>2019</td>
      <td>311</td>
      <td>224</td>
      <td>Bati</td>
    </tr>
    <tr>
      <th>10</th>
      <td>2020</td>
      <td>377</td>
      <td>138</td>
      <td>Güney</td>
    </tr>
  </tbody>
</table>
</div>




```python
sales_by_region = df.groupby("Bölge")["Satiş"].sum()
sales_by_region
```




    Bölge
    Bati      770
    Güney    1656
    Kuzey     827
    Name: Satiş, dtype: int32




```python

plt.bar(sales_by_region.index, sales_by_region.values,color='green', width=0.8 , edgecolor="blue")
plt.xlabel("Bölge",  fontsize=12,  fontweight="bold",  color="black")
plt.ylabel("Tutar",  fontsize=12, fontweight="bold" , color="black")
plt.title("Bölgelerin Toplam Satışı")
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_20_0.png)
    


### **4.4 Histogramlar:**
   - **Tanım:** Histogramlar, sayısal verilerin dağılımını görselleştirmek için kullanılır. Verinin frekansını göstermek için kullanılır.
   - **Syntax:**
     ```python
     plt.hist(data, bins=20, color='purple')
     ```
   - **Parametreler:**
     - `data`: Histogramı oluşturacak veri.
     - `bins`: Histogramdaki çubuk sayısı.
     - `color`: Histogram rengi.
     - `histtype`: Histogram tipini belirtir. "bar", "barstacked", "step", "stepfilled" olabilir.
     - `range`: Bin'lerin alt ve üst sınırını belirler.
     - `density`: Histogram grafiğindeki çubukların yüksekliklerinin değil, toplam alanın 1'e eşit olduğu bir yoğunluk grafiği oluşturulmasını sağlar. Bu, veri dağılımının daha doğru bir şekilde temsil edilmesini sağlar ve farklı histogramların daha kolay karşılaştırılmasına olanak tanır. True olursa grafik yoğunluk belirtir, False olursa frekans belirtir. 


```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.randn(1000)  # Rastgele veri oluşturma
plt.hist(data, bins=15, color='purple')
plt.title('Histogram Örneği')
plt.xlabel('Değerler')
plt.ylabel('Frekans')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_22_0.png)
    


* Satışların frekansını gösteren bir histogram çizelim.


```python
import numpy as np
import pandas as pd
np.random.seed(0)

data = {
    "Yil": np.arange(2010, 2021),
    "Satiş": np.random.randint(100, 500, 11),
    "Masraf": np.random.randint(50,400, 11)
}

df = pd.DataFrame(data)

regions = ["Kuzey", "Güney", "Doğu", "Bati"]
df["Bölge"] = np.random.choice(regions, df.shape[0])
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Yil</th>
      <th>Satiş</th>
      <th>Masraf</th>
      <th>Bölge</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2010</td>
      <td>272</td>
      <td>292</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2011</td>
      <td>147</td>
      <td>342</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2012</td>
      <td>217</td>
      <td>137</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2013</td>
      <td>292</td>
      <td>120</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2014</td>
      <td>423</td>
      <td>138</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2015</td>
      <td>351</td>
      <td>364</td>
      <td>Güney</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2016</td>
      <td>295</td>
      <td>243</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>7</th>
      <td>2017</td>
      <td>459</td>
      <td>89</td>
      <td>Bati</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2018</td>
      <td>109</td>
      <td>137</td>
      <td>Kuzey</td>
    </tr>
    <tr>
      <th>9</th>
      <td>2019</td>
      <td>311</td>
      <td>224</td>
      <td>Bati</td>
    </tr>
    <tr>
      <th>10</th>
      <td>2020</td>
      <td>377</td>
      <td>138</td>
      <td>Güney</td>
    </tr>
  </tbody>
</table>
</div>




```python
# satiş miktarları aralıklarını kategorik olarak ayırır. her satış miktarı aralığında eşit değer olur. 
sales_bins = pd.qcut(df["Satiş"], q=10)
bin_counts = sales_bins.value_counts()
bin_counts.sort_index()
```




    Satiş
    (108.999, 147.0]    2
    (147.0, 217.0]      1
    (217.0, 272.0]      1
    (272.0, 292.0]      1
    (292.0, 295.0]      1
    (295.0, 311.0]      1
    (311.0, 351.0]      1
    (351.0, 377.0]      1
    (377.0, 423.0]      1
    (423.0, 459.0]      1
    Name: count, dtype: int64




```python
# grafiğe koymak içim aralıkların sağdaki ve soldaki değerlerinin orta noktasını alır.
orta_nokta = [(aralik.left + aralik.right) / 2 for aralik in bin_counts.index]
orta_nokta
```




    [127.9995, 182.0, 244.5, 282.0, 293.5, 303.0, 331.0, 364.0, 400.0, 441.0]




```python
plt.hist(df["Satiş"], bins=10, alpha=0.5, color="blue", label="Satışların Frekansı", width=20)
plt.legend()
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_27_0.png)
    


* density parametresini kullanarak yoğunluğu gösterelim.


```python
plt.hist(df["Satiş"], bins=10, alpha=0.5, color="blue", label="Satışların Frekansı", width=20, density=True)
plt.legend()
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_29_0.png)
    


### **4.5 Kutu Grafikleri:**

   - **Tanım:** Kutu grafikleri, veri dağılımının istatistiksel özetini göstermek için kullanılır. Verinin çeyrekliklerini, medyanı, minimum ve maksimum değerleri gösterir.
   - **Syntax:**
     ```python
     plt.boxplot(data, notch=True, vert=False, patch_artist=True)
     ```
   - **Parametreler:**
     - `data`: Kutu grafik oluşturmak için kullanılacak veri.
     - `notch`: Kutunun ortasındaki çıkıntıların olup olmayacağı.
     - `vert`: Dikey veya yatay kutu grafiği oluşturulacağı (True: dikey, False: yatay).
     - `patch_artist`: Kutunun içini renklendirmek için (True: renklendir, False: renklendirme yapma).


```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.randn(100)  # Rastgele veri oluşturma
plt.boxplot(data, notch=True, vert=False, patch_artist=True)
plt.title('Kutu Grafik Örneği')
plt.ylabel('Değerler')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_31_0.png)
    


### **4.6 Pasta Grafikleri:**

   - **Tanım:** Pasta grafikleri, bir bütünün parçalarının oransal dağılımını göstermek için kullanılır. Her bir dilim, bütünün yüzdesini temsil eder.
   - **Syntax:**
     ```python
     plt.pie(sizes, labels=labels, autopct='%1.1f%%', startangle=90, colors=['red', 'green', 'blue'])
     ```
   - **Parametreler:**
     - `sizes`: Pasta dilimlerinin büyüklükleri.
     - `labels`: Pasta dilimlerinin etiketleri.
     - `autopct`: Pasta dilimlerinin yüzdesini göstermek için formatlama.
     - `startangle`: İlk dilimin başlangıç açısı (saat yönünde derece cinsinden).
     - `colors`: Pasta dilimlerinin renkleri.


```python
import matplotlib.pyplot as plt

sizes = [25, 30, 15, 10, 20]
labels = ['A', 'B', 'C', 'D', 'E']

plt.pie(sizes, labels=labels, autopct='%1.1f%%', startangle=90, colors=['red', 'green', 'blue'])
plt.title('Pasta Grafik Örneği')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_33_0.png)
    



```python
import matplotlib.pyplot as plt

sizes = [25, 30, 15, 10, 20]
labels = ['A', 'B', 'C', 'D', 'E']

plt.pie(sizes, labels=labels, autopct='%1.1f%%')
plt.title('Pasta Grafik Örneği')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_34_0.png)
    


### **4.7 Alan Dolgulu Grafikler:**

   - **Tanım:** Alan dolgulu grafikler, zamanla değişen verinin belirli bir aralıktaki değişimini vurgulamak için kullanılır. Bir çizginin altını renkli bir alana doldurarak oluşturulur.
   - **Syntax:**
     ```python
     plt.fill_between(x, y1, y2, color='skyblue', alpha=0.5)
     ```
   - **Parametreler:**
     - `x`: X eksenindeki veri noktaları.
     - `y1`: Dolgu alanının alt sınırını belirleyen veri.
     - `y2`: Dolgu alanının üst sınırını belirleyen veri.
     - `color`: Dolgu alanının rengi.
     - `alpha`: Dolgu alanının opaklığı.

- Pasta grafikleri, veri setindeki kategorik oranları net bir şekilde görselleştirmek için kullanılırken, alan dolgulu grafikler ise zamana bağlı olarak değişen veri setlerinin aralıklarını vurgulamak için kullanılabilir. Bu grafik türleri, farklı veri analiz ihtiyaçlarına göre kullanılarak verinin anlaşılmasını kolaylaştırır.


```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y1 = [1, 3, 5, 7, 9]
y2 = [0, 2, 4, 6, 8]

plt.fill_between(x, y1, y2, color='skyblue', alpha=0.5)
plt.title('Alan Dolgulu Grafik Örneği')
plt.xlabel('X Ekseni')
plt.ylabel('Y Ekseni')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_36_0.png)
    


## **5) Grafiklerin Özelleştirilmesi:**

Grafiklerin özelleştirilmesi, veri görselleştirmenin önemli bir parçasıdır ve matplotlib.pyplot kütüphanesi bu konuda geniş bir esneklik sunar. İşte grafiklerin özelleştirilmesi için kullanılan bazı temel teknikler:

1. **Renkler ve Stiller:**
   - Grafiklerde kullanılan çizgi, nokta, sütun gibi öğelerin renklerini ve stillerini belirlemek için kullanılır.
   - Örneğin, `color` parametresiyle rengi belirlenir, `linestyle` parametresiyle çizgi stili (örneğin '-', '--', ':', '-.') belirlenir.
   - Örnek:
     ```python
     plt.plot(x, y, color='blue', linestyle='--')
     ```

2. **Başlık ve Eksen Etiketleri:**
   - Grafiklerin başlığını ve eksen etiketlerini belirlemek için kullanılır.
   - Örneğin, `plt.title()` fonksiyonu ile başlık eklenir, `plt.xlabel()` ve `plt.ylabel()` fonksiyonları ile x ve y eksenlerine etiketler eklenir.
   - Örnek:
     ```python
     plt.title('Örnek Grafik')
     plt.xlabel('X Ekseni')
     plt.ylabel('Y Ekseni')
     ```

3. **Eksen Aralıkları ve Ölçekler:**
   - Grafikte gösterilen eksen aralıklarını ve ölçekleri belirlemek için kullanılır.
   - Örneğin, `plt.xlim()` ve `plt.ylim()` fonksiyonları ile x ve y eksenlerinin aralıkları belirlenebilir.
   - Örnek:
     ```python
     plt.xlim(0, 10)
     plt.ylim(0, 100)
     ```

4. **Grafik Boyutu ve Çözünürlük:**
   - Oluşturulan grafik figürünün boyutunu ve çözünürlüğünü belirlemek için kullanılır.
   - Örneğin, `plt.figure(figsize=(8, 6))` ile grafik boyutu belirlenebilir.
   - Örnek:
     ```python
     plt.figure(figsize=(10, 8), dpi=100)
     ```

5. **Arka Plan ve Çerçeve:**
   - Grafik arka planının ve çerçevesinin özelliklerini belirlemek için kullanılır.
   - Örneğin, `plt.grid()` fonksiyonu ile ızgarayı ekleyebiliriz.
   - Örnek:
     ```python
     plt.grid(True, linestyle='--', color='gray', alpha=0.5)
     ```

6. **Metin ve Annotasyonlar:**
   - Grafik üzerine metin veya annotasyonlar eklemek için kullanılır.
   - Örneğin, `plt.text()` ile metin ekleyebiliriz, `plt.annotate()` ile annotasyon ekleyebiliriz.
   - Örnek:
     ```python
     plt.text(2, 20, 'Örnek Metin', fontsize=12, color='red')
     plt.annotate('Annotasyon', xy=(3, 30), xytext=(4, 40),
                  arrowprops=dict(facecolor='blue', arrowstyle='->'))
     ```

Bu özellikler, matplotlib.pyplot kütüphanesinin kullanıcıya sunduğu grafiklerin detaylı bir şekilde özelleştirilmesini sağlar. Yukarıdaki örneklerle birlikte bu özellikleri kullanarak grafiklerinizi istediğiniz gibi şekillendirebilirsiniz.

## **6. Birden Fazla Grafik:**

   - **Birden Fazla Alt Grafik Oluşturma: subplot'lar**
     - subplot'lar, bir figür içinde birden fazla alt grafik oluşturmak için kullanılır.
     - subplot'lar, satır ve sütun sayısı ile belirlenen bir düzen içinde yer alırlar.
     - `plt.subplot()` veya `fig.add_subplot()` fonksiyonları ile oluşturulur.

   - **Grafiklerin Yan Yana veya Üst Üste Yerleştirilmesi:**
     - subplot'lar, yan yana veya üst üste yerleştirilerek farklı düzenler elde edilebilir.
     - Bu, `plt.subplots()` veya `fig.add_subplot()` fonksiyonlarına verilen parametrelerle belirlenir.

#### **Alt Grafik Oluşturma:**


```python
import matplotlib.pyplot as plt

# 2x2'lik bir alt grafik düzeni oluşturma
fig, axes = plt.subplots(nrows=2, ncols=2)

# İstenen alt grafiklere erişim ve işlem yapma
axes[0, 0].plot([1, 2, 3], [4, 5, 6])  # 1. satır, 1. sütun
axes[0, 1].scatter([1, 2, 3], [4, 5, 6])  # 1. satır, 2. sütun
axes[1, 0].bar(['A', 'B', 'C'], [10, 15, 20])  # 2. satır, 1. sütun
axes[1, 1].pie([25, 35, 40], labels=['X', 'Y', 'Z'])  # 2. satır, 2. sütun

# İstenmeyen ekseni ve boşlukları kaldırma
fig.tight_layout()

plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_40_0.png)
    


Yukarıdaki örnekte, `plt.subplots()` fonksiyonu ile 2x2'lik bir alt grafik düzeni oluşturulur. Oluşturulan `fig` ve `axes` nesneleri kullanılarak her bir alt grafik üzerinde çizimler yapılır.

`plt.subplot()` veya `fig.add_subplot()` fonksiyonları ile de tek tek alt grafikler oluşturulabilir:

Bu kod, Matplotlib kütüphanesini kullanarak 2x2'lik bir alt grafik düzeni oluşturur ve her bir alt grafikte farklı türde veri görselleştirmesi yapar. İşte kodun adım adım açıklaması:

1. `import matplotlib.pyplot as plt`: Matplotlib kütüphanesini `plt` takma adıyla içe aktarır.

2. `fig, axes = plt.subplots(nrows=2, ncols=2)`: 2x2'lik bir alt grafik düzeni oluşturur. `fig` ana figürü, `axes` ise alt grafikleri temsil eden bir dizi (matris) oluşturur. `nrows` ve `ncols` parametreleri, sırasıyla satır ve sütun sayısını belirtir.

3. `axes[0, 0].plot([1, 2, 3], [4, 5, 6])`: İlk alt grafikte bir çizgi grafiği oluşturur. `axes[0, 0]`, 1. satır ve 1. sütundaki alt grafik alanına erişimi sağlar. `plot()` fonksiyonu, x ve y değerleri verilen veri setini çizer.

4. `axes[0, 1].scatter([1, 2, 3], [4, 5, 6])`: İkinci alt grafikte bir dağılım grafiği oluşturur. `scatter()` fonksiyonu, verilen x ve y değerlerine sahip noktaları dağılım grafiği olarak çizer.

5. `axes[1, 0].bar(['A', 'B', 'C'], [10, 15, 20])`: Üçüncü alt grafikte bir sütun grafiği oluşturur. `bar()` fonksiyonu, x ve y değerlerini belirterek sütun grafiğini çizer.

6. `axes[1, 1].pie([25, 35, 40], labels=['X', 'Y', 'Z'])`: Dördüncü alt grafikte bir pasta grafiği oluşturur. `pie()` fonksiyonu, dilimlerin büyüklüğünü belirlemek için verilen değerleri kullanır ve dilim etiketlerini `labels` parametresiyle belirler.

7. `fig.tight_layout()`: Alt grafikler arasındaki boşlukları minimize eder ve grafiklerin daha düzenli görünmesini sağlar.

8. `plt.show()`: Oluşturulan grafikleri gösterir.


```python
import matplotlib.pyplot as plt

# İlk alt grafik oluşturma
plt.subplot(2, 1, 1)  # 2 satır, 1 sütun, 1. alt grafik
plt.plot([1, 2, 3], [4, 5, 6])

# İkinci alt grafik oluşturma
plt.subplot(2, 1, 2)  # 2 satır, 1 sütun, 2. alt grafik
plt.scatter([1, 2, 3], [4, 5, 6])

plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_42_0.png)
    


Bu örnekte `plt.subplot()` fonksiyonu ile 2 satırlı ve 1 sütunlu bir düzende, ilk olarak bir çizgi grafiği ve sonra bir nokta grafiği oluşturulur.

## **7. Metin ve Annotasyon Ekleme:**

   - **Grafiklere Metin Ekleme:**
     - Grafiklere metin eklemek, grafiklerdeki belirli bilgileri açıklamak veya başlıkları vurgulamak için kullanışlıdır.
     - Metin eklemek için `plt.text()` veya `ax.text()` fonksiyonları kullanılabilir.
     - **Syntax:**
       ```python
       plt.text(x, y, 'Metin', fontsize=12, color='blue')
       ```
     - **Parametreler:**
       - `x` ve `y`: Metnin konumunu belirten koordinatlar.
       - `'Metin'`: Eklemek istenen metin.
       - `fontsize`: Metin boyutu.
       - `color`: Metin rengi.


```python
import matplotlib.pyplot as plt

plt.plot([1, 2, 3], [2, 3, 5])
plt.text(2, 4, 'Bu bir metindir', fontsize=12, color='blue')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_45_0.png)
    


   - **Önemli Noktaları Vurgulamak için Annotasyonlar:**
     - Annotasyonlar, grafikteki belirli bir noktayı veya aralığı vurgulamak için kullanılır.
     - `plt.annotate()` veya `ax.annotate()` fonksiyonları kullanılarak eklenir.
     - **Syntax:**
       ```python
       plt.annotate('Açıklama', xy=(x, y), xytext=(x_text, y_text), arrowprops=dict(facecolor='red', arrowstyle='->'))
       ```
     - **Parametreler:**
       - `'Açıklama'`: Annotasyon metni.
       - `xy`: Annotasyonun ekleneceği noktanın koordinatları.
       - `xytext`: Metnin ekleneceği noktanın koordinatları.
       - `arrowprops`: Ok özelliklerini belirten bir sözlük.


```python
import matplotlib.pyplot as plt

plt.plot([1, 2, 3], [2, 3, 5])
plt.annotate('Önemli Nokta', xy=(2, 3), xytext=(2.5, 3.5),
            arrowprops=dict(facecolor='red', arrowstyle='->'))
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_47_0.png)
    


## **8. Grafiklerin Kaydedilmesi:**

- **Grafiklerin Farklı Dosya Formatlarında Kaydedilmesi:**
  - Oluşturduğumuz grafikleri farklı dosya formatlarında kaydetmek, grafikleri paylaşmak veya yayınlamak için önemlidir.
  - `plt.savefig()` fonksiyonu kullanılarak grafik dosyaya kaydedilir.


```python
import matplotlib.pyplot as plt

# Örnek veri
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

# Grafik oluşturma
plt.plot(x, y)
plt.title('Örnek Grafik')
plt.xlabel('X Ekseni')
plt.ylabel('Y Ekseni')

# Grafik dosyaya kaydetme
plt.savefig('ornek_grafik.png', dpi=300)  # PNG formatında kaydetme
plt.savefig('ornek_grafik.jpg', dpi=300)  # JPEG formatında kaydetme
plt.savefig('ornek_grafik.pdf')           # PDF formatında kaydetme

plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_49_0.png)
    


**Parametreler:**
- `'ornek_grafik.png'`, `'ornek_grafik.jpg'`, `'ornek_grafik.pdf'`: Kaydedilecek dosyanın adı ve uzantısı.
- `dpi`: Çözünürlük (dots per inch), varsayılan değer genellikle yeterlidir, ancak gerektiğinde ayarlanabilir.

Bu şekilde, oluşturduğumuz grafikleri farklı dosya formatlarında kaydetmeyi öğrendik. Grafiklerimizi PNG, JPEG veya PDF olarak kaydederek, ihtiyacımıza göre paylaşabilir veya kullanabiliriz.

## **9. Grafiklerin İleri Seviye Özellikleri:**

#### - **Renk Haritaları ve Renk Ölçekleri:**
  - Renk haritaları, veri değerlerini renklerle ilişkilendirmek için kullanılır ve genellikle 2D veya 3D görüntülerde kullanılır.
  - `plt.imshow()` veya `ax.imshow()` fonksiyonları kullanılarak renk haritası uygulanır.


```python
import matplotlib.pyplot as plt
import numpy as np

# Örnek veri oluşturma
data = np.random.rand(10, 10)

# Renk haritası ile veriyi görselleştirme
plt.imshow(data, cmap='viridis')
plt.colorbar()  # Renk ölçeği ekleme
plt.title('Renk Haritası Örneği')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_52_0.png)
    


Kodun detaylı açıklaması:

1. `import matplotlib.pyplot as plt`: Matplotlib kütüphanesini plt takma adıyla içe aktarır. Bu, Matplotlib'in pyplot modülünü kullanarak veri görselleştirmesi yapmamıza olanak tanır.

2. `import numpy as np`: Numpy kütüphanesini np takma adıyla içe aktarır. Bu, rastgele veri oluşturmak için kullanacağımız NumPy dizilerine erişmemize olanak tanır.

3. `data = np.random.rand(10, 10)`: 10x10 boyutunda bir NumPy dizisi oluşturur. Bu dizi, 0 ile 1 arasında rastgele sayılardan oluşur. Yani, `rand()` fonksiyonu, belirtilen boyutta rastgele sayılardan oluşan bir dizi döndürür.

4. `plt.imshow(data, cmap='viridis')`: Oluşturduğumuz rastgele veriyi bir görüntü olarak görselleştirmek için `imshow()` fonksiyonunu kullanırız. Bu fonksiyon, belirtilen veriyi renkli bir görüntü olarak gösterir. `cmap` parametresi, kullanılacak renk haritasını belirler. Burada "viridis" renk haritasını kullanıyoruz. Renk haritaları, veri değerlerini renklere dönüştürmek için kullanılır ve farklı renk haritaları farklı renkler sağlar.

5. `plt.colorbar()`: Renkli bir görüntü oluşturduğumuzda, renklerin veri değerlerine karşılık gelen sayısal değerleri neler olduğunu göstermek için bir renk ölçeği eklemek iyi bir uygulamadır. `colorbar()` fonksiyonu, oluşturduğumuz renkli görüntünün yanına bir renk ölçeği ekler.

6. `plt.title('Renk Haritası Örneği')`: Grafiğin başlığını belirler. Bu durumda, başlık "Renk Haritası Örneği" olarak ayarlanmıştır.

7. `plt.show()`: Oluşturduğumuz görüntüyü görüntüler. Bu, Matplotlib'in pencereyi açmasını ve oluşturduğumuz grafikleri göstermesini sağlar.

Bu kod, rastgele veri oluşturup bu veriyi bir renk haritası kullanarak görselleştirir ve ardından bu görselleştirmeyi kullanıcıya sunar.

Renk haritası olarak imshow() fonksiyonunda kullanılabilecek bazı popüler seçenekler şunlardır:

* 'viridis'
* 'plasma'
* 'inferno'
* 'magma'
* 'cividis'
* 'gray'
* 'hot'
* 'cool'
* 'spring'
* 'summer'
* 'autumn'
* 'winter'

#### - **3D Grafikler:**
  - 3D grafikler, üç boyutlu verileri görselleştirmek için kullanılır.
  - `mpl_toolkits.mplot3d` modülü kullanılarak 3D grafikler oluşturulur.


```python
import matplotlib.pyplot as plt
import numpy as np
from mpl_toolkits.mplot3d import Axes3D

# Örnek veri oluşturma
x = np.linspace(-5, 5, 100)
y = np.linspace(-5, 5, 100)
X, Y = np.meshgrid(x, y)
Z = np.sin(np.sqrt(X**2 + Y**2))

# 3D yüzey grafiği oluşturma
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')
ax.plot_surface(X, Y, Z, cmap='viridis')
ax.set_title('3D Yüzey Grafiği')
plt.show()
```


    
![png](matplotlib-turkce-dok%C3%BCmentasyon_files/matplotlib-turkce-dok%C3%BCmentasyon_57_0.png)
    


Yukarıdaki örneğin kodunun adım adım açıklaması:

**1. İlgili kütüphanelerin içe aktarılması:**

```python
import matplotlib.pyplot as plt
import numpy as np
from mpl_toolkits.mplot3d import Axes3D
```

   - `matplotlib.pyplot` (plt): Grafikler oluşturmak ve görselleştirmek için kullanılır.
   - `numpy` (np): Bilimsel hesaplamalar yapmak için kullanılan bir kütüphanedir.
   - `mpl_toolkits.mplot3d` (Axes3D): 3D grafikler oluşturmak için gerekli araçları sağlar.

**2. Örnek veri oluşturma:**

```python
x = np.linspace(-5, 5, 100)
y = np.linspace(-5, 5, 100)
X, Y = np.meshgrid(x, y)
Z = np.sin(np.sqrt(X**2 + Y**2))
```

   - `np.linspace(-5, 5, 100)`: -5 ile 5 arasında eşit aralıklarla 100 değer oluşturur.
   - `np.meshgrid(x, y)`: x ve y dizilerinden bir ızgara oluşturur.
   - `np.sin(np.sqrt(X**2 + Y**2))`: Her bir ızgara noktasının sinüs değerini hesaplar.

**3. 3D yüzey grafiği oluşturma:**

```python
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')
ax.plot_surface(X, Y, Z, cmap='viridis')
ax.set_title('3D Yüzey Grafiği')
```

   - `plt.figure()`: Yeni bir figür oluşturur.
   - `fig.add_subplot(111, projection='3d')`: Yeni bir 3D subplot (alt grafik) oluşturur.
   - `ax.plot_surface(X, Y, Z, cmap='viridis')`: X, Y ve Z değerlerini kullanarak bir 3D yüzey grafiği çizer. 'viridis' renk haritasını kullanır.
   - `ax.set_title('3D Yüzey Grafiği')`: Grafiğin başlığını belirler.

**4. Grafiği görüntüleme:**

```python
plt.show()
```

   - `plt.show()`: Oluşturulan grafiği gösterir.

Bu şekilde, önce veri oluşturulur, sonra bu veri ile birlikte bir 3D yüzey grafiği oluşturulur ve son olarak bu grafiği görüntüleriz.
