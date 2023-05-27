# accounting-parent

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

    gh release create 1.1 -t v1.1 --generate-notes

#### Wait until the release is published

    gh run watch


