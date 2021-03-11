[![Java CI with Gradle](https://github.com/MineInAbyss/KotlinSpice/actions/workflows/gradleci.yml/badge.svg)](https://github.com/MineInAbyss/KotlinSpice/actions/workflows/gradleci.yml)
[![Package](https://badgen.net/maven/v/metadata-url/repo.mineinabyss.com/releases/com/mineinabyss/kotlinspice/maven-metadata.xml)](https://repo.mineinabyss.com/releases/com/mineinabyss/kotlinspice)

# KotlinSpice
A platform for common libraries for our Minecraft plugins.

Save a lot of disc space and a tree. We plan on switching to [PDM](https://github.com/knightzmc/pdm/) when more features are added.

## Usage

### Gradle

```groovy
repositories {
    maven  { url 'https://repo.mineinabyss.com/releases' }
}

dependencies {
    compileOnly platform("com.mineinabyss:kotlinspice:$kotlinVersion+")
    //Add optional deps without specifying a version!
    //(The appropriate repo must still be provided for them)
    compileOnly "com.github.okkero:skedule"
    compileOnly "de.erethon:headlib"
}
```

