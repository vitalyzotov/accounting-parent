# accounting-parent

## Module dependencies

See docs/modules

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

    gh release create 2.0 -t v2.0 --generate-notes

#### Wait until the release is published

    gh run watch

#### Checkout tagged repo

    git checkout 2.0
