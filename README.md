No 'site_path'
==============

A DupalGap module.

For all information, please see http://drupalgap.org/project/nositepath

## Usage

In your `settings.js` file specify where nositepath should redirect when in
offline mode.  The default is "nositepath".

```
drupalgap.settings.nositepath = {
  offline_redirect: "nositepath"
};
```

If you would like to have a link to the connection form then add the following
snippet to the list of links defined as part of
`drupalgap.settings.menus['main_menu']` in your settings.js file:

```
{
  title: 'Connection',
  path: 'nositepath',
  options: {
    attributes: {'data-icon': 'gear'}
  },
},
```
