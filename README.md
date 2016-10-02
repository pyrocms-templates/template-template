```
                 )))
 ______  __ooO__(oo )__Ooo_     ___ ______  ___    ______  ___ ___ ___ ____ _     ___ ______  ___     
|      |/  _]    (_)|    \ |   /   |      |/  _]  |      |/  _]  |||  |    \ |   /   |      |/  _]    
|      /  [_| _   _ |  o  )|  |  o |      /  [_   |      /  [_| (o o) |  o  )|  |  o |      /  [_     
|_|  ||    _]  \_/  |   _/ |__|    |_|  ||    _]  |_|  ||    _]  (_)  |   _/ |__|    |_|  ||    _]    
  |  ||   [_|   |   |  | |    |  _  ||  ||   [_     |  ||   [_|   |   |  | |    |  _  ||  ||   [_     
  |  ||     |   |   |  | |    |  |  ||  ||     |    |  ||     |   |   |  | |    |  |  ||  ||     |    
  |__||_____|___|___|__| |____|__|__||__||_____|    |__||_____|___|___|__| |____|__|__||__||_____|    

```  
> The default [Pyro Builder](github.com/websemantics/builder-extension) template for building [Pyro Builder ](github.com/websemantics/builder-extension) templates.

## Features

- All that is needed to build a [Pyro Builder](github.com/websemantics/builder-extension) template.

## Getting Started

To create an addon template you'll first need to install [Pyro Builder](github.com/websemantics/builder-extension) then run the following command,

```bash
php artisan make:addon anomaly.theme.flat --template
```

The previous command will create a template project for a theme addon. The `vendor` and `slug` information are going to be used as default values for the target addon. Use option `--force` to download a fresh copy of `template-template`.

The builder will prompt you to enter extra details or accept their default values

```
 Description? [An addon template for Pyro Builder.]:
 > Earthly flat

 Company name? [Web Semantics, Inc.]:
 > Anomaly Labs
```

This will create a template for a `theme` addon that has a default slug, `flat` and a default vendor, `anomaly`.

#### Default Values

The values for `vendor` and `slug` from the examples above are used as default values for the target template (`module`, `theme`, `extension` etc). The end-user can accept these defaults when the template is being used or specify different values.

#### Location

The target template will be located as per the usual formula, `vendor.type.slug` (**anomaly.theme.flat**) at `app/addons/default/anomaly/flat-theme`. Move the template outside your project to avoid runtime exceptions.

#### Development

To test and develop the generate template locally, place it in the builder storage folder (`app/storage/streams/default/builder/flat-theme`) then run,

```bash
php artisan make:addon flat-theme
```

Do not use `--force` option here or run `builder:clear` command as the template is not present in the registry, yet!

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
