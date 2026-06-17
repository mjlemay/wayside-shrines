# Wayside Shrines

A puzzle experience built around trigger volumes as the core mechanic.

## CHECK OUT THESE COOL TOOLS THAT I AM USING!!
- [Hytale Plugin Template](https://github.com/HytaleModding/plugin-template)
- [Hytale Gradle Plugin](https://github.com/AzureDoom/Hytale-Gradle-Plugin),


## How to start

Run the local development server:

   ```bash
   ./gradlew runServer
   ```

## Useful commands

```bash
# Sync/setup the local Hytale development environment
./gradlew setupHytaleDev

# Run the local Hytale server
./gradlew runServer

# Run the server with debugging and hot swap enabled
./gradlew runServer -Ddebug=true -Dhotswap=true

# Check your JVM and hot swap setup
./gradlew hytaleJvmDoctor

# Build the plugin
./gradlew build

# Refresh dependencies if something fails to resolve
./gradlew build --refresh-dependencies
```

## Project structure

```text
src/main/java/        Plugin source code
src/main/resources/   Plugin resources, including manifest.json
gradle.properties     Main template configuration
build.gradle.kts      Gradle build and Hytale Gradle Plugin configuration
settings.gradle.kts   Plugin repositories and project name
```

## Manifest configuration

The generated `manifest.json` is driven by the values in `gradle.properties`, including:

- `manifest_group`
- `mod_id`
- `version`
- `mod_description`
- `mod_author`
- `mod_url`
- `main_class`
- `manifest_dependencies`
- `manifest_opt_dependencies`
- `manifestServerVersion`

After changing these values, run:

```bash
./gradlew updatePluginManifest
```


## License

MIT is OPP Yeah you know me!
