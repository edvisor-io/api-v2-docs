## School

Attribute | Description
--- | ---
schoolId | 
name | 
photoId | 
phone | 
email | 
website | 
address | 
instituteNumber | 
location | 
countryId | 
country | The Country object
currency | 
twitter | 
facebook | 
instagram | 
youtube | 
schoolBannerFileId | 
featuredVideoUrl | 
walkscore | 
mapUrl | 
courses | An array of Course objects
accommodations | An array of Accommodation objects
addons | An array of Addon objects
fees | An array of Fee objects


### Queries

* `school(id: <id>)`
* `schools(ids: [<ids>])`

### Mutations

* `createSchool(input: <body>)`
* `updateSchool(id: <id>, input: <body>)`
* `deleteSchool(id: <id>)`