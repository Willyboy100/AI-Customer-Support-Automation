# Customer Support Workflow Automation

A rule-based customer support workflow built with Make, Airtable, Gmail, a text parser, and Slack.

## Overview

Customer support processes often involve reviewing records, notifying the right people, and keeping ticket information up to date. This project demonstrates how no-code automation connects these steps and reduces repetitive manual handling.

## Workflow Overview

![Make customer support workflow overview](docs/workflow-overview.png)

The existing scenario contains the following modules:

1. **Airtable — Watch Records:** Monitors Airtable records.
2. **Router:** Splits the workflow into two routes using configured rules.
3. **Gmail — Send an email:** Sends an email on the first route.
4. **Airtable — Update a Record:** Updates an Airtable record after the email step.
5. **Text Parser — Match pattern:** Matches text against a configured pattern on the second route.
6. **Slack — Send a Message:** Sends a Slack notification on the second route.

The exact routing conditions and message contents require further verification.

## Technology Stack

* Make — Workflow automation and routing
* Airtable — Record monitoring and updates
* Gmail — Email notifications
* Text Parser — Pattern matching
* Slack — Team notifications

## Business Value

This workflow demonstrates how connected tools can reduce repetitive manual steps, send notifications through existing communication channels, and keep records updated.

Actual time savings and performance improvements have not yet been measured.

## Future Improvements

* Document and test routing conditions
* Add sample input records and expected outcomes
* Track failed runs and notification errors
* Build a dashboard for ticket volume and response times
* Explore AI-assisted ticket classification as a future enhancement

## Project Status

Existing workflow documented from the available Make scenario screenshot. Detailed configuration and end-to-end testing remain to be documented.
