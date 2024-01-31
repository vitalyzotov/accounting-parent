# accounting-parent

## Module dependencies

![](http://www.plantuml.com/plantuml/svg/3Sf13W8n20NGg-W1B7jlWxIP8Q7GqCyOFRs-zRkhYrKVbNOxWRMVHCdlTYZEUjKUAU4OZYOnwLAmVRw1k8X5eXpgnsDn_WTDLgSUGZDwsTXjrRGV)

## Development workflow

#### Checkout main (master) branch of module

```shell
cd <module>
git checkout main
```

Git will merge any local changes.

#### Replace SNAPSHOT versions in pom.xml

#### Create release tag

    mvn gitflow:release

#### Create GitHub release

```powershell
$tag=git describe --tags --abbrev=0;gh release create "$tag" -t "v$tag" --generate-notes
```


#### Wait until the release is published

    gh run watch

#### Checkout tagged repo

    git checkout 2.0
