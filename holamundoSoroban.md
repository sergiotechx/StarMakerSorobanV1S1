**Creación de una entidad un “alias” de una billetera:**

```plaintext
stellar keys generate --global <alias> --network testnet --fund
stellar keys address <alias>
```

**Creación del proyecto**

```plaintext
stellar contract init hello-world --name hello-world
```

**Compilación**
```plaintext
stellar contract build
```

⚠️ **Nota**

<table><tbody><tr><td><strong>Caracter</strong></td><td><strong>Sistema</strong></td><td><strong>se reemplaza por</strong></td></tr><tr><td>*</td><td>Mac y Linux<strong>&nbsp;</strong></td><td><strong>\</strong></td></tr><tr><td>*</td><td>Windows</td><td>`</td></tr><tr><td>@</td><td>Mac y Linux</td><td>/</td></tr><tr><td>@</td><td>Windows</td><td>\</td></tr></tbody></table>

**Despliegue**

```plaintext
stellar contract deploy *
 --wasm target@wasm32v1-none@release@hello_world.wasm *
  --source <entity> *
  --network testnet *
  --alias hello_world
```

**Prueba en testnet**

```plaintext
stellar contract invoke *
--id <contract_id>*
--source <entity> *
--network testnet *
-- *
hello *
--to "Stellar"
```
