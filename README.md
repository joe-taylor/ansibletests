# Ansible Tests

This repo is a storehouse for a random assortment of Ansible playbooks; mainly
works in progress or feature demos/tests. Each folder is a self-contained
suite of one or more playbooks, and should also include a Vagrantfile to spin
up at least one host in which to run aforementioned playbooks.

Because this repository was created for learning purposes, the playbooks may
be contrived to try out some ansible features. You are unlikely to find much
of actual practical value, unless you're learning ansible too.

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
