# ssnaps
Tool to simplify snapshot management and remote backup using libbtrfsutil.

# Features
* None

# Coming soon
* No ID abstraction, commands use the same IDs as btrfs itself.
* Fast(er) comparison mode just showing additions and deletions.
* Difference in pairs between _n_ snapshots either by id or name.
* Fast space-usage estimates.
* Preservation of exclusive monthly, weekly, daily, and recent snapshots and / or backups.
* Remove snapshots when free space under an amount or over a percentage of use.
* Backups.
* Documentation.
* Configs.
* Systemd units.
* Rollback of any subvolume either via set/get default or by namechange.
* all-in-one application.
* btrfs-progs style interface (e.g. ssnaps [[[[[[[c]o]m]p]a]r]e] for ssnaps compare)
* Reduced set of snapshot types, no pre-post / number - ssnaps will only manage backups, timeline, and read-write snapshots.
* snapper conversion.
* man page
* help
* undochange that reflinks

# Eventually?
* GUI for rollback, comparisons etc.
* gettext translations.
* zfs support.
* bcachefs support.
* cron support.
* sudo alt support (doas?)

# Setup
* Subvolume mounted at .snapshots directory.
* Remote snapshots require user account on backup system with sudo btrfs access for particular jobs / locations and key-based login.
* Uses pv if available.
