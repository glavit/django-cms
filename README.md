# django-cms
Pages and categories for django.

# Install
* Add to INSTALLED_APPS 'cms', 
* Add to end of MIDDLEWARE_CLASSES 'cms.middleware.PageMiddleware',
* Add to end of urls.py url(r'^', include('cms.urls')),
* manage.py syncdb
## Notise
If you want to use multilanguage you must instal hvad, define LANGUAGES in settings and use 'middleware.SwitchLocaleMiddleware', to change languages.


# Futures
* Templates for admin
* Add slash checking (https://docs.djangoproject.com/en/dev/ref/settings/#append-slash)
* Templates paganation
* New views
* New templates

# I think about
* tree to category parent select

# Changelog
## 2012.11.07
### Add
* Templates for multilanguage
* DE Locale
### Fix
* views template puth
* README.md

## 2012.11.07
### Add
* Multilanguage
### Fix
* view()
* views::page() Optimization

## 2012.10.17
### Fix
* PEP-8
* Remove tiny_mce


## 2012.07.24
### Add
* Filter by sites.
* cms_render template tag

## 2012.07.14
### Add
* SafeUnicode to Category.
* Rename Pages to Page.
* Ordering to pages.

### Fix
* Optimized README.md
* Add permalink to get_absolute_url for Category.
* Optimized urls.py.
* Optimized Meta class of Category.
* Optimized url_puth method of Category.
* Optimized middleware PageMiddleware.
* Fix save method of Category. If you save category all childs will by saved and all pages of this category to change url.


## 2012.07.13
### Add
* Add get_absolute_url to Category.

### Fix
* Now, SEO is a standalone application.
* MetaTeg moved to SEO.
* Optimized middleware.
* Optimized Pages save method.
* Now use ugettext_lazy.

## 2012.07.11
### Add
* created_at
* updated_at

### Fix
* new README.md
* full_url field changed to url
* Optimized save method.
* Optimized url_puth method.
* Optimized display method.
* Optimized __unicode__ method.
