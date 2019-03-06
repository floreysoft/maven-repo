# Maven internal repository

```
<repositories>

    <repository>
        <id>floreysoft-releases</id>
        <url>https://github.com/floreysoft/maven-repo/raw/master/releases</url>
    </repository>

    <repository>
        <id>floreysoft-snapshots</id>
        <url>https://github.com/floreysoft/maven-repo/raw/master/snapshots</url>
    </repository>

<repositories>

```

## Publishing to maven repo:

- Clone the [maven-repo](https://github.com/floreysoft/maven-repo) project on the same folder level of this project.

- Run **yarn deploy** on the module you want to publish. This will deploy to the maven-repo only on local machine. Changes will still be pending.

## Publishing Snapshots:

- Deploy with -SNAPSHOT appended to project version

- Push changes to maven-repo to github.


## Publishing Releases:

- Remove the -SNAPSHOT tail from project version

- Tag and commit the code

- Deploy to local maven-repo

- Push changes to github
