# RubyDung rd-132211

This is a decompiled Java project for the old Minecraft/RubyDung `rd-132211`
build. It uses LWJGL 2, so it needs the matching LWJGL 2 jars and native DLLs.

## IntelliJ Setup

Open this folder as the IntelliJ project:

```text
C:\Users\zeera\AppData\Roaming\PrismLauncher\libraries\com\mojang\minecraft\rd-132211\src
```

The project is configured with:

- Main class: `com.mojang.rubydung.RubyDung`
- Working directory: `$PROJECT_DIR$`
- Native library path: `$PROJECT_DIR$\natives`
- LWJGL jars from `$PROJECT_DIR$\lib`

Use the included `RubyDung` run configuration from the IntelliJ run dropdown.

## Java Version

LWJGL 2 is old and works best with Java 8. A portable Java 8 JDK zip can live in
the project root, and the extracted copy can be used by IntelliJ.

If IntelliJ does not auto-detect the local JDK, add it manually:

1. Open **File > Project Structure > Platform Settings > SDKs**.
2. Click **+ > Add JDK**.
3. Select:

```text
$PROJECT_DIR$\jdk8
```

4. Set the project SDK to that Java 8 SDK.

## Files

- `level.dat` stores the current world.
- `terrain.png` is loaded as a classpath resource.
- `lib` contains the LWJGL 2 jars used at compile time.
- `natives` contains extracted LWJGL 2 Windows DLLs.
