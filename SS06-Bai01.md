root@103725795523314:~# mkdir -p /var/www/my-app/public
root@103725795523314:~# mkdir -p /var/www/my-app/logs
root@103725795523314:~# ls -la /var/www/my-app
total 16
drwxr-xr-x 4 root root 4096 Oct  7 14:06 .
drwxr-xr-x 7 root root 4096 Oct  7 14:00 ..
drwxr-xr-x 2 root root 4096 Oct  7 14:06 logs
drwxr-xr-x 2 root root 4096 Oct  7 14:00 public
root@103725795523314:~# chmod 750 /var/www/my-app/public
root@103725795523314:~# ls -la /var/www/my-app
total 16
drwxr-xr-x 4 root root 4096 Oct  7 14:06 .
drwxr-xr-x 7 root root 4096 Oct  7 14:00 ..
drwxr-xr-x 2 root root 4096 Oct  7 14:06 logs
drwxr-x--- 2 root root 4096 Oct  7 14:00 public
root@103725795523314:~# chmod 770 /var/www/my-app/logs
root@103725795523314:~# ls -la /var/www/my-app
total 16
drwxr-xr-x 4 root root 4096 Oct  7 14:06 .
drwxr-xr-x 7 root root 4096 Oct  7 14:00 ..
drwxrwx--- 2 root root 4096 Oct  7 14:06 logs
drwxr-x--- 2 root root 4096 Oct  7 14:00 public
root@103725795523314:~# chown -R toandev:www-data /var/www/my-app
root@103725795523314:~# ls -la /var/www/my-app
total 16
drwxr-xr-x 4 toandev www-data 4096 Oct  7 14:06 .
drwxr-xr-x 7 root    root     4096 Oct  7 14:00 ..
drwxrwx--- 2 toandev www-data 4096 Oct  7 14:06 logs
drwxr-x--- 2 toandev www-data 4096 Oct  7 14:00 public
