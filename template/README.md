```
{{[slug,' ',type]|join|upper|figlet('crawford')}}
{{'T E M P L A T E'|figlet}}
```
> {{description}}

## Features

- All files needed to build a [Pyro Builder](github.com/websemantics/builder-extension) template.

## Install

After installing [Pyro Builder](github.com/websemantics/builder-extension) run,

```
php artisan make:builder {{slug}}-{{type}}
```

## Support

Need help or have a question? post a questions at [StackOverflow](https://stackoverflow.com/questions/tagged/{{[slug,'-',type,' -template']|join|lower}})

*Please don't use the issue trackers for support/questions.*

## License

[MIT license](http://opensource.org/licenses/mit-license.php)
Copyright (c) {{company}}
