```
                 )))
 ______  __ooO__(o o)__Ooo_     ___ ______  ___    ______  ___ ___ ___ ____ _     ___ ______  ___     
|      |/  _]    (_)|    \ |   /   |      |/  _]  |      |/  _]  |||  |    \ |   /   |      |/  _]    
|      /  [_| _   _ |  o  )|  |  o |      /  [_   |      /  [_| (o o) |  o  )|  |  o |      /  [_     
|_|  ||    _]  \_/  |   _/ |__|    |_|  ||    _]  |_|  ||    _]  (_)  |   _/ |__|    |_|  ||    _]    
  |  ||   [_|   |   |  | |    |  _  ||  ||   [_     |  ||   [_O   |   O  | |    |  _  ||  ||   [_     
  |  ||     |   |   |  | |    |  |  ||  ||     |    |  ||     o   |   o  | |    |  |  ||  ||     |    
  |__||_____|___|___|__| |____|__|__||__||_____|    |__||_____|___|___|__| |____|__|__||__||_____|    

```  
> The default [Pyro Builder](github.com/websemantics/builder-extension) template for building [Pyro Builder ](github.com/websemantics/builder-extension) templates.

## Features

- All that is needed to build a [Pyro Builder](github.com/websemantics/builder-extension) template.

## Getting Started

To create an addon template you'll first need to install [Pyro Builder](github.com/websemantics/builder-extension) then run the following command,

```bash
php artisan builder:make template-template
```

Use option `--force` to download a fresh copy of `template-template`.

The builder will prompt you to enter a default `slug`, addon `type` and `vendor` for the target template.

```
Template default slug? [name]:
 > flat

 Template addon type? [module]:
  [0] module
  [1] theme
  [2] extension
  [3] field_type
 > 1

 Template default Vendor? [websemantics]:
 > anomaly

 Description? [An addon template for Pyro Builder.]:
 > Earthly flat

 Company name? [Web Semantics, Inc.]:
 > Anomaly Labs
```

The example above will create a template for a `theme` addon type that has a default slug, `flat` and a default vendor, `anomaly`.

Well, this gets my head spinning every-time, but, because the generated code is for the target template (of type, `module`, `theme`, `extension` etc) the user will be able to specify different `vendor` and `slug` values when it is used.

The target template will be located as per the usual formula, `vendor.type.slug`, **anomaly.theme.flat**. Move the template folder from `app/addons/default/anomaly/flat-theme` outside your project to prevent PHP throwing an exception.

To test and develop the generate template locally, place it in the builder storage folder (`app/storage/streams/default/builder/flat-theme`) then run,

```bash
php artisan builder:make flat-theme
```

Do not use `--force` option here or run `builder:clear` command as the template is not present in the registry, yet!

## The Easy Way

Is there an easy way, you ask? absolutely! Use the `make:addon` command as follows,

```bash
php artisan make:addon anomaly.theme.flat --template  --force --default
```

- `--template`: changes the behaviour of `make:addon` to create a template instead of the addon itself.
- `--default`: skips user interactivity and uses template default values.

## Contribution

If you have built an awesome template that would help others building better Pyro apps faster, consider submitting a request to include it in the registry. Thank you :)

## Support

Need help or have a question? post a questions at [StackOverflow](https://stackoverflow.com/questions/tagged/builder-extension+template-template)

*Please don't use the issue trackers for support/questions.*

## Resources

- [Pyro Builder](https://github.com/websemantics/entity_builder-extension), scaffold your PyroCMS apps in style for a more pleasurable and productive coding experience.
- [Default Module](https://github.com/pyrocms-templates/template-template), the default module template for Pyro Builder Extension.
- [Auto Pyro](https://github.com/websemantics/auto-pyro), a PyroCMS deploy tool for faster development experience.
- [Awesome PyroCMS](https://github.com/websemantics/awesome-pyrocms), a curated list of PyroCMS addons and resources.
- [PyroCMS](https://github.com/pyrocms/pyrocms), an MVC PHP Content Management System built to be easy to use, theme and develop with. It is used by individuals and organizations of all sizes around the world.

## License

[MIT license](http://opensource.org/licenses/mit-license.php)
Copyright (c) Web Semantics, Inc.
