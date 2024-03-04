# Software Versioning

Versioning is a critical aspect of software development. It is the process of assigning identifiers to a package to distinguish it from other versions of the same package. In contrast to a "git hash", which serves as an immutable machine-friendly identifier of the state of the software, the version number serves more to communicate the function of the package to (human) users. This document outlines our practices for versioning a package.

## Semantic Versioning

Semantic versioning (SemVer) is a versioning scheme that provides a simple set of rules and requirements that dictate how version numbers are assigned and incremented. The version number is a three-part number in the format of `MAJOR.MINOR.PATCH`.
- `MAJOR` version when you make incompatible API changes,
- `MINOR` version when you add functionality in a backwards-compatible manner, and
- `PATCH` version when you make backwards-compatible bug fixes, or maintenance/ upkeep and other developer-facing improvements.


## Calender Versioning

Calender versioning (CalVer) is a versioning scheme that uses some portion of the date of release as the version number. There are different styles of CalVer. One is very similar to SemVer, however the `MAJOR` version is instead replaced with the year of release, e.g. `YYYY.MINOR.PATCH`. Other variants can be found here: [CalVer](https://calver.org/).

## R Packages

R packages should be versioned using a Semantic Versioning (SemVer) compliant variant as described in the [R package versioning guide](https://r-pkgs.org/release.html#release-version).

This means, either standard SemVer, or the CalVer variant as described above. This may be the case, for example, in packages who's primary exported outputs are data, and the package is updated on a regular schedule.

## Other Repositories

At this stage, no clear guidance is given for other `RMI-PACTA` repositories. In general, some consistent tagging system may be useful (e.g. tag relevant images with `date-built`, or `COP CH 2024`, or other useful user-facing tags), but the specifics of this are left to the discretion of the repository maintainers.

## References

- [Semantic Versioning](https://semver.org/)
- [Calender Versioning](https://calver.org/)

## How

-   [R package versioning guide](https://r-pkgs.org/release.html#release-version).
