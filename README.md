# Water Walking — NeoForge 1.21.1

A standalone port of Cyclic 1.12.2's Waterwalking potion/effect for Minecraft 1.21.1 and NeoForge 21.1.263.

## Behavior

- 3-minute Waterwalking potion effect.
- Prevents downward movement while walking above a water block, when the space at the entity's feet is air.
- Sneaking allows a player to sink.
- Uses the original Cyclic Waterwalking icon.
- Brewing recipe: Awkward Potion + Cod -> Waterwalking Potion.

## Build locally

Requires Java 21 and internet access for Gradle/Minecraft/NeoForge dependencies.

- Linux/macOS: `./gradlew --no-daemon build`
- Windows: `gradlew.bat --no-daemon build`

The mod JAR is written to `build/libs/`.

## Build without a computer (GitHub Actions)

This repository includes `.github/workflows/build.yml` so GitHub Actions can build the JAR in the cloud. Upload the contents of this project to a GitHub repository, open the **Actions** tab, select **Build Water Walking**, and run the workflow. After it finishes, open its run and download the `waterwalking-neoforge-1.21.1` artifact. This requires a GitHub account and access to create a repository/run Actions.

## Status

The source and workflow are prepared, but this environment cannot download Gradle from `services.gradle.org`, so compilation has not been verified here. The cloud workflow is included as an alternative build route.
