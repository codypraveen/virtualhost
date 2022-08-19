Virtualhost Manage Script
===========

Bash Script to create or delete apache virtual hosts in Ubuntu quickly.

## Installation ##

1. Download the script
2. Optional: if you want to use the script globally, then you need to copy the file to your /usr/local/bin directory, is better
if you copy it without the .sh extension:

```bash
sudo cp /path/to/virtualhost.sh /usr/local/bin/virtualhost
```

3. Apply permission to execute:
```
chmod +x /usr/local/bin/virtualhost
```

## Usage ##

With script installed on /usr/local/bin

```bash
sudo virtualhost [create | delete] [domain] [optional root_dir]
```

Basic command line syntax:

```bash
sudo sh /path/to/virtualhost.sh [create | delete] [domain] [optional root_dir]
```

### Examples ###

to create a new virtual host:

```bash
sudo virtualhost create mysite.dev
```
to create a new virtual host with custom directory name:

```bash
sudo virtualhost create anothersite.dev root_dir
```
to delete a virtual host

```bash
sudo virtualhost delete mysite.dev
```

to delete a virtual host with custom directory name:

```
sudo virtualhost delete anothersite.dev root_dir
```
