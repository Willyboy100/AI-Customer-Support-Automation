# Workflow Notes

## Purpose

This project documents an existing rule-based support workflow built in Make. It connects Airtable, Gmail, a text parser, and Slack to support record handling and notifications.

## Modules

| Module | Function |
|---|---|
| Airtable — Watch Records | Watches Airtable records |
| Router | Splits the workflow into two routes |
| Gmail — Send an email | Sends an email on the first route |
| Airtable — Update a Record | Updates a record after the email step |
| Text Parser — Match pattern | Matches text against a configured pattern on the second route |
| Slack — Send a Message | Sends a Slack message on the second route |

## Example Input

See `examples/sample-ticket.json` for a fictional support-ticket example. It illustrates the kind of data a support process might handle; it is not a recorded execution result.

## Current Limitations

- Exact router conditions have not been documented.
- The text pattern and message templates have not been verified.
- Airtable field mappings have not been documented.
- The implementation is rule-based; AI classification is not included in the documented workflow.
- No measured business outcomes or execution logs are currently available.

## Next Validation Steps

1. Confirm the Airtable trigger settings.
2. Document the conditions for both router branches.
3. Record the text parser's matching pattern.
4. Capture example email and Slack outputs with private information removed.
5. Test the scenario and document the execution results.
