## Duration Type

Attribute | Description
--- | ---
durationTypeId | 
codeName | 

### Queries

```shell
#example of using durationTypes

curl https://api.edvisor.io/graphql \
  -X POST \
  -H "Authorization: Bearer MY_API_KEY" \
  -H 'content-type: application/json' \
  -d '{"query":"query {durationTypes {durationTypeId, codeName}}"}'
```

Query | Return object
--- | ---
durationTypes | Array&lt;[DurationType](#duration-type)&gt;