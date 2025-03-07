---
title: Windows
description: Install Hugo on Windows.
categories: [installation]
menu:
  docs:
    parent: installation
    weight: 40
toc: true
weight: 40
---
{{% readfile file="/installation/_common/01-editions.md" %}}

{{% readfile file="/installation/_common/02-prerequisites.md" %}}

{{% readfile file="/installation/_common/03-prebuilt-binaries.md" %}}

## Package managers

### Chocolatey

[Chocolatey] is a free and open source package manager for Windows. This will install the extended edition of Hugo:

```sh
choco install hugo-extended
```

[Chocolatey]: https://chocolatey.org/

### Scoop

[Scoop] is a free and open source package manager for Windows. This will install the extended edition of Hugo:

```sh
scoop install hugo-extended
```

[Scoop]: https://scoop.sh/

### Winget

[Winget] is Microsoft's official free and open source package manager for Windows. This will install the extended edition of Hugo:

```sh
winget install Hugo.Hugo.Extended
```

[Winget]: https://learn.microsoft.com/en-us/windows/package-manager/

{{% readfile file="/installation/_common/04-docker.md" %}}

{{% readfile file="/installation/_common/05-build-from-source.md" %}}

{{% note %}}
See these [detailed instructions](https://discourse.gohugo.io/t/41370) to install GCC on Windows.
{{% /note %}}

## Comparison

||Prebuilt binaries|Package managers|Docker|Build from source
:--|:--:|:--:|:--:|:--:|:--:
Easy to install?|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|
Easy to upgrade?|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:
Easy to downgrade?|:heavy_check_mark:|:heavy_check_mark: [^2]|:heavy_check_mark:|:heavy_check_mark:
Automatic updates?|:x:|:x: [^1]|:x: [^1]|:x:
Latest version available?|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:

[^1]: Possible but requires advanced configuration.
[^2]: Easy if a previous version is still installed.
