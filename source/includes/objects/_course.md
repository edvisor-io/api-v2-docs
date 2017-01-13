## Course

Attribute | Description
--- | ---
offeringId | 
schoolId | The campus the course belongs to
reqMinDurationAmount | 
reqMinDurationTypeId | 
reqMaxDurationAmount | 
reqMaxDurationTypeId | 
reqMinAge | 
reqMaxAge | 
availabilityStart | 
availabilityEnd | 
name | 
offeringCourseCategoryId | 
reqEnglishLevelId | 
descriptions[] | Array of descriptions in different languages
descriptions[].languageId | 
descriptions[].description | 
prices[] | Array of pricing rules associated with the course
prices[].startDate | 
prices[].endDate | 
prices[].minDuration | 
prices[].maxDuration | 
prices[].durationTypeId | 
prices[].amount | 
prices[].isAmountPerDuration | 
pricingIsTiered | Whether to use tiered pricing with the price rules
fees[] | Array of fees associated with the course
fees[].name | 
fees[].prices[] | Array of pricing rules for the fees
fees[].prices[].amount | 
fees[].prices[].isRepeating | Allows the fees to repeat
fees[].prices[].repeatDurationAmount | 
fees[].prices[].repeatDurationTypeId | 
fees[].prices[].rules[] | Rules that configure how the pricing should be applied
fees[].prices[].rules[].priceRuleTypeId | ie. Study duration, Valid time period, Student Age, or Booking date
fees[].prices[].rules[].comparisonTypeId | ie. Equal, Not equal, Greater than, Less than, etc..
fees[].prices[].rules[].value | 
fees[].prices[].rules[].durationTypeId | 
fees[].prices[].rules[].startDate | 
fees[].prices[].rules[].endDate | 
fees[].prices[].rules[].logicalOperatorId | ie. AND / OR
timetables[] | Array of timetables for the course
timetable | Timetable object 
timetable.timetableTypeId | ie. Full time / Part time / Other
timetable.durationAmount | Used to define an intensity, ie. 20 hrs/week
timetable.durationTypeId | Used to define an intensity, ie. 20 hrs/week
timetable.perDurationTypeId | Used to define an intensity, ie. 20 hrs/week
timetable.items[] | Array of items defining the timetable
timetable.items[].day | 
timetable.items[].start | Start time
timetable.items[].end | End time
timetable.items[].description | 
startDates[] | Array of start dates for the course
startDates[].startDate | 

### Queries

* `course(id: <id>)`
* `courses(ids: [<ids>])`

### Mutations

* `createCourse(input: <body>)`
* `updateCourse(id: <id>, input: <body>)`
* `upsertCourse(input: <body>)`
* `deleteCourse(id: <id>)`
