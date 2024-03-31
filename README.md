# Grass Bot Kurulumu

> Öncelikle [Parenthost]( https://parenthost.com/) sitesine üye olup 1 adet Static Residential Proxy satın alalım.(NOT: Kripto cüzdanınız ile Polygon ağında ödeme yapabiliyorsunuz.)
> 
> 1 Adet en az 2vCpu 4GB VPS lazım. bunu da Sanal Kart ile ücretsiz bir şekilde [Atlantic Server]( https://cloud.atlantic.net/r/hzhf89vq) sitesine üye olup 250$'lık bonus ile alabilirsiniz.

## Kuruluma Geçelim

```console
# Kodları tek tek sunucunuza girin.
sudo apt update
sudo apt install git
sudo apt install python3 && sudo apt install python3-pip
```
> Y diyoruz...
> 
![image](https://i.hizliresim.com/8dt707h.jpg)

```console

git clone https://github.com/excelliumCoin/grassbt.git && cd grassbt && pip3 install websockets_proxy && pip3 install loguru

```
>
```console

nano main.py

```
## Gerekli yerleri düzenliyoruz

![image](https://i.hizliresim.com/ar0xgeb.jpg)

> _user_id için [Grass Dashboard](https://app.getgrass.io/dashboard) 'a giriyoruz. F12 tuşuna basıyoruz veya mouse sağ tık ve sayfayı incele diyoruz.
> 
> Console tıklıyoruz. Alttaki kodu yapıştırıp çıkan user id kopyalıyoruz.
```console
localStorage.userId
```
![image](https://i.hizliresim.com/2themzn.jpg)

> socks5_proxy_list kısmına ise ParentHosttan almış olduğunuz Static Residential Proxy'i bu formata göre düzenleyip yapıştırıyoruz 'socks5://USERNAME:PASSWORD@IPADDRESS:port'
>
> Resimdeki gibi

![image](https://i.hizliresim.com/p9nj7yc.jpg)

## CTRL X+Y Enter diyip çıkıyoruz.


```console
sudo apt install screen & screen -s grass

```
## Ve çalıştırıyoruz.

```console
python3 main.py

```
### Aşağıdaki gibi bir çıktı aldıysanız işlem tamamdır
![image](https://i.hizliresim.com/ew6f5ry.jpg)

### CTRL A+D diyoruz ve sunucu konsolunu kapatıyoruz


## Grass Dashboard'a girin ve kontrol edin. Aşağıdaki gibi bağlantınız %100 gözükmeli.

![image](https://i.hizliresim.com/hec0hv6.jpg)
