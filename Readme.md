# Installation

```
cd /path/where/you/want/the/repository

# clone the repository
git clone https://github.com/xianzhon/i3.git i3
cd i3

# compile & install
autoreconf --force --install
rm -rf build/
mkdir -p build && cd build/

# Disabling sanitizers is important for release versions!
# The prefix and sysconfdir are, obviously, dependent on the distribution.
../configure --prefix=/usr --sysconfdir=/etc --disable-sanitizers
make
sudo make install
```

Refer to:  
[i3 gaps installation guide](https://github.com/Airblader/i3/wiki/Compiling-&-Installing)
