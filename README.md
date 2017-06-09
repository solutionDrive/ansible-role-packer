Role Name
=========
Install packer on mac os

Requirements
------------
none

Role Variables
--------------

``` 
packer_install_version: "1.0.0"
```
Version which should be installed

```
packer_download_destination: "/tmp/packer_{{ packer_install_version }}.zip"
```
Path which will be used to download Packer

``` 
packer_unarchive_destination: "/tmp/packer/"
```
Path which will be used to extract downloaded archive

```
packer_execution_path: "/usr/local/bin/packer"
```
Path which will be used to move the extracted file and make it executable

```
packer_releases_url: "https://releases.hashicorp.com/packer/{{ packer_install_version }}/packer_{{ packer_install_version }}_darwin_amd64.zip"
```
Url to download packer

Dependencies
------------
None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: 127.0.0.1
      connection: local
      roles:
         - { role: solutionDrive.packer }

License
-------
MIT/BSD

Author Information
------------------

This role was created by [solutionDrive](http://solutiondrive.de)
