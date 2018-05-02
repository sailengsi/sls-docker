# lnmp.org官方1.5版本镜像制作

## 依赖

- centos.md

## command

- wget http://soft.vpser.net/lnmp/lnmp1.5beta.tar.gz -cO lnmp1.5beta.tar.gz && tar zxf lnmp1.5beta.tar.gz && cd lnmp1.5 && LNMP_Auto="y" DBSelect="4" DB_Root_Password="centos-lnmp-mysql" InstallInnodb="y" PHPSelect="8" SelectMalloc="1" ./install.sh lnmp