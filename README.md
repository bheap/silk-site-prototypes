# silk site prototypes
### site prototypes for the Silk Web Toolkit

Site prototypes are scaffolding or templates to help get you started quickly with site building.
Build whatever templates help you out, complement the limited core templates bundled with Silk.

## how to build a site prototype
### manually

* have a look at the handful of samples under org/silkyweb
* find or create a package directory to place your site prototype in
  * placing site prototypes in packages helps guarantee uniqueness
* name your prototype something sensible
  * 'default-empty' is the simplest possible site prototype, it simply creates a skeleton directory structure
  * 'default-basic' provides the simplest example with some css, one view, a template and a static component
* create a directory with the same name as the version of Silk you are using
  * just use the major.minor.patch ie 0.1.0
* create all the required directories; .dna, component, meta, resource, site, template, view
* add a dna.conf definition to .dna, see the examples under org/silkyweb
  * check your package value is the same as the directory hierarchy you have placed your site in
  * silk-version is the version of Silk the template has been built and tested against
  * it is useful to add a quick description of the purpose of the site prototype, like what it integrates with
* place any components you would like in the 'component' directory
* place any number of views (in the case of a static site these are effectively pages) in 'view'
* place a template called default.html in 'template'
* place css, less, js etc in the 'resource' directory
* place robots.txt and other metadata if required in 'meta'
* test your site prototype by 'spinning' it with Silk

### or with silk

* 'silk clone-site some-site'
* modify the .dna/dna.conf file to suit
* modify the rest of the content to suit
* in your site's parent directory 'silk install-site'


## how to contribute

### you

* fork this repository
* add your site prototype
* submit a pull request

### us

* review your pull request
* add to silk site prototype repository so your site prototype is available with 'silk update'
