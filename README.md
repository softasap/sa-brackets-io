sa-brackets-io
==============

[![Build Status](https://travis-ci.org/softasap/sa-brackets-io.svg?branch=master)](https://travis-ci.org/softasap/sa-brackets-io)

Example of use:

- hosts: dev

  vars:
    - root_dir: "{{playbook_dir}}/../"


  pre_tasks:
    - debug: msg="Pre tasks section"

  roles:

    - {
        role: "sa-brackets-io"
      }


  tasks:
    - debug: msg="Tasks section"



Possible overrides:

  brackets_io_version: X.X  - defaults to 1.6

