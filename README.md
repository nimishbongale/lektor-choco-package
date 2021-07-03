# Lektor Chocolatey Package

Lektor "Chocolatey" Package is the community driven package for installing and running the [Lektor CMS](https://www.getlektor.com/) on Windows OS. 

See the package in action here: [https://chocolatey.org/packages/lektor](https://chocolatey.org/packages/lektor)

///////////////TODO - BADGES///////////////

## Installation

The [Chocolatey CLI]() will be needed as a primary requirement.

To install the latest package from [chocolatey](https://chocolatey.org):

```powershell
choco install lektor
```

For a specific version:

```powershell
choco install lektor@123 ////////////////TODO - VERSION//////////////////
```

## Usage

To run the package from this repository directly, run these commands:

```powershell
git clone https://github.com/nimishbongale/chocolatey-lektor-package.git
cd chocolatey-lektor-package
choco pack
choco install -fdv 
```

To make & push the updated package to chocolatey (not for community use!):

```powershell
choco pack
choco apikey --key <apikey> --source https://push.chocolatey.org/
choco push lektor.<version>.nupkg --source https://push.chocolatey.org/
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
