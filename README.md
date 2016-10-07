１． DB
sudo apt install mysql-server
sudo apt install mysql-client
mysql -u username -p
CREATE USER stream IDENTIFIED BY 'password';
CREATE DATABASE xxx1;
CREATE DATABASE xxx2;
GRANT ALL ON *.* TO xxx3;
GRANT ALL ON ?.* TO xxx3;
GRANT ALL ON ?.* TO xxx3;
GRANT SELECT,UPDATE,INSERT,DELETE ON ?.* TO xxx3;
GRANT SELECT,UPDATE,INSERT,DELETE ON ?.* TO xxx3;
2.
sudo apt-get install redis-server
sudo apt-get install nginx
sudo vi /etc/nginx/nginx.conf
sudo vi /etc/nginx/sites-enabled/??.conf
sudo vi /etc/nginx/sites-enabled/??.conf
3. php
sudo apt install php5
sudo apt-get install php5-fpm
sudo service nginx reload
sudo service php5-fpm restart
/etc/php5/fpm/pool.d/www.conf user/group
sudo apt-get install php5-curl
sudo apt-get install php5-memcached
sudo apt-get install php5-mysql
sudo apt-get install php5-dev for phpize
git clone https://github.com/hnw/php-timecop.git
cd php-timecop
phpize
./configure
make
sudo make install
timecop.iniファイルを作る。
for yaml
sudo apt-get install php-pear libyaml-dev
sudo pecl install YAML
extension=yaml.so
 
3. git submodule update
(git submodule init
git submodule update) 
git submodule foreach git pull origin master
git reset HEAD res
 
redis-cli
 
４．modify timezone to JST
sudo ln -sf /usr/share/zoneinfo/Japan /etc/localtime
 
５．いつも使っているコマンド
sudo service nginx reload
sudo service php5-fpm restart
sudo service redis-server restart
 
6.zsh install
sudo apt-get install zsh
 
7. rbenv(ruby 管理ツール) install
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
cd ~/.rbenv && src/configure && make -C src
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
~/.rbenv/bin/rbenv init
 
8. gem/bundle install
http://www.d-wood.com/blog/2013/09/25_4699.html
 
9. redis-dump/redis-load install
gem install redis-dump
