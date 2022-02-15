# CPU-cli

CPU-cli is a simple command-line utility to manage CPU settings.
The usage is very simple:
* `# cpu --governor <governor>` or `# cpu -g <governor>` – set the CPU governor
* `# cpu --minfreq <minfreq>` or `# cpu -l <minfreq>` – set the CPU minimum frequency
* `# cpu --maxfreq <maxfreq>` or `# cpu -h <maxfreq>` – set the CPU maximum frequency

## (Un)Installation
### Universal
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Git clone the repository.
* `$ git clone https://github.com/Amarakon55/cpu-cli`
2. Change working directory to *cpu-cli*.
* `$ cd cpu-cli`
3. Install CPU-cli using the Makefile
* `# make install`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Change working directory to *cpu-cli*.
* `$ cd cpu-cli`
2. Uninstall CPU-cli using the Makefile
* `# make uninstall`

### Gentoo
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Add my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using [eselect-repository](https://packages.gentoo.org/packages/app-eselect/eselect-repository)
* `# eselect repository add amarlay git https://github.com/Amarakon55/amarlay`
2. Sync my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using `emerge`
* `# emerge --sync amarlay`
3. Emerge the CPU-cli package
* `# emerge sys-apps/cpu-cli` or `# emerge cpu-cli`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Unmerge the CPU-cli package
* `# emerge -c sys-apps/cpu-cli` or `# emerge -c cpu-cli`
2. (Optional) Remove my overlay
* `# eselect-repository remove -f amarlay`
3. (Optional) Sync using `emerge`
* `# emerge --sync`
