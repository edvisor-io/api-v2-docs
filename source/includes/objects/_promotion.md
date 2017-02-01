## Promotion

Attribute | Description
--- | ---
promotionId | 
schoolId | The campus that the promotion belongs to
name | 
descriptions[] | Array of descriptions in different languages
descriptions[].languageId | 
descriptions[].description | 
beginBookingExpiry | 
endBookingExpiry | 
beginStartDateExpiry | 
endStartDateExpiry | 
minAge | 
maxAge | 
isEligibleAllStudentNationalities | 
isEligibleAllAgencies | 
isEligibleByAgencyLocation | 
promotionApplicableTypeId | ie. Total after tax, Tuition only
eligibleAgencies[] | Array of agencies that the promotion is eligible for
eligibleAgencies[].agencyId | 
eligibleCountries[] | Array of countries that the promotion is eligible for
eligibleCountries[].countryId | 
eligibleOfferings[] | Array of courses/accommodation/addons  that the promotion is eligible for
eligibleOfferings[].offeringId | 
eligibleNationalities[] | Array of student nationalities that the promotion is eligible for
eligibleNationalities[].countryId | 
promotionTypes[] | Array of promotion types that define how this promotion will be applied
promotionTypes[].promotionTypeId | ie. Amount off, percentage off, discount fee, duration extension, etc..
promotionTypes[].promotionSecondaryTypeId | ie. Bonus amount, bonus percentage, etc..
promotionTypes[].amount_is_per_duration | 
promotion_types[].offerings_discounted[] | Array other course/accommodations/add-ons to discount 
promotionTypes[].offerings_discounted[].offering_id | 
promotionTypes[].details[] | Array of details describing the rules for the specific promotion type
promotionTypes[].details[].amount | 
promotionTypes[].details[].minDuration | 
promotionTypes[].details[].durationTypeId | 
promotionTypes[].details[].description | 
promotionTypes[].details[].fees[] | Array of fees that can potentially be discounted
promotionTypes[].details[].fees[].feeId | 


### Queries

* `promotion(id: <id>)`
* `promotions(ids: [<ids>])`

### Mutations

* `createPromotion(input: <body>)`
* `updatePromotion(id: <id>, input: <body>)`
* `deletePromotion(id: <id>)`
