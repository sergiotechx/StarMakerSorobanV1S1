**⚠️ Nota si se usa un buntu 24.XXX ejecutar las siguientes instrucciones**

Copy

```plaintext
sudo nano /etc/apt/sources.list.d/jammy.list
```

dentro del editor de texto agegar la siguiente linea de código

Copy

```plaintext
deb [arch=amd64] http://archive.ubuntu.com/ubuntu jammy main
```

Se guarda los cambios (Ctrl+O) y cierra (Ctrl+X)

Ejecuta:

Copy

```plaintext
sudo add-apt-repository ppa:ubuntu-toolchain-r/test
sudo apt-get update
sudo apt-get install build-essential libssl3 libstdc++6
```
