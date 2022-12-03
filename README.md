В репозитории находится Vagrantfile, который собирает Raid 5, командой
mdadm --create --verbose /dev/md0 --level=6 --raid-devices=5 /dev/sdb1 /dev/sdc1 /dev/sdd1 /dev/sde1 /dev/sdf1
Для выполнения надо скопировать файл себе и запустить с помощью vargant up
Проверить можно командой
mdadm -D /dev/md0
