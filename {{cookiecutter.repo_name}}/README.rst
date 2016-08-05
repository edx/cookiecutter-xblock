README for {{cookiecutter.project_desc}}

Testing with Docker
-------------------

This XBlock comes with a Docker test environment ready to build, based on the xblock-sdk workbench. To build it, run::

        $ docker build -t {{cookiecutter.package_name}} .

Then, to run the docker image you built::

        $ docker run -d -p 8000:8000 --name {{cookiecutter.package_name}} {{cookiecutter.package_name}}

The XBlock SDK Workbench, including this XBlock, will be available on the list of XBlocks at http://localhost:8000
