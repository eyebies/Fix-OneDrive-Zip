# Fix-OneDrive-Zip

![Linux build](https://github.com/pmqs/Fix-OneDrive-Zip/workflows/Linux%20build/badge.svg)
![Macos build](https://github.com/pmqs/Fix-OneDrive-Zip/workflows/Macos%20build/badge.svg)
![Windows build](https://github.com/pmqs/Fix-OneDrive-Zip/workflows/Windows%20build/badge.svg)

Fix OneDrive/Windows Zip files larger than 4Gig that have an invalid `Total
Number of Disks` field in the `ZIP64 End Central Directory Locator`. The
value in this field should be 1, but OneDrive/Windows sets it to 0. This
makes it difficult to work with these files using standard unzip utilities.

This program changes the `Total Number of Disks` field value to 1.

## Usage

    fix-onedrive-zip [--dry-run] file1.zip [file2.zip...]

## Support

https://github.com/pmqs/Fix-OneDrive-Zip/issues


## Copyright

Copyright (c) 2020 Paul Marquess (pmqs@cpan.org). All rights reserved.

This program is free software; you can redistribute it and/or modify it
under the same terms as Perl itself.
