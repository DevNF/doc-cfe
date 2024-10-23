# Extrato CF-e

## Requirements
* PHP version 7.1 or higher


## Install with composer

```bash
composer require nfservice/doc-cfe
```


## Quick Start

```php
use NFService\CFe\Extrato;

$xml = __DIR__ . 'path_to_xml';

$logo = __DIR__ . 'path_to_logo';


$infoConsultaAplicativo = "Informação para consulta do QrCode via aplicativo utilizado no estado";

$extrato = new Extrato($xml, $logo, $infoConsultaAplicativo);

//Obtêm extrato em HTML
$html = $extrato->html();

//Obtêm extrato em PDF 
$pdf = $extrato->pdf();

//Realiza download do extrato em PDF
$extrato->pdf(true);


```

## Autor Original

Este projeto foi desenvolvido originalmente por [Arley Oliveira](https://github.com/arleyoliveira).

## Fork

Este fork foi criado por [Henrique Ernandes](https://github.com/henriquernandes).
