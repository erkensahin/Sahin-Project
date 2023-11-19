# Project-101: Cloudformation kullanılarak AWS EC2'ye dağıtılan Kittens Carousel Statik Web Sitesi

## Description (Tanım)
Kittens Carousel, AWS Cloudformation Service kullanılarak AWS Elastic Compute Cloud (EC2) Örneğinde Apache Web Sunucusu ile dağıtılan statik bir web sitesi uygulamasıdır.

## Problem Statement (Sorun bildirimi)

![Project_101](Pro_Project_101.png)

- Firmanız yakın zamanda evcil hayvan severlerin çekim noktası olacak bir web uygulama projesine başlamıştır. Projenin ilk adımı olarak ekibinizdeki geliştiriciler, yavru kedi atlıkarınca uygulamasının ön tasarımını hazırladılar ve proje için gerekli dosyaları GitHub'daki depoya aktardılar.

- Göreviniz, uygulama tasarımının geliştirme ortamında statik bir web sayfası olarak nasıl göründüğünü göstermektir. Bu nedenle web uygulamasını 'index.html' ve 'statik-web' klasöründe verilen görselleri kullanarak dağıtmanız gerekir. Web uygulamanız için aşağıdakilere dikkat edin.

- Web uygulaması başlatıldığında kullanıcı ilk önce `index.html` ile karşılaşmalıdır.

- Uygulama Apache Web Sunucusunda konuşlandırılmalıdır.

- Uygulama, AWS Cloudformation Service kullanılarak AWS EC2 Örneğindeki geliştirme ortamında dağıtılmalıdır. Geliştirme ortamında Cloudformation şablonunuzu aşağıdakileri kullanarak yapılandırabilirsiniz:

- Uygulama yığını yeni AWS kaynaklarıyla oluşturulmalıdır.

- Uygulama, Amazon Linux 2023 Image'ın (Bonus) en son sürümünde çalışmalıdır. İşte bu zorlukla ilgili bilgileri bulabileceğiniz bağlantı. Ancak Amazon Linux 2023 AMI'ye ihtiyacımız olduğu için aşağıda göreceğiniz bu yazıda Amazon Linux 2'ye ait bazı parametreleri değiştirmeniz gerekmektedir.

https://aws.amazon.com/blogs/compute/query-for-the-latest-amazon-linux-ami-ids-using-aws-systems-manager-parameter-store/

- EC2 Bulut Sunucusu türü 't2.micro' olarak yapılandırılabilir.

- Cloudformation tarafından başlatılan örnek "StackName Web Sunucusu" olarak etiketlenmelidir

- Web Uygulamasına web tarayıcısı aracılığıyla her yerden erişilebilmelidir.

- Uygulama dosyaları Github deposundan indirilmeli ve Cloudformation şablonu içindeki kullanıcı veri komut dosyası kullanılarak EC2 Örneğine dağıtılmalıdır.

- Kittens Carousel Uygulaması Web Sitesi URL'si, yığın oluşturulduktan sonra Cloudformation Service tarafından çıktı olarak verilmelidir.

## Project Skeleton

```
101-kittens-carousel-static-website-ec2 (folder)
|
|----readme.md         # Öğrencilere verildi(Projenin tanımı)
|----cfn-template.yml  # To be delivered by students (Cloudformation template)
|----static-web
        |----index.html  # Öğrencilere verildi (HTML file)
        |----cat0.jpg    # Öğrencilere verildi (image file)
        |----cat1.jpg    # Öğrencilere verildi (image file)
         |----cat2.jpg    # Öğrencilere verildi (image file)
```         

## Expected Outcome (Beklenen sonuç)

![Project 101 : Kittens Carousel Application Snapshot](./project-101-snapshot.png)

### Proje sonunda aşağıdaki konular ele alınacaktır;

- Apache Web Server Installation on Linux (Linux'ta Apache Web Sunucusu Kurulumu)

- Static Website Deployment (Statik Web Sitesi Dağıtımı)

- Bash scripting

- AWS EC2 Service

- AWS Security Groups Configuration

- AWS Cloudformation Service

- AWS Cloudformation Template Design

- Git & Github for Version Control System

### At the end of the project, students will be able to; (Proje sonunda öğrenciler);

- Apache Web Sunucusunu Amazon Linux 2023'e yükleyin

- EC2 Örneğinde web uygulamasını yüklemek ve ayarlamak için Cloudformation'daki "kullanıcı verileri" bölümünü kullanarak bash komut dosyası yazma becerilerini geliştirin.

- AWS EC2 Bulut Sunucusu ve Güvenlik Gruplarını yapılandırın.

- Cloudformation şablonunu AWS Kaynaklarını kullanacak şekilde yapılandırın.

- Yığınları başlatmak için AWS Cloudformation Service'i kullanın.

- git komutlarını (Push, pull, commit, add vb.) ve Github'u Sürüm Kontrol Sistemi olarak kullanın.

## Steps to Solution (Çözüm Adımları)

- Adım 1: Github'daki "clarusway" deposundan proje tanımını indirin veya kopyalayın

- Adım 2: Bilgisayarınızda yerel genel depo için proje klasörü oluşturun

- 3. Adım: Uygulamanızı EC2 Örneğinde dağıtmak için bir bulut oluşturma şablonu hazırlayın

- Adım 4: Başvurunuzu Github'daki kendi genel deponuza aktarın

- Adım 5: Uygulamanızı ekibinizde sergilemek için Cloudformation şablonunu kullanarak uygulamanızı AWS Cloud'a dağıtın.

## Notes

- 'index.html' içindeki 'öğrenci_adı' yerine adınızı sabit kodlayarak uygulamayı özelleştirin.

## Resources (Kaynaklar)

- [AWS Cloudformation User Guide](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)