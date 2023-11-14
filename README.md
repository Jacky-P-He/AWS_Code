# AWS_Code
** To deploy a Website on AWS EC2 using Apache**

sudo su -
ls
yum update -y
yum install -y httpd

wget https://github.com/Jacky-P-He/ArtistSearch/archive/refs/heads/main.zip
unzip main.zip 
cd ArtistSearch-main/
mv * /var/www/html
cd /var/www/html
systemctl enable httpd
systemctl start httpd
systemctl status httpd

[Optional] systemctl stop httpd
