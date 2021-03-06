# Test your local running app from your mobile browser (DNS Mobile React iPhone Android)
Testing Your Local React App Mobile Browser iPhone Android

# Install DNS in your Mac
The instructions are for Mac OSX via Homebrew:

> brew install dnsmasq

dnsmasq is a lightweight dns server that will fallback to the original DNS server when it encounters an unknown domain

Add the line address=/www.your-domain.com/192.168.86.26 (my Mac ip in this sample) to the file /usr/local/etc/dnsmasq.conf

> vi /usr/local/etc/dnsmasq.conf

The IP Address 192.168.86.26 is whatever the IP address assigned to your local computer by your router. You can find this via Network Utility (ifconfig)

> sudo brew services restart dnsmasq

This starts dnsmasq process, and it will listen on the DNS ports

Edit your /etc/hosts

> sudo vi /etc/hosts
>
> 127.0.0.1  yourdomain.com

Set your local computer's IP Address as your DNS Server your iPhone, go to Settings -> Wi-Fi -> Info icon for your connected router -> DNS

![IMG_1049](https://user-images.githubusercontent.com/19804605/155190823-8837fbbb-bbe0-45d9-bbb3-7b1f3d473899.PNG)

![IMG_1050](https://user-images.githubusercontent.com/19804605/155190865-ec1d3d8a-eff1-42f6-a542-a3388518ff06.PNG)

