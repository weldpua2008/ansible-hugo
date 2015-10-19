[![Build Status](https://travis-ci.org/weldpua2008/ansible-hugo.svg)](https://travis-ci.org/weldpua2008/ansible-hugo)
Role Name
=========

Ansible role to install HUGO - Fast and Flexible Static Site Generator http://gohugo.io/ 
![Hugo](https://raw.githubusercontent.com/spf13/hugo/master/docs/static/img/hugo-logo.png)

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

*   `hugo_url`: full path to artifact in  - https://github.com/spf13/hugo/releases: `https://github.com/spf13/hugo/releases/download/v0.14/hugo_0.14_amd64.deb`
*   `hugo_version`: `0.14` (See new versions on hugo_version)
*   `hugo_os`: `by default "linux"` is used for filename 
*   `hugo_extention`: (By default "tar.gz" https://github.com/spf13/hugo/releases/download/v0.14/hugo_0.14_amd64`.tar.gz`)
*   `hugo_dest_dir`: "/opt/hugo"
*   `hugo_bin_dir`: "/opt/hugo/bin"
*   `hugo_temp_dir`: "/tmp"

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: static-web-servers
      roles:
         - { role: weldpua2008.hugo, hugo_version: "0.14" }

License
-------
MIT
BSD

Author Information
------------------

Valeriy Solovyov (weldpua2008@gmail.com)
