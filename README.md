This a sub-repo of [Neard project](https://github.com/crazy-max/neard) involving MariaDB binary bundles.

## Installation

* Download and install [Neard](https://github.com/crazy-max/neard).
* If you already have installed Neard, stop it.
* Download [a MariaDB bundle](#download).
* Use a file archiver that supports [7z format](http://www.7-zip.org/7z.html) like [7zip](http://www.7-zip.org/) and extract the archive in `neard\bin\mariadb\`.

Directory structure example :
```
[-] neard
 | [-] bin
 |  | [-] mariadb
 |  |  | [-] mariadb5.5.34
 |  |     | neard.conf
 |  |  | [-] mariadb10.1.9
 |  |     | neard.conf
 ```

* Start Neard.
* Switch to the MariaDB version you have extracted on Neard :

![](https://raw.github.com/crazy-max/neard-bin-mariadb/master/img/switchVersion-20151214.png)

## Download

![](https://raw.github.com/crazy-max/neard-bin-mariadb/master/img/star-20151214.png) : Default bundle on Neard.

### 5.5

|                    | MariaDB release date | Neard release | Download |
| ------------------ |:--------------------:|:-------------:|:--------:|
| **MariaDB 5.5.34** ![](https://raw.github.com/crazy-max/neard-bin-mariadb/master/img/star-20151214.png) | 2013/11/21 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-5.5.34-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-5.5.34-r1.zip) |
| **MariaDB 5.5.43** | 2015/05/01 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-5.5.43-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-5.5.43-r1.zip) |
| **MariaDB 5.5.46** | 2015/10/12 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-5.5.46-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-5.5.46-r1.zip) |
| **MariaDB 5.5.48** | 2016/02/11 | [r2](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r2) | [neard-mariadb-5.5.48-r2.7z](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r2/neard-mariadb-5.5.48-r2.7z) |

### 10.0

|                     | MariaDB release date | Neard release | Download |
| ------------------- |:--------------------:|:-------------:|:--------:|
| **MariaDB 10.0.6**  | 2013/11/18 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-10.0.6-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-10.0.6-r1.zip) |
| **MariaDB 10.0.19** | 2015/05/09 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-10.0.19-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-10.0.19-r1.zip) |
| **MariaDB 10.0.22** | 2015/10/29 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-10.0.22-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-10.0.22-r1.zip) |
| **MariaDB 10.0.24** | 2016/02/19 | [r2](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r2) | [neard-mariadb-10.0.24-r2.7z](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r2/neard-mariadb-10.0.24-r2.7z) |

### 10.1

|                     | MariaDB release date | Neard release | Download |
| ------------------- |:--------------------:|:-------------:|:--------:|
| **MariaDB 10.1.9**  | 2015/11/23 | [r1](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r1) | [neard-mariadb-10.1.9-r1.zip](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r1/neard-mariadb-10.1.9-r1.zip) |
| **MariaDB 10.1.13** | 2016/03/25 | [r2](https://github.com/crazy-max/neard-bin-mariadb/releases/tag/r2) | [neard-mariadb-10.1.13-r2.7z](https://github.com/crazy-max/neard-bin-mariadb/releases/download/r2/neard-mariadb-10.1.13-r2.7z) |

## Sources

* https://mariadb.com/

## Contribute

If you want to contribute to this bundle and create new bundles, you have to download [neard-dev](https://github.com/crazy-max/neard-dev) in the parent folder of the bundle.
Directory structure example :

```
[-] neard-dev
 | [-] build
 |  |  | build-commons.xml 
[-] neard-bin-mariadb
 |  | build.xml
```

To create a new bundle :
* Do not forget to increment the `build.release` in the `build.properties` file.
* If you want you can change the `build.path` (default `C:\neard-build`).
* Open a command prompt in your bundle folder and call the Ant target `release` : `ant release`.
* Upload your release on a file hosting system like [Sendspace](https://www.sendspace.com/).
* Create an [issue on Neard repository](https://github.com/crazy-max/neard/issues) to integrate your release.

## Issues

Issues must be reported on [Neard repository](https://github.com/crazy-max/neard/issues).<br />
Please read [Found a bug?](https://github.com/crazy-max/neard#found-a-bug) section before reporting an issue.
