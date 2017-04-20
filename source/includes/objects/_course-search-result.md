## Course Search Result

Attribute | Description
--- | ---
offeringId | 
name | 
durationAmount | 
durationTypeId | 
startDate | 
durationType | [DurationType](#duration-type)
offering | [Offering](#offering)

### Queries

```shell
#example of using coursesGetList

curl https://api.edvisor.io/graphql \
  -X POST \
  -H "Authorization: Bearer MY_API_KEY" \
  -H 'content-type: application/json' \
  -d '{"query":"query CustomQueryName($pagination: PaginationInput, $filter: CourseSearchFilter) {coursesGetList(pagination: $pagination, filter: $filter) {count, data {offeringId}}}","variables":{"pagination":{"limit":10,"offset":0},"filter":{"age":{"eq":18}}}}'
```

Query | Return object
--- | ---
coursesGetList(pagination: &lt;PaginationInput&gt;, filter: [&lt;CourseSearchFilter&gt;](#course-search-filter)) | [ListResult](#list-result)