# Aerospike exporter for Prometheus (Docker)
This is a docker version of Aerospike exporter for Prometheus.

It's a docker wrapper of [alicebob/asprom](https://github.com/alicebob/asprom)

Using base image：[golang](https://hub.docker.com/_/golang/)

## Usage

Default will fetch aerospike data from `127.0.0.1:3000` and export metrics on `port: 9145`

`docker run --net=host --name aerospike_exporter ysde/aerospike_exporter `

or specify the address and port you want to listen and export to

`docker run --name aerospike_exporter ysde/aerospike_exporter -listen :9999 -node 10.x.x.x`
