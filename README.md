# docker-fast-cli
Fast.com using a headless docker container that can run on a server without a screen.

# build
```
docker build --tag 'fast-cli' .
```

# run download speed test
```
docker run 'fast-cli'
```

# run download and upload speed test
```
docker run 'fast-cli' fast --upload
```

See the underlying library code for [fast-cli](https://github.com/sindresorhus/fast-cli) for details on how the program works.  All this docker image does is install the necessary puppeteer components like Chrome first before setting up the fast-cli in the container.
