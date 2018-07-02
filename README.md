# Debian image for Molecule

This [Docker](https://www.docker.com) image can be used to test [Ansible](https://www.ansible.com) playbooks based on [Molecule](https://molecule.readthedocs.io/en/latest/).

## Supported tags

* 8
* 9

## Usage

Run the container as a daemon

```console
docker run --cap-add SYS_ADMIN --detach --name debian-9 --rm --volume /sys/fs/cgroup:/sys/fs/cgroup:ro dhoppe/molecule-debian:9
```

Enter the container

```console
docker exec -it debian-9 bash
```

Stop the container

```console
docker stop debian-9
```