ez-ipupdate Cookbook
====================
Installs the ez-ipdate service under Opscode Chef

Requirements
------------
Platforms: 
Tested on Fedora. May work on other Linux platforms.

Attributes
----------

e.g.
#### ez-ipupdate::default
<table>
  <tr>
    <th>Key</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['package_name']</tt></td>
    <td>Package name</td>
    <td><tt>ez-ipupdate</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['package_config']</tt></td>
    <td>Location of config file</td>
    <td><tt>/etc/ez-ipdate/default</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['username']</tt></td>
    <td>Your provider username</td>
    <td><tt>username</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['password']</tt></td>
    <td>Your DNS update provider password</td>
    <td><tt>password</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['host']</tt></td>
    <td>The hostname of your domain</td>
    <td><tt>host</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['service-type']</tt></td>
    <td>Your service provider name</td>
    <td><tt>provider</tt></td>
  </tr>
  <tr>
    <td><tt>['ez-ipupdate']['interface']</tt></td>
    <td>The ethernet interface of your server or desktop</td>
    <td><tt>eth0</tt></td>
  </tr>
</table>

Usage
-----
#### ez-ipupdate::default

Just include `ez-ipupdate` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[ez-ipupdate]"
  ]
}
```

And then override the attributes.

Contributing
------------
If you wish to contribute:

1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write you change
4. Submit a Pull Request using Github

License and Authors
-------------------
Authors: Rilindo.Foster <rilindo.foster@monzell.com>