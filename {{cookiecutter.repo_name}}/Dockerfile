FROM jbarciauskas/xblock-sdk
RUN mkdir -p /usr/local/src/{{cookiecutter.package_name}}
ADD . /usr/local/src/{{cookiecutter.package_name}}
RUN pip install -e /usr/local/src/{{cookiecutter.package_name}}

