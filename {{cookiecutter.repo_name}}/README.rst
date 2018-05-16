README for {{cookiecutter.project_desc}}

Testing with Docker
-------------------

This XBlock comes with a Docker test environment ready to build, based on the xblock-sdk workbench. To build and run it::

        $ make dev.run

The XBlock SDK Workbench, including this XBlock, will be available on the list of XBlocks at http://localhost:8000

Translating
-----------

Use the locale directory to provide internationalized strings for your XBlock project.

For more information on how to enable translations, visit the Open edX XBlock tutorial on Internationalization:
http://edx.readthedocs.org/projects/xblock-tutorial/en/latest/edx_platform/edx_lms.html

The template uses django-statici18n to provide translations to static javascript
using `gettext`.

The included Makefile contains targets for extracting, compiling, validating etc.
