README for {{cookiecutter.short_name}}

Testing with Docker
-------------------

This XBlock comes with a Docker test environment ready to build, based on the xblock-sdk. To build it, run::

        $ docker build -t xblock-{{cookiecutter.short_name}} .

Then, to run the docker image you built::

        $ docker run -d -p 8000:8000 --name xblock-{{cookiecutter.short_name}} xblock-sdk-{{cookiecutter.short_name}}

Your XBlock will be available on the list of XBlocks at http://localhost:8000
