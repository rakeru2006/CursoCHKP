# CheckPoint
Laboratorios para Checkpoint

![Diagrama](https://octodex.github.com/images/yaktocat.png)

Credenciales default (admin/q1w2e3r4)

# Laboratorio 1: Configuracion de direccionamiento IP interno


|Equipo | hostname | IP | Netmask |
|--- | --- | --- | --- |
|Consola | cplabo | 10.0.1.250 | 255.255.255.0 |
|gw1 | fw1 | 10.0.1.251 | 255.255.255.0 |
|gw2 | fw2 | 10.0.1.252 | 255.255.255.0 |
|linux | cliente1 | 10.0.1.10 | 255.255.255.0 |

# Objetivos:

* Configurar las direcciones IP en los equipos de la tabla
* Lograr que ping de la consola a linux responda


# Apendice

## CheckPoint CLI

```
# Mostrar IP
show interface <ifname> ipv4-address

# Configurar IP
set interface <ifname> ipv4-address <ip> mask-leng <mask length>

```

## Configuracion IP Linux

```
# Mostrar
ifconfig <ifname>

# Configurar IP
sudo ifconfig <ifname> <ip> netmask <netmask>
```
