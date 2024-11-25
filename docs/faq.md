---
sidebar_position: 5
---

# Frequently Asked Questions


## Known Issues

### basename

basename is used when files are created/uploaded. this function is local aware. the matching locale is not being set yet, this might lead to issues with multibyte character paths (filesplus won't allow you to create a file if the characters are invalid for the current locale) https://www.php.net/manual/en/function.basename.php

### File / Database synchronisation

If a filesystem operation is made (e.g. moving a file) but the database operation fails for some reason, then the file is moved in the filesystem but not in the database. If this happens, the only way to fix this would be to rescan all files.