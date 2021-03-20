# php-iii-mar-2021-course-zend

## Lab: compile extension

- %s/INIT_DIR/INI_DIR/

- Error trying to compile

```bash
vagrant@php-training:~/Zend/workspaces/DefaultWorkspace/php3/src/ModAdvancedTechniques/Extensions/TelemetryExtension$ make
g++ -shared -o telemetry.so main.o -lphpcpp
/usr/bin/ld: cannot find -lphpcpp
collect2: error: ld returned 1 exit status
make: *** [Makefile:99: telemetry.so] Error 1
```

Not found PHP-CPP, I'm trying to compile but without success :-(


## Lab: Built-in web server


```bash
vagrant@php-training:~/php-iii-mar-2021-course-zend$ php -S localhost:8888
[Fri Mar 19 19:19:09 2021] PHP 8.0.3 Development Server (http://localhost:8888) started
[Fri Mar 19 19:19:17 2021] 127.0.0.1:58574 Accepted
[Fri Mar 19 19:19:17 2021] 127.0.0.1:58574 [200]: GET /
[Fri Mar 19 19:19:17 2021] 127.0.0.1:58574 Closing
[Fri Mar 19 19:19:17 2021] 127.0.0.1:58578 Accepted
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58578 [404]: GET /images/branding/googlelogo/1x/googlelogo_white_background_color_272x92dp.png - No such file or directory
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58578 Closing
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58582 Accepted
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58582 [404]: GET /xjs/_/js/k=xjs.hp.en.G6nUwKbI9pM.O/m=sb_he,d/am=AHiCOA/d=1/rs=ACT90oHk7-GIG-UpN3wj5rS6ZumP157E0A - No such file or directory
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58582 Closing
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58584 Accepted
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58584 [404]: GET /images/nav_logo229.png - No such file or directory
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58586 Accepted
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58584 Closing
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58586 [200]: GET /client_204?&atyp=i&biw=1380&bih=799&ei=pVtVYKrdLLSJjLsPweqtmAY
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58586 Closing
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58592 Accepted
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58592 [404]: GET /images/nav_logo229.png - No such file or directory
[Fri Mar 19 19:19:18 2021] 127.0.0.1:58592 Closing
```

- [index.php](/index.php): index.php to test built-in PHP web server

