**⚠️ Nota si se usa un buntu 24.XXX ejecutar las siguientes instrucciones**

```bash
sudo nano /etc/apt/sources.list.d/jammy.list
```
Dentro del editor de texto agegar la siguiente linea de código

```plaintext
deb [arch=amd64] http://archive.ubuntu.com/ubuntu jammy main
```

Se guarda los cambios (Ctrl+O) y cierra (Ctrl+X)

Ejecuta:

```plaintext
sudo add-apt-repository ppa:ubuntu-toolchain-r/test
sudo apt-get update
sudo apt-get install build-essential libssl3 libstdc++6
```
