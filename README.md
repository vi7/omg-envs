PlatformIO environment configs for the OpenMQTTGateway
======================================================

Usage
-----

Recommended way is to create symlinks in the OpenMQTTGateway repo dir pointing to each individual env config file located in this repo.

Optionally you can create `secret_env.ini` (ignored by the Git) taking [secret_env.ini.example](./secret_env.ini.example) as an example and populating it with relevant values. This will completely disable ESP WifiManager and configure OpenMQTTGateway using variables provided in the `secret_env.ini`

Example:
```bash
cd /path/to/the/OpenMQTTGateway
ln -sf /path/to/the/omg-envs/omg_grower_env.ini .
ln -sf /path/to/the/omg-envs/omg_d1mini_rf_env.ini .
ln -sf /path/to/the/omg-envs/secret_env.ini .
```
