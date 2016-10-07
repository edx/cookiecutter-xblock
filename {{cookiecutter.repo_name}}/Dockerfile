FROM xblock-sdk
RUN mkdir -p /usr/local/src/{{cookiecutter.repo_name}}
VOLUME ["/usr/local/src/{{cookiecutter.repo_name}}"]
RUN echo "pip install -e /usr/local/src/{{cookiecutter.repo_name}}" >> /usr/local/src/xblock-sdk/install_and_run_xblock.sh
RUN echo "exec python /usr/local/src/xblock-sdk/manage.py \"\$@\"" >> /usr/local/src/xblock-sdk/install_and_run_xblock.sh
RUN chmod +x /usr/local/src/xblock-sdk/install_and_run_xblock.sh
ENTRYPOINT ["/bin/bash", "/usr/local/src/xblock-sdk/install_and_run_xblock.sh"]
CMD ["runserver", "0.0.0.0:8000"]
