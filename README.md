# SimpleAdr
[![Latest Stable Version](https://poser.pugx.org/n1215/simple-adr/v/stable)](https://packagist.org/packages/n1215/simple-adr)
[![License](https://poser.pugx.org/n1215/simple-adr/license)](https://packagist.org/packages/n1215/simple-adr)
[![Build Status](https://scrutinizer-ci.com/g/n1215/simple-adr/badges/build.png?b=master)](https://scrutinizer-ci.com/g/n1215/simple-adr/build-status/master)
[![Code Coverage](https://scrutinizer-ci.com/g/n1215/simple-adr/badges/coverage.png?b=master)](https://scrutinizer-ci.com/g/n1215/simple-adr/?branch=master)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/n1215/simple-adr/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/n1215/simple-adr/?branch=master)

A dead simple [Action-Domain-Responder pattern](https://github.com/pmjones/adr) example with no framework.
Compatible with [PSR-15 HTTP Server Request Handlers](https://www.php-fig.org/psr/psr-15/) and [PSR-17 HTTP Factories](https://www.php-fig.org/psr/psr-17/).

# Usage

## Install

```
composer create-project n1215/simple-adr
```

## Start server

```
cd simple-adr
php -S localhost:8000 -t public
```

and access

- http://localhost:8000/?id=1
- http://localhost:8000/?id=2
- http://localhost:8000/?id=3

## Directory structure

- entry point: [public/index.php](public/index.php)
- Action: [\N1215\SimpleAdr\Action\UserShowAction](src/Action/UserShowAction.php)
- Domain: [\N1215\SimpleAdr\Domain\UserShowUseCase](src/Domain/UserShowUseCase.php)
- Responder: [\N1215\SimpleAdr\Responder\UserShowJsonResponder](src/Responder/UserShowJsonResponder.php)


# License
The MIT License (MIT). Please see [LICENSE](LICENSE) for more information.
