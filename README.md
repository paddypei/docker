# docker
php7.2+swoole4.x

use
docker run --privileged -it -d  --hostname=twitf  --name=twitf  -v D:/wwwroot:/www/wwwroot -p 2203:22 twitf/php72-swoole4
默认上级目录为根目录 php版本7.1,可在当前目录下的.env文件修改

install
git clone https://github.com/twitf/docker.git
cd docker
docker-compose up -d
目录 /www
├── tmp
├── wwwlogs
├── server
│   ├── php      
│   └── supervisor
├── wwwlogs
└── wwwroot
ssh
SSH登录：root用户密码为root，用户twitf密码为twitf

#安装扩展

pecl install xxx && enable-php-extension xxx
