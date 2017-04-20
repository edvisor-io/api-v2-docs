## Offering Course Category

Attribute | Description
--- | ---
offeringCourseCategoryId | 
left | 
right | 
depth | 
codeName | 

### Queries

```shell
#example of using offeringCourseCategories

curl https://api.edvisor.io/graphql \
  -X POST \
  -H "Authorization: Bearer MY_API_KEY" \
  -H 'content-type: application/json' \
  -d '{"query":"query {offeringCourseCategories {offeringCourseCategoryId, codeName}}"}'
```

Query | Return object
--- | ---
offeringCourseCategories | Array&lt;[OfferingCourseCategory](#offering-course-category)&gt;