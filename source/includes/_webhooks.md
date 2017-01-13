# Webhooks

## Introduction

In addition to the available GraphQL API, Edvisor.io can register webhooks so you can synchronise the data in your agency account with an external service or system. When registering a webhook, you’re able to subscribe to specific events so that you only receive the events (synchronize the data) that you want. 

For example, if you’d like keep the student information in your external CRM up-to-date with changes made to students in your Edvisor.io account, you can register a webhook that subscribes to the “student:update” event.  When a student is updated on Edvisor.io, we will then send the updated information to a pre-set URL.

Sample Webhook:

Webhook endpoint: `https://api.your-agency.com/webhook/edvisor`

Events subscribed: `student:create`, `student:update`

What happens: When a student is updated or created, we will send a `POST https://api.your-agency.com/webhook/edvisor` request with a body containing the changes that represent the event.

## Available events

### Student

* student:create
* student:update
* student:delete

### School

* school:create
* school:update
* school:delete

### Offering

* offering:create
* offering:update
* offering:delete

### Quote

* quote:create
* quote:update
* quote:delete

### Promotion

* promotion:create
* promotion:update
* promotion:delete

### Student enrollment

* studentEnrollment:create
* studentEnrollment:update
* studentEnrollment:delete

## Event Object

The event object that is sent along with the webhook request will be structured like the following:

Attribute | Description
--- | ---
object | String value `event`
type | Event name (ie. `student:create`)
created |
data | 
data.object | The object affected AFTER the event has taken place
data.previousObject | the object BEFORE the event took place
