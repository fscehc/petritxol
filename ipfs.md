# Gateway IPFS

[Català, Español, English]

## [Català] Com muntar un gateway IPFS

Necessitem:

    - Un servidor, amb mínim **512mb** de **RAM** i **5 gigabytes de disc**.
    - Un domini que apunti a la IP del nostre servidor
    - Una distribució Linux recent: **Debian**, **CentOS 7**, **Ubuntu**, etc.
    - El port **HTTPS (443)** accessible des d'**Internet**

El primer pas és instal.lar Docker, que es fa en pocs passos seguint aquesta guia:

- **Debian**: https://docs.docker.com/engine/installation/linux/docker-ce/debian/
- **Centos**: https://docs.docker.com/engine/installation/linux/docker-ce/centos/
- **Ubuntu**: https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/

Un cop instal.lat docker i amb el server corrent, executem:

```
docker run -d -e CADDYHOST=exemple.cat -v pwd/data:/data -p 80:80 -p 443:443 —name ipfs-gateway cbluth/ipfs-gateway:latest
```

substituint **'exemple.cat'** pel domini que apunta al nostre servidor.
En uns minuts hauria de estar disponible el gateway; ho podem provar accedint en el nostre navegador a:

https://exemple.cat/ipns/QmZxWEBJBVkGDGaKdYPQUXX4KC5TCWbvuR4iYZrTML8XCR


## [Español] Cómo montar un gateway IPFS

Necesitamos:

    - Un servidor, con mínimo **512mb** de **RAM** y **5 gigabytes de disco**.
    - Un dominio que apunte a la IP de nuestro servidor
    - Una distribución Linux reciente: **Debian**, **CentOS 7**, **Ubuntu**, etc.
    - El puerto **HTTPS (443)** accesible des de **Internet**

El primer paso es instal.lar Docker, lo cual se hace en pocs pasos seguiendo aquesta guía:

- **Debian**: https://docs.docker.com/engine/installation/linux/docker-ce/debian/
- **Centos**: https://docs.docker.com/engine/installation/linux/docker-ce/centos/
- **Ubuntu**: https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/

Una vez instalado docker y con el servirdor corriendo, ejecutamos:

```
docker run -d -e CADDYHOST=exemple.cat -v pwd/data:/data -p 80:80 -p 443:443 —name ipfs-gateway cbluth/ipfs-gateway:latest
```

sustuyendo '**exemple.cat**' por el dominio que apunta a nuestro servidor.
En unos minutos tendría que estar disponible el gateway; lo podemos probar accediendo en nuestro navegador a:

https://exemple.cat/ipns/QmZxWEBJBVkGDGaKdYPQUXX4KC5TCWbvuR4iYZrTML8XCR


## [English] How to set up an IPFS gateway

We need:

    - A server, with a minimum amount of **512mb RAM** and **5 gigabytes** of free disk space.
    - A domain pointing to our server's IP
    - A recent Linux distribution: **Debian**, **CentOS 7**, **Ubuntu**, etc.
    - The **HTTPS (443)** port must be accessible from **Internet**

The first step is to install Docker, which is done following howto:

- **Debian**: https://docs.docker.com/engine/installation/linux/docker-ce/debian/
- **Centos**: https://docs.docker.com/engine/installation/linux/docker-ce/centos/
- **Ubuntu**: https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/

Once Docer is installed and the server working, we execute the following command line:

```
docker run -d -e CADDYHOST=exemple.cat -v pwd/data:/data -p 80:80 -p 443:443 —name ipfs-gateway cbluth/ipfs-gateway:latest
```

'**exemple.cat**' must be replaced by the domain pointing to our server.
In few minutes the gateway should be ready. We can test it typing in our browser the following link:

https://exemple.cat/ipns/QmZxWEBJBVkGDGaKdYPQUXX4KC5TCWbvuR4iYZrTML8XCR
