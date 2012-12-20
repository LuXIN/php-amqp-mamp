# Installation
1. Copy `amqp.so` to /Applications/MAMP/bin/php/php5.x.x/lib/php/extensions/no-debug-non-zts-200xxxxx (Channge 5.x.x to your PHP version)
2. Add `extension="amqp.so"` to the end of php.ini (Open MAMP click on File → Edit Template → PHP → PHP 5.x.x php.ini) (Channge 5.x.x to your PHP version)
3. Restart MAMP.

## Dependencies

* rabbitmq
* librabbitmq

### Depencencies installation


**RabbitMQ**

```
brew install rabbitmq
```

**librabbitmq**

```
git clone git://github.com/alanxz/rabbitmq-c.git
cd rabbitmq-c
git submodule init
git submodule update
autoreconf -i && ./configure && make && sudo make install

```

