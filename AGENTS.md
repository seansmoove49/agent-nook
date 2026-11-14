# Ownership

Machine-wide installations and machine settings belong in macbook-nook.
Repository-local dependencies belong in the repository that uses them.
Manage each installation in one place only.

This repository owns plugins, skills, icons, marketplace catalogs, and its local
maintenance tools. The skills CLI is a pinned npm development dependency here;
use the local installation rather than installing it globally.
