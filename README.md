## Usage
Run it using
```
docker run -h pyro -v <local-opendreambox>:/oe -v <local-path-of-home>:/home -u oe -it opendreambox/build:pyro
```

If the mounted /oe has no opendreambox pyro, you can start with something like this

```
cd /oe
git clone https://github.com/opendreambox/opendreambox.git -b pyro pyro
cd pyro
make image MACHINE=<dreamone|dreamtwo>
```

