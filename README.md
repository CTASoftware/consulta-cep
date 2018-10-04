# Buscar CEP Grátis
Com esse pacote você poderá realizar consultas de CEP gratuitamente.

Para evitar problemas com indisponibilidade de serviços, a consulta é realizada paralelamente em providers diferentes:

* [API ToolsWeb](https://toolsweb.com.br/busca-cep)
* [Website dos correios](http://www.buscacep.correios.com.br/sistemas/buscacep/)
* [API Viacep](https://viacep.com.br/)

A library irá retornar para você a resposta mais rápida, aumentando assim a performance da consulta.

### Changelog

* 1.0.1 - 03/10/2018 Primeira versão do pacote.


### Como utilizar

Adicione a library

```shell
$ composer require CTASoftware/consulta-cep
```
    
Adicione o autoload.php do composer no seu arquivo PHP.

```php
require_once 'vendor/autoload.php';  
```

Agora basta chamar o método `CepGratis::search($cep)`

```php
use CTASoftware\CepGratis\CepGratis;

$address = CepGratis::search('40301000'); 
```

### License

The MIT License (MIT)
