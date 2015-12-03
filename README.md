# Jetty Ansible Role

Installs and configures Jetty.

# Configuration Options

Name          | Default              | Description
--------------|----------------------|------------------------------------------------------------------------------
java_options  | null                 | Extra options to pass to the JVM
jetty_base    | /opt/jetty/demo-base | Location for your configurations and customizations to the Jetty distribution
jetty_home    | /opt/jetty           | Location for the Jetty distribution binaries / Install directory
jetty_version | 9.3.6.v20151106      | Jetty version that will be installed

# Usage example

```yaml
---
- hosts: all
  sudo: true
  roles:
    - role: jetty
      java_options: -Xms1024m -Xmx1024m
      jetty_base: /home/user/application
```

# License

[![GPLv3](http://www.gnu.org/graphics/gplv3-127x51.png)](http://www.gnu.org/licenses/gpl-3.0.html)
