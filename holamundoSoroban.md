**Creación de una entidad un “alias” de una billetera:**

```plaintext
stellar keys generate --global <alias> --network testnet –fund
stellar keys address <alias>
```

**Creación del proyecto**

```plaintext
stellar contract init hello-world --name hello-world
```

**Compilación**

stellar contract build

⚠️ **Nota**

**\* En mac y linux se cambia por \\**

    **windows por** \`

**Despliegue**

```plaintext
stellar contract deploy *
 --wasm target\wasm32v1-none\release\hello_world.wasm *
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
hello
--to "Stellar"
```
