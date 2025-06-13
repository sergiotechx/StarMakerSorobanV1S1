## **☄️Cliente Stellar**

El cliente de Stellar es super importante en la escritura de contratos en Stellar, ya que se encarga de la creación de la estructura básica y archivos, su compilación, despliegue y pruebas respectivas.

**Intalación:**

**MAC** 

Se ejecuta el siguiente comando en la terminal

```plaintext
brew install stellar-cli
```

**Linux**

Vamos a la pagina de releases [https://github.com/stellar/stellar-cli/releases/](https://github.com/stellar/stellar-cli/releases/)

**busca el binario corresponidente a la  arquitectura de tu ordenador \[arch64 o x86\_64\]**

```plaintext
# Caso de x86_64
wget https://github.com/stellar/stellar-cli/releases/download/v22.6.0/stellar-cli-22.6.0-x86_64-unknown-linux-gnu.tar.gz

# Caso de arch64

wget https://github.com/stellar/stellar-cli/releases/download/v22.6.0/stellar-cli-22.6.0-aarch64-unknown-linux-gnu.tar.gz 
```

Descomprime el archivo 

```plaintext
#caso x86_64
tar -xvf stellar-cli-22.6.0-x86_64-unknown-linux-gnu.tar.gz

# Caso de arch64
tar -xvf stellar-cli-22.6.0-aarch64-unknown-linux-gnu.tar.gz
```

Crea un alias con el binario para que se ejecute en terminal con el comando stellar

```plaintext
sudo mv stellar /usr/local/bin/ && sudo chmod +x /usr/local/bin/stellar
```

Comprueba que se instaló correctamente

```plaintext
stellar --version
```

---

**⚠️ Nota si se usa un buntu 24.XXX ejecutar las siguientes instrucciones**

```plaintext
sudo nano /etc/apt/sources.list.d/jammy.list
```

dentro del editor de texto agegar la siguiente linea de código

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

---

**Windows**

```plaintext
winget install --id Stellar.StellarCLI 
```

---

Para los diferentes sistemas operativos también se puede ir al repositorio de github y bajar de allí los últimos ejecutables

[https://github.com/stellar/stellar-cli/releases/](https://github.com/stellar/stellar-cli/releases/)

Una vez instalado en la terminal ejecutamos el comando stellar ( en la terminal).

```plaintext
stellar
```

![](https://docs.stellarespanol.info/~gitbook/image?url=https%3A%2F%2F4030095675-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtbyfkjBGlvJb3cEGvvm8%252Fuploads%252FPmKyXOU2utpYauP8mivD%252Fimage.png%3Falt%3Dmedia%26token%3Df6ede047-9310-48f2-befc-ae501100d425&width=768&dpr=4&quality=100&sign=6489f090&sv=2)

                                                                                                                      _Ejecución de prueba_
