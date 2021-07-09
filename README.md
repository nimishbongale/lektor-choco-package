# Lektor Chocolatey Package

![https://img.shields.io/badge/hosted%20on-chocolatey-brown](https://img.shields.io/badge/hosted%20on-chocolatey-brown)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
![https://img.shields.io/chocolatey/dt/lektor](https://img.shields.io/chocolatey/dt/lektor)
![https://img.shields.io/github/workflow/status/nimishbongale/lektor-choco-package/main](https://img.shields.io/github/workflow/status/nimishbongale/lektor-choco-package/main)


Lektor "Chocolatey" Package is a community driven package for installing and running the [Lektor CMS](https://www.getlektor.com/) on Windows. 

See the package in action here: [https://chocolatey.org/packages/lektor](https://chocolatey.org/packages/lektor)

## Installation

The [Chocolatey CLI](https://docs.chocolatey.org/en-us/choco/) will be needed as a primary requirement.

To install the latest package from [chocolatey](https://chocolatey.org): 

```powershell
choco install lektor
```

For a specific version:

```powershell
choco install lektor --version=3.2.0
```

To uninstall:

```powershell
choco uninstall lektor
```

## Usage

To run the package from this repository directly, run these commands:

```powershell
git clone https://github.com/nimishbongale/chocolatey-lektor-package.git
cd chocolatey-lektor-package
choco pack
choco install -fdv lektor.<version>.nupkg 
```

To make & push the updated package to chocolatey (strictly not for community use!):

```powershell
choco pack
choco apikey --key <apikey> --source https://push.chocolatey.org/
choco push lektor.<version>.nupkg --source https://push.chocolatey.org/
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
