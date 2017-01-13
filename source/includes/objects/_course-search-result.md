## Course Search Result

Attribute | Description
--- | ---
offeringId | 
name | 
schoolId | 
school | The School object
intensityAmount | 
intensityAmountDurationType | The Duration Type object
intensityPerDurationType | The Duration Type object
enrollmentOptions | An array of enrollment options
enrollmentOptions[].durationAmount | 
enrollmentOptions[].durationType | 
enrollmentOptions[].price | 
enrollmentOptions[].currency | 
enrollmentOptions[].promotion | The promotion object
enrollmentOptions[].promotion.name | 
enrollmentOptions[].promotion.descriptions | An array of descriptions for the promotion
enrollmentOptions[].promotion.descriptions[].language | 
enrollmentOptions[].promotion.descriptions[].description | 
enrollmentOptions[].promotion.bookFrom | 
enrollmentOptions[].promotion.bookTo | 
enrollmentOptions[].promotion.studyFrom | 
enrollmentOptions[].promotion.studyTo | 
enrollmentOptions[].promotion.eligibleNationalities | An array of nationalities eligible for this promotion
enrollmentOptions[].promotion.discounts | An array of discounts to describe the promotion
enrollmentOptions[].promotion.discounts[].label | 
enrollmentOptions[].promotion.discounts[].amount | 
enrollmentOptions[].promotion.discounts[].isPercentage | 

### Queries

* `courseSearch(filter: <body>)`