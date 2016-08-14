FROM jbarciauskas/xblock-sdk
RUN mkdir -p /usr/local/src/{{cookiecutter.package_name}}-xblock
ADD . /usr/local/src/{{cookiecutter.package_name}}-xblock
RUN pip install -e /usr/local/src/{{cookiecutter.package_name}}-xblock
VOLUME ["/usr/local/src/{{cookiecutter.package_name}}-xblock"]

