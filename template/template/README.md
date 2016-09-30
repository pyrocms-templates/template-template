{% verbatim %}
```
{{[slug,' ',type]|join|upper|figlet}}
```
> {{description}}

## Install

After installing [Pyro Builder](github.com/websemantics/builder-extension) run,

```
php artisan make:builder {{slug}}-{{type}}
```

## License

[MIT license](http://opensource.org/licenses/mit-license.php)
Copyright (c) {{vendor}}
{% endverbatim %}
