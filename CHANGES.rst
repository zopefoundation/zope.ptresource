=========
 Changes
=========


4.1.0 (2017-08-31)
==================

- Add support for Python 3.5 and 3.6.

- Drop support for Python 2.6 and 3.3.



4.0.0 (2014-12-24)
==================

- Add support for PyPy and PyPy3.

- Add support for Python 3.4.

- Add support for testing on Travis.



4.0.0a1 (2013-02-25)
====================

- Add support for Python 3.3.

- Replace deprecated ``zope.interface.implements`` usage with equivalent
  ``zope.interface.implementer`` decorator.

- Drop support for Python 2.4 and 2.5.



3.9.0 (2009-08-27)
==================

Initial release. This package was split off zope.app.publisher as a part
of refactoring process. It's now a plugin for another package that was
refactored from zope.app.publisher - zope.browserresource. See its
documentation for more details.

Other changes:

 * Don't render PageTemplateResource when called as the IResource interface
   requires that __call__ method should return an absolute URL. When accessed
   by browser, it still will be rendered, because "browserDefault" method now
   returns a callable that will render the template to browser.
