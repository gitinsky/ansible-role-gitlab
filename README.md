Installation based on [official](https://about.gitlab.com/downloads/) instructions.

Tested on ubuntu 14.04.

WARNING: by default gitlab is [configured](http://doc.gitlab.com/omnibus/settings/nginx.html) to http protocol, you must not use it for authorisation.

Username: root 
Password: 5iveL!fe

Variables and there default values:
- gitlab_enable_configuration: yes # set to 'no' to disable configuration and install package with default gitlab values
- gitlab_url: "http://{{ ansible_default_ipv4.address }}"
- gitlab_email_from: "gitlab@{{ ansible_fqdn }}"
- gitlab_email_display_name: Gitlab

Gitlab CI variables are ignored for now.
