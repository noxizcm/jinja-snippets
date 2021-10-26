# Jinja Snippets for VSCode

[![MIT License](https://img.shields.io/badge/License-MTI-green)](https://opensource.org/licenses/MIT)

**A fast, and attractive way to build Jinja / HTML templates.**



>**Jinja** is a fast, expressive, extensible templating engine. Special placeholders in the template allow writing code similar to Python syntax. Then the template is passed data to render the final document. [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.0.x/templates/)


## Getting started

To start using the snippets simply type **j.** *snippet_name*.

* To preview the selected snippet click `CTRL+SPACEBAR`.  
* To use the selected snippet simply click `TAB`.


## Features

### Basics
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.comm**|`{#  #}`|Comments|
|**j.exp, j.print**|`{{  }}`|Expressions|
|**j.stat**|`{% statement %}`|Statements|
|**j.block**|`{% block name} {% endblock %}`|Blocks|

### If statements
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.if**|`{% if condition } {% endif %}`|if statement|
|**j.if-else**|`{% if condition } {% else} {% endif %}`|if and else statement|
|**j.if-elif-else**|`{% if condition } {% elif condition2 } {% else} {% endif %}`|if, elif and else statement|
|**j.if-for**|`{% if iterable }{% for item in iterable %} {% endfor %}{% endif %}`|for loop in a if statement|

### For and with statements
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.for**|`{% for item in iterable %} {% endfor %}`|for statement|
|**j.for-if**|`{% for item in iterable %}{% if item } {% endif %}{% endfor %}`|if statement in a for loop|
|**j.for-else**|`{% for item in iterable %} {% else %} {% endfor %}`|else break statement in a for loop|
|**j.with**|`{% with item} %} {% endwith %}`|with statements|

### Extendsn, Inclides and Imports 
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.extends**|`{% extends 'filename' %}`|template inheritance|
|**j.incl**|`{% include 'filename' %}`|include a template into the current namespace. Tabstops Choice: ignore missing, with context, ignore missing with context|
|**j.imp**|`{% import 'filename' %}`|import module into current namespace. Tabstops Choice: with context|
|**j.imp-from**|`{% from 'template' import 'module' } %}`|import specific names from a template into the current namespace. Tabstops Choice: with context|

### Macros, Call, Filters
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.macro**|`{% macro name(args) %} {% endmacro %}`|define macro/function|
|**j.call**|`{% call macroname(args}) %} {% endcall %}`|call functionality for macro/function|
|**j.filter**|`{% filter filtername %} {% endfilter %}`|apply regular jinja filters|

### Assignments
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.set**|`{% set variable = value %}`|assign value to variable|
|**j.setmulti**|`{% set key, value = callable() %}`|assign key, value returned by a callable|
|**j.setblock**|`{% set variable %} contents {% endset %}`|block assignments: capture the contents of block into variable|

### lipsum, Random and Url
|Snippets|Output|Desciption|
|--------|------|----------|
|**j.lipsum, j.lorem**|`{{ lipsum(n=5, html=True, min=20, max=100) }}`|generate some lorem ipsum.|
|**j.random**|`{{ range(0, 10000, 1) \| random }}`|generate random item from a range|
|**j.url**|`{{ url_for('endpoint') }}`|url for endpoint (flask)|


## Release Notes

### 1.0.0

Initial release of version

___
**Enjoy!**