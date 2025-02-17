# MyProgram

## Installation Instructions

### Step 1: Generate the configuration script (--install key already containts the aclocal and ### automake --add-missing commands)
```sh
autoreconf --install
```

### Step 2: Configure the build system
```sh
./configure --host=x86_64-pc-linux-gnu
```

### Step 3: Compile the program
```sh
make
```

### Step 4: Install the program
```sh
sudo make install
```

### Step 5: Clean all generated files
```sh
make clean-all
