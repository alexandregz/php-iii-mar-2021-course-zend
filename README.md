# php-iii-mar-2021-course-zend

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

