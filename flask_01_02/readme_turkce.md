# Hands-on Flask-01-02 : Creating First Flask Application - Hello World and basic usage of Jinja Templates

Bu uygulamalı eğitimin amacı, öğrencilere yerel olarak Flask web uygulamasının nasıl oluşturulacağı konusunda hızlı giriş bilgisi vermektir.

## Learning Outcomes (Öğrenme Çıktıları)

Bu uygulamalı eğitimin sonunda öğrenciler;

client-server (İstemci-sunucu) yazılım mimarisini anlayın.

Python Flask frameworkünu öğrenin.

Python ve Flask frameworkünu yerel olarak yükleyin

Python Flask frameworküyle basit bir web uygulaması oluşturun.

uygulama sürümlendirmesini yönetmek için git repo'yu kullanın.

GitHub deposunu kod tabanı olarak kullanarak web uygulamasını AWS EC2 örneğinde çalıştırın (eğitmen tarafından gösterilecektir).

## Outline (Taslak)

Bölüm 1 - Python Flask frameworkünu tanıma

Bölüm 2 - GitHub Repo'da Basit Bir Merhaba Dünya Web Uygulaması Yazın

Bölüm 3 - GitHub Repo'da Jinja şablonuyla Basit bir Merhaba Dünya Web Uygulaması yazın

Bölüm 4 - Amazon Linux 2 EC2 Bulut Sunucusuna Python ve Flask frameworkünu yükleyin

## Part 1 - Getting to know the Python Flask framework (Bölüm 1 - Python Flask frameworkünu tanıma)

![Flask](./flask.png)

Flask, Python'da yazılmış bir web uygulaması geliştirme frameworküdür. Django gibi ortak kod ve bağımlılıklara sahip tam yığın frameworklerle karşılaştırıldığında başlamayı kolaylaştıran, yalnızca temel bileşenleri sağlayan bir mikro frameworküdür.
Yine de Flask, kimlik doğrulama, veritabanı ORM vb. gibi ek özelliklere sahip web uygulamaları geliştirmek için kitaplıklar, araçlar ve modüller sağlar.

Flask Framework'ün bazı özellikleri şunlardır;

Bir geliştirme sunucusu ve bir hata ayıklayıcı sağlar.

Şablonlama motoru olarak Jinja2'yi kullanır.

WSGI 1.0 ile uyumludur.

Birim testi için entegre destek sağlar.

İşlevlerini geliştirmek için birçok uzantı mevcuttur.


## Part 2 - Write a Simple Hello World Web Application on GitHub Repo (Bölüm 2 - GitHub Repo'da Basit Bir Merhaba Dünya Web Uygulaması Yazın)

flask-01-02-hello-world-app-Jinja-TemplateKlasörün altında reponuzda adlandırılmış bir klasör oluşturun python/hands-onve altına gidin.

flask-01-hello-world-app Adlı klasör oluştur

Adlı python dosyası oluşturunhello-world-app.py

Flask modülünü içe aktarın.

appİçe aktarılan Flask modülünden adlandırılmış bir nesne oluşturun .

helloBir dize döndüren bir işlev oluşturun Hello World.

helloİşlevi dekoratörle yönlendiren bir URL atayın @app.route('/').

secondBir dize döndüren bir işlev oluşturun ve işlevi dekoratörle This is the second pageyönlendiren bir URL atayın .second@app.route('/second')

thirdBir dize döndüren bir işlev oluşturun ve işlevi dekoratörle This is the subpage of third pageyönlendiren bir URL atayın .third@app.route('/third/subthird')

Kimlik numarasını dinamik olarak alan dinamik bir URL oluşturun ve sayfanın kimliğini gösteren bir masajla geri dönün.

uygulamayı hata ayıklama modunda çalıştırın

Hello World uygulamasını web tarayıcısından localhost:5000veya ile bağlayın.127.0.0.1:5000

uygulamaya 80 numaralı bağlantı noktasının herhangi bir yerinden erişmek için hata ayıklama modunu değiştirin

Kodun tamamını klasörün hello-world-app.pyaltındaki dosya olarak kaydedin hands-on/flask-01-02-hello-world-app-Jinja-Template/flask-01-hello-world-app.

Yerel depodaki tüm değişiklikleri ekleyin ve uygulayın

hello-world-app.pyUzak deponuza aktarın


## Part 3 - Write a Simple Hello World Web Application with Jinja template on GitHub Repo (Bölüm 3 - GitHub Repo'da Jinja şablonuyla Basit bir Merhaba Dünya Web Uygulaması yazın)

flask-02-Jinja_TemplateDeponuzun altında adlandırılmış bir klasör oluşturun python/hands-onve altına gidin

Adlı python dosyası oluşturunjinja.py

Flask ve render_template modüllerini içe aktarın.

appİçe aktarılan Flask modülünden adlandırılmış bir nesne oluşturun .

index.htmlŞablonlar klasörü altında bir dosya oluşturun .

Sayıları ve headdeğişkenleri . _ Bu değişkenleri dosyada kullanın . İşlevi dekoratörle yönlendiren bir URL atayın .number1number2index.htmlindex.htmlhead@app.route('/')

body.htmlŞablonlar klasörü altında bir dosya oluşturun .

Sayıyı ve bunların toplamını numbergönderen adında bir fonksiyon oluşturun . Bu değişkenleri dosyada kullanın . İşlevi dekoratörle yönlendiren bir URL atayın .num1num2index.htmlbody.htmlnumber@app.route('/sum')

uygulamayı hata ayıklama modunda çalıştırın

Hello World uygulamasını web tarayıcısından localhost:5000veya ile bağlayın.127.0.0.1:5000

Kodun tamamını klasörün jinja.pyaltındaki dosya olarak kaydedin flask-02-Jinja_Template.

Yerel depodaki tüm değişiklikleri ekleyin ve uygulayın

Tüm dosyaları GitHub'daki uzak deponuza aktarın.

## Part 4 - Run the Hello World App on EC2 Instance (Bölüm 4 - EC2 Bulut Sunucusunda Hello World Uygulamasını Çalıştırın)

SSH (Bağlantı Noktası 22) ve HTTP (Bağlantı Noktası 80) bağlantılarına izin veren güvenlik grubuyla Amazon Linux 2 AMI'yi kullanarak bir Amazon EC2 bulut sunucusu başlatın.

Örneğinize SSH ile bağlanın.

Örneğinizde yüklü paketleri ve paket önbelleğini güncelleyin.

git ve wget'i yükle

Web uygulaması dosyasını GitHub deposundan indirin.

Web uygulamasını çalıştırın

Merhaba Dünya uygulamasını web tarayıcısından bağlayın

Hello World uygulamasını terminalden komutuyla bağlayın curl.