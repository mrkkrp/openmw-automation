# OpenMW Automation

Run like this:

```
$ ansible-playbook -K openmw.yml
```

This [Ansible](https://www.ansible.com/) playbook does the following in
order:

1. Installs dependencies for [OpenMW](https://openmw.org/) using `pacman`
   (I'm on Arch Linux).
2. Grabs, builds, and installs the latest OpenMW trunk.
3. Setups the [Pelagiad](https://github.com/Isaskar/Pelagiad) font, which is
   better for the eyes than Morrowind's “Magic Cards” (the default font).
4. Tweaks the `~/.config/openmw/settings.cfg` the way I like it.

I'm automating this because I like to keep an eye on the engine's latest
developments and experiment with the settings, but I don't like to mess with
this stuff manually every time (for example I had to set Pelagiad font after
every re-build again, not fun!).
