1. [Documentation](#documentation)
1. [Linux Support](#linux-support)
1. [Windows Support](#windows-support)
1. [Contributing](#contributing)

## Documentation

Some distribution have special requirements for our Icinga packages, see the OS
directories above for details.

Please make sure to check the [Icinga Documentation] for the product you want to use:

* [Icinga 2](https://www.icinga.com/docs/icinga2/latest)
* [Icinga Web 2](https://www.icinga.com/docs/icingaweb2/latest)

## Linux Support

Icinga tries to support a lot of Linux distributions in order for you
to use Icinga where you want.

Check the matrix below about what distributions are supported with
which Icinga version.

If a concrete version number is mentioned, this means that the product won't be updated
to latest version on this platform. Consider updating your OS release.

| OS       | Version      | Core 2   | Web 2    | PHP        | OS Support    |
|----------|--------------|----------|----------|------------|---------------|
| EPEL     | 6            | *latest* | *latest* | 7.0-SCL [[9]] / 5.3 [[11]] | 2020-11 [[1]] |
| EPEL     | 7            | *latest* | *latest* | 7.1-SCL [[10]] / 5.4 [[12]] | 2024-06 [[1]] |
| Debian   | 7 wheezy     | *latest* | 2.4.2    | 5.4 [[13]] | 2018-05 [[2]] |
| Debian   | 8 jessie     | *latest* | *latest* | 5.6 [[13]] | 2020-04 [[2]] |
| Debian   | 9 stretch    | *latest* | *latest* | 7.0 [[14]] | 2022-06 [[2]] |
| Ubuntu   | 14.04 trusty | *latest* | 2.4.2    | 5.5 [[15]] | 2019-06 [[3]] |
| Ubuntu   | 16.04 xenial | *latest* | *latest* | 7.0 [[16]] | 2021-03 [[3]] |
| Ubuntu   | 17.04 zesty  | *latest* | *latest* | 7.0 [[16]] | 2017-12 [[3]] |
| Ubuntu   | 17.10 artful | *latest* | *latest* | 7.1 [[17]] | 2018-06 [[3]] |
| Fedora   | 25           | *latest* | *latest* | 7.0 [[18]] | 1m after 27 [[6]] |
| Fedora   | 26           | *latest* | *latest* | 7.1 [[19]] | 1m after 28 [[6]] |
| SUSE SLE | 11.4         | *latest* | 2.4.2    | 5.2 [[20]] | 2019-03 [[4]] |
| SUSE SLE | 12.2         | *latest* | *latest* | 7.0/5.5 * [[22]] | 2018-03 [[4]] |
| SUSE SLE | 12.3         | *latest* | *latest* | 7.0/5.5 * [[22]] | TDB [[4]]     |
| openSUSE | 42.2         | *latest* | *latest* | 7.0/5.5 [[21]] | 2018-01 [[5]] |
| openSUSE | 42.3         | *latest* | *latest* | 7.0/5.5 [[21]] | 2019-01 [[5]] |

* EPEL: RedHat Enterprise / CentOS (and derivatives) + EPEL repository enabled
* OS Support End is for the target distribution (and regular LTS)
  (payed additional update support is excluded)
* Icinga Support cycle might not be the same as the distribution itself
* PHP on SUSE SLE 12 needs a special add-on module "Web and Scripting Module"

### Out of support

The following releases are out of our support, please check the last
available version for that release from the table below.

| OS       | Version      | Icinga 2 | Icinga Web 2 | OS Support    |
|----------|--------------|----------|--------------|---------------|
| EPEL     | 5            | 2.6.3    | -            | 2017-03 [[1]] |
| Debian   | 6 squeeze    | 2.4.1    | -            | 2016-02 [[2]] |
| Ubuntu   | 12.04 precise| 2.6.2    | 2.3.4        | 2017-06 [[3]] |
| Ubuntu   | 15.04 vivid  | 2.4.1    | 2.3.4        | 2016-01 [[3]] |
| Ubuntu   | 15.10 wily   | 2.4.10   | 2.3.4        | 2016-06 [[3]] |
| Ubuntu   | 16.10 yakkety| 2.7.1    | 2.4.2        | 2017-06 [[3]] |
| openSUSE | 13.2         | 2.6.3    | 2.4.1        | 2017-01 [[5]] |
| openSUSE | 42.1         | 2.6.3    | 2.4.1        | 2017-05 [[5]] |

### Upcoming Releases

| OS       | Version      | Icinga 2 | Icinga Web 2 | OS Support        |
|----------|--------------|----------|--------------|-------------------|
| Fedora   | 27           | TODO     | TODO         | 1m after 29 [[6]] |

## Windows Support

Windows is only supported for Icinga 2 as a client/agent.

Supported is:
* Windows Vista/Server 2008 or higher
* Microsoft .NET Framework 2.0 for the setup wizard

Please see the [Icinga 2 documentation on Windows](https://www.icinga.com/docs/icinga2/latest/doc/06-distributed-monitoring/#client-setup-on-windows).

## Contributing

You can find our packaging files and scripts on [Icinga GitHub].

If you experience any issues with the packages themselves, please report an issue against [icinga-packaging].

Other problems regarding the products can be reported on GitHub as well:

* [Icinga 2](https://github.com/icinga/icinga2)
* [Icinga Web 2](https://github.com/icinga/icingaweb2)

[Icinga Documentation]: https://www.icinga.com/docs/
[Icinga GitHub]: https://github.com/Icinga
[icinga-packaging]: https://github.com/icinga/icinga-packaging

[1]: https://access.redhat.com/support/policy/updates/errata#Life_Cycle_Dates
[2]: https://wiki.debian.org/LTS
[3]: https://www.ubuntu.com/info/release-end-of-life
[4]: https://www.suse.com/lifecycle/
[5]: https://en.opensuse.org/Lifetime
[6]: https://fedoraproject.org/wiki/Fedora_Release_Life_Cycle#Maintenance_Schedule

[9]: http://mirror.centos.org/centos/6/sclo/x86_64/rh/rh-php70/
[10]: http://mirror.centos.org/centos/7/sclo/x86_64/rh/rh-php71/
[11]: http://mirror.centos.org/centos/6/os/x86_64/Packages/
[12]: http://mirror.centos.org/centos/7/os/x86_64/Packages/
[13]: https://tracker.debian.org/pkg/php5
[14]: https://tracker.debian.org/pkg/php7.0
[15]: https://launchpad.net/ubuntu/+source/php5
[16]: https://launchpad.net/ubuntu/+source/php7.0
[17]: https://launchpad.net/ubuntu/+source/php7.1
[18]: https://mirrors.n-ix.net/fedora/linux/releases/25/Server/source/tree/Packages/p/
[19]: https://mirrors.n-ix.net/fedora/linux/releases/26/Server/source/tree/Packages/p/
[20]: https://www.suse.com/LinuxPackages/packageRouter.jsp?product=server&version=11&service_pack=sp2&architecture=x86_64&package_name=php5
[21]: https://software.opensuse.org/package/php7
[22]: https://www.suse.com/de-de/products/server/features/modules/#TODO
