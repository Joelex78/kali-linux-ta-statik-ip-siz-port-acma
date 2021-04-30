# Kali linux'ta statik ip olmadan port açın / without static ip address open port in kali linux
Evrensel Tak & Çalıştır ile statik ip olmadan port açın / With Universal Plug aNd Play (upnp) open port without static ip

# UPNP nedir ? / What is UPNP ?
Evrensel Tak & Çalıştır adı verilen teknoloji sayesinde birçok elektronik cihaz kolayca birbiriyle uyumlu çalışabilir hale gelmektedir.
Böylece statik ip olmadan port açabilmemize olanak sağlamış oluruz. / With Universal Plug & Play technology most of the electronic devices communicate each other easily.
In this way you can open port without static ip.

![Alt text](https://www.teknolojihaber.net/images/upload/screenshot.1886912837.jpg)


# Not / Note
1-Öncelikle modeminizin upnp' yi desteklemesi gerekiyor. Gidip modem ayarlarından kontrol edebilirsiniz. / First of all your router needs to have upnp in it. You can check router's settings.

2-Eğer ana makineniz windows ise ve kali linux sanal makinede ise bir wifi kartına ihtiyacınız olacak. Wifi kartı kali linux'a bağlı hale getirdikten sonra sonraki adıma geçebilirsiniz. / If your machine has windows as a mother os and your kali linux is on virtual machine you need a wifi adapter. After you bind your wifi adapter with kali linux you can pass next step.


# Nasıl yapılır ? / How to do it ?
Öncelikle apt-get install upnpc ile gerekli yazılımı kuruyoruz. Ardından terminale upnpc -a XXX.XXX.X.X port port tcp veya udp yazarak enterlıyoruz.
'XXX.XXX.X.X' kısmı sizin ip adresiniz genelde 192. ile başlar, 'port port' yazan yer ise açmak istediğiniz portu girdiğiniz yer, 'tcp veya udp' açıklamama gerek olmadığını düşünüyorum. / First with apt-get install upnpc we install the script. then open terminal write and enter upnpc -a XXX.XXX.X.X port port tcp or udp.
'XXX.XXX.X.X' is your ip address usually its begin with 192., 'port port' which port do you want to open, 'tcp or udp' i guess i didn't have to explain.
