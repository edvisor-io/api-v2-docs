# Integrations

An Edvisor Agency account manages information about students, staff tasks and reminders, quotes, invoices, products and services (courses, accommodations, add-ons, fees) offered by “connected” schools, products and services offered by the agency, and student registrations. 

This document is provides an overview of the ways you can integrate with your edvisor agency account and the types of data you can push, pull, or synch with.  Most commonly, we see Edvisor Agency integrations with 3rd party CRMs (to make quoting and registering students more seamless), B2C Websites (to provide quoting or ecommerce functionality for students online), and accounting systems. 

There are three ways to integrate with your Edvisor account. 

## API integration

This method allows you to update data in your Edvisor account with changes in your external system by calling the Edvisor API.

<img src='/images/integration_agency_1.png'>

## Webhooks integration

This method allows you to update your external system with changes in your Edvisor account by registering a webhook and subscribing to the relevant events and implementing the necessary logic needed to handle the change event to update your existing system. 

<img src='/images/integration_agency_2.png'>

## API and Webhooks integration

This method allows 2-way synchronization between your Edvisor account and your existing back-office system by combining Method 1 and Method 2.