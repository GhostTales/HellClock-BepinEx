## Installation

### 1. Locate the Hell Clock installation folder

Download or clone this repository, then copy its files into your Hell Clock installation directory.

**Linux**
```text
/home/GhostTales/.local/share/Steam/steamapps/common/Hell Clock/
```

**Windows**
```text
C:\Program Files (x86)\Steam\steamapps\common\Hell Clock
```

Alternatively, you can find the folder through Steam:

1. Open your Steam Library.
2. Right-click **Hell Clock**.
3. Select **Manage → Browse Local Files**.

### 2. Create the plugins folder

The repository does not include the `plugins` folder, so you must create it manually if it doesn't already exist.

Create the following directory inside your Hell Clock installation:

```text
BepInEx/plugins/
```

### 3. Install mods

Once the `plugins` folder is in place, install your mods by placing their files inside it.

Your directory structure should look something like this:

```text
Hell Clock/
└── BepInEx/
    └── plugins/
        ├── Mod1/
        ├── Mod2.dll
        └── ...
```

## Linux: Steam Launch Options

Linux users must configure Steam to load the required Windows DLL override.

1. Open your Steam Library.
2. Right-click **Hell Clock** and select **Properties**.
3. Under **General**, find **Launch Options**.
4. Add the following command:

```bash
WINEDLLOVERRIDES="winhttp=n,b" %command%
```

Launch the game through Steam after completing the setup.
