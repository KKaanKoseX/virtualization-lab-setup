Bu projede VMware sanallaştırma ortamı ve Proxmox VE kullanılarak sanal bir BT sistem alt yapısı oluşturulacaktır.

1. Sistemimizde kurulunu olan sanallaştırma platformu (VMware kullandım) içerisine Proxmox VE kurulumu gerçekleştireceğiz.
2. Kurulan Proxmox VE ortamına Windows-Server(Active Directory,DNS,DHCP), Ubuntu Server ve Veeam Backup Server kurulumu gerçekleştirilecektir.

3. Proxmox kurulumunu yaptıktan sonra(kullanıcı adı:root şifre:belirlediğiniz şifre.).

   
<img width="1457" height="738" alt="Screenshot 2025-07-23 152841" src="https://github.com/user-attachments/assets/f03714a2-658e-49fd-ae40-8233e3a15241" />

Ekran görüntüsünde verilen ip adresini tarayıcınızdan girdikten, Proxmox web arayüzüne erişip kullanıcı adı ve şifrenizi girdikten sonra kurmuş olduğunuz sanal ortamın web arayüzüne bağlanmış olacaksnız.


<img width="1457" height="738" alt="resim" src="https://github.com/user-attachments/assets/2561ed54-7b84-481a-9e15-2205e377226d" />


4. Proxmox sanallaştırma ortamına windows-server kurulumu.
   Öncelikli olarak windows-server-22 iso dosyasını indirmemiz gerekiyor.
   İndirme işlemi bittikten sonra Proxmox web arayüzünde sol tarafta bulunan Server View ekranında bulunan Datacenter>pve>local(pve)>ISO Images sekmesine Iso image'imizi eklememiz gerekiyor.


   <img width="1457" height="738" alt="resim" src="https://github.com/user-attachments/assets/4cd3125f-deba-45f8-a1a5-6a7268bf83a8" />


5. Sanallaştırma ortamın'a ISO dosyasını ekledikten sonra sağ üst kısımda bulunan Create VM ile Windows-Server-22 sanal makinemizin kurulumunu yapıyoruz.
   General kısmında snal makineye isim verdikten sonra Next'e tıklayıp OS sekmesinde ise kuracağımız ve Virtual Environment'a eklediğimiz iso dosyasını seçiyoruz. Operation System olarak Microsoft Windows'u seçtiğinizden emin    olun.

<img width="1457" height="738" alt="resim" src="https://github.com/user-attachments/assets/8d2f0593-775a-4f74-a991-636a9fd323de" />


BİLGİLENDİRME -------> Nested Virtualization için sistem gereksinimlerim yetersiz olduğu için VMware içerisinde Proxmox kullanmayıp, oluşturacağım sistemi VMware üzerinden oluşturmak durumundayım, fakat proxmox üzerinden bu adımları gerçekleştirebilirsiniz.


