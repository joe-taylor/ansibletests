# Ansible Tests

This is a storing house for my random assortment of test playbooks. Each
folder is a self-contained ansible environment containing a collection of one
or more playbooks, and each folder includes a Vagrantfile to spin up at least
one host in which to run aforementioned playbooks.

## Usage

cd into a directory, follow any applicable instructions (if present in the
associated README), and then run `vagrant up`. Use `vagrant ssh` to inspect
what's been provisioned in that folder's vm. Finally, use `vagrant
destroy -f` to destroy the vms when you're finished.

e.g.

    cd addpublickeys
    vagrant up

Then loop between `vagrant ssh` and `vagrant provision` as necessary before
running `vagrant destroy -f`.
