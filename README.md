## pgloader
```
docker build -t mabden/pgloader:latest -f pgloader.dockerfile .
docker push mabden/pgloader:latest
docker run -i -t mabden/pgloader pgloader mysql://root@host.docker.internal:3306/mysql postgresql://postgres@host.docker.internal:5432/postgres 
```