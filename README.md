nginx
=====
Installs `nginx` and its config files. The default site config template is for a Django site.

Role Variables
==============
| Variable | Description | Default value |
|----------|-------------|---------------|
|`nginx_access_log`| Name of the access log file | `{{ nginx_server_name }}.access.log` |
|`nginx_conf_file` | Path to the nginx config template | `nginx.conf` |
|`nginx_error_log` | Name of the error log file | `{{ nginx_server_name }}.error.log` |
|`nginx_server_name` | Value of `server_name` directive in virtual host config | `none` |
|`nginx_static_path` | Path to static files | `none` |
|`nginx_templates_path` | Path to Django site templates | `none` |
|`nginx_vhost_conf_src` | Path to the virtual host config template | `vhost.conf.j2` |

Dependencies
============
none

License
=======
BSD
