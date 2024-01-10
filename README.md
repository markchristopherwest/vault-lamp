# Vault LAMP

This repo will spin up a HashiCorp Vault instance using docker compose.  Using init containers, setup Vault then LAMP including Transit via TF.  

## Create Vault & LAMP via Docker Compose

```bash

./run all
./run cleanup

```

## Create Vault with LAMP where Vault provides a transit key to a volume mounted to LAMP named /sensitive

```bash

# To verify your vault init container logs:

docker logs compose-vaultsetup-1

# To verify your vault service container logs:

docker logs compose-vault-1

# To verify your vault init container logs:

docker logs compose-lamp-1


# Check the json file in the sensitive folder for your 

```


