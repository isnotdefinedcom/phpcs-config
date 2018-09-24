PHP Coding Standard
===================

> Yet another PHP coding standard.

[![Packagist Version](https://img.shields.io/packagist/v/redaxmedia/php-coding-standard.svg)](https://packagist.org/packages/redaxmedia/php-coding-standard)
[![License](https://img.shields.io/packagist/l/redaxmedia/php-coding-standard.svg)](https://packagist.org/packages/redaxmedia/php-coding-standard)


Installation
------------

```
composer require redaxmedia/php-coding-standard
```


Usage
-----

Refer the coding standard inside your `phpcs.xml` file:

```xml
<ruleset>
	<rule ref="vendor/redaxmedia/php-coding-standard/phpcs.xml" />
</ruleset>
```

Exclude controversial `TypeHintDeclaration` rules as needed:

```xml
<rule ref="SlevomatCodingStandard.TypeHints.TypeHintDeclaration.MissingTraversableReturnTypeHintSpecification">
	<exclude-pattern>*</exclude-pattern>
</rule>
<rule ref="SlevomatCodingStandard.TypeHints.TypeHintDeclaration.MissingTraversableParameterTypeHintSpecification">
	<exclude-pattern>*</exclude-pattern>
</rule>
<rule ref="SlevomatCodingStandard.TypeHints.TypeHintDeclaration.MissingTraversablePropertyTypeHintSpecification">
	<exclude-pattern>*</exclude-pattern>
</rule>
```
