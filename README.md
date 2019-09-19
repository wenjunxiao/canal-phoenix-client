# canal-phoenix-client

Repackage the phoenix client to apply to alibaba canal.
Remove or relocation the confict packages.

## Compile

Download the special version of phoenix from [https://phoenix.apache.org/download.html](https://phoenix.apache.org/download.html).

```bash
$ export PHOENIX_VERSION=4.14.0-HBase-1.2
$ wget http://archive.apache.org/dist/phoenix/apache-phoenix-$PHOENIX_VERSION/bin/apache-phoenix-$PHOENIX_VERSION-bin.tar.gz
$ tar -xzf apache-phoenix-$PHOENIX_VERSION-bin.tar.gz
$ mkdir -p repo/org/apache/phoenix/phoenix-client/$PHOENIX_VERSION
$ cp apache-phoenix-$PHOENIX_VERSION-bin/phoenix-$PHOENIX_VERSION-client.jar repo/org/apache/phoenix/phoenix-client/$PHOENIX_VERSION/phoenix-client-$PHOENIX_VERSION.jar
$ mvn clean package
```