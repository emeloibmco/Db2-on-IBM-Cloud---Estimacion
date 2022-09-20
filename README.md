# Db2-on-IBM-Cloud-:cloud:-Estimación

En el presente repositorio se encuentra un modelo de excel para estimación de DB2 on IBM Cloud. 

Se deben considerar las siguientes premisas:

1. El servicio DB2 se puede estimar como Standard o Enterprise, así:
- **Standard**: Almacenamiento de hasta 4000GB y hasta 16 vCPU (inclusive)
- **Enterprise**: Almacenamiento de hasta 4000GB y hasta 56 vCPU
2. La memoria RAM tendrá una relación 4:1 con las vCPU. (16 vCPU equivalen a 64GB RAM)
3. Se considera la inclusión de Private Endpoint (CSE) en el servicio.
4. En caso de incluir alta disponibilidad (HA), se incluyen dos nodos adicionales para un total de 3.
5. En caso de incluir disaster recovery (DR), se incluye un nodo adicional para un total de 2.
6. En caso de incluir HA y DR, se incluyen tres nodos adicionales para un total de 4.
7. Recuerde que sólo es posible estimar almacenamiento por múltiplos de 20 (20GB, 40GB, 60GB ... )
8. Los recursos de cómputo sólo se pueden asignar en los siguientes tamaños: 2 vCPUs, 4 vCPUs, 8 vCPUs, 16 vCPUs, 32 vCPUs, 56 vCPUs.

## Referencias :mag:

- [DB2 Size & Price](https://db2-pricing.mybluemix.net/)
- [High Availability](https://cloud.ibm.com/docs/Db2onCloud?topic=Db2onCloud-ha)

## Autores :black_nib:
Equipo IBM Cloud Tech Sales Colombia.