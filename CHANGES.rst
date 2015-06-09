Changelog
=========

3.0.5 (unreleased)
------------------

- Nothing changed yet.


3.0.4 (2015-05-13)
------------------

- patch locking functions to use _v_safe_write attribute
  [vangheem]

- Be able to use _v_safe_write attribute to specify objects are safe to write
  [vangheem]


3.0.3 (2015-03-30)
------------------

- handle zope root not having IKeyManager Utility and CRSF protection
  not being supported on zope root requests yet
  [vangheem]

3.0.2 (2015-03-13)
------------------

- Add ITransform.transformBytes for protect transform to fix compatibility
  with plone.app.blocks' ESI-rendering
  [atsoukka]


3.0.1 (2014-11-01)
------------------

- auto CSRF protection: check for changes on all the storages
  [mamico]

- CSRF test fixed
  [mamico]


3.0.0 (2014-04-13)
------------------

- auto-rotate keyrings
  [vangheem]

- use specific keyring for protected forms
  [vangheem]

- add automatic clickjacking protection(thanks to Manish Bhattacharya)
  [vangheem]

- add automatic CSRF protection
  [vangheem]


2.0.2 (2012-12-09)
------------------

- Use constant time comparison to verify the authenticator. This is part of the
  fix for https://plone.org/products/plone/security/advisories/20121106/23
  [davisagli]

- Add MANIFEST.in.
  [WouterVH]

- Add ability to customize the token created.
  [vangheem]


2.0 - 2010-07-18
----------------

- Update license to BSD following board decision.
  http://lists.plone.org/pipermail/membership/2009-August/001038.html
  [elro]

2.0a1 - 2009-11-14
------------------

- Removed deprecated AuthenticateForm class and zope.deprecation dependency.
  [hannosch]

- Avoid deprecation warning for the sha module in Python 2.6.
  [hannosch]

- Specify package dependencies
  [hannosch]

1.1 - 2008-06-02
----------------

- Add an optional GenericSetup profile to make it easier to install
  plone.protect.
  [mj]

1.0 - 2008-04-19
----------------

- The protect decorator had a serious design flaw which broke it. Added
  proper tests for it and fixed the problems.
  [wichert]

1.0rc1 - 2008-03-28
-------------------

- Rename plone.app.protect to plone.protect: there is nothing Plone-specific
  about the functionality in this package and it really should be used outside
  of Plone as well.
  [wichert]

- Made utils.protect work with Zope >= 2.11.
  [stefan]

1.0b1 - March 7, 2008
---------------------

- Refactor the code to offer a generic protect decorator for methods
  which takes a list of checkers as options. Add checkers for both the
  authenticator verification and HTTP POST-only.
  [wichert]

1.0a1 - January 27, 2008
------------------------

- Initial release
  [wichert]