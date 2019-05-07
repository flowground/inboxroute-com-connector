# ![LOGO](logo.png) Mailsquad **flow**ground Connector

## Description

A generated **flow**ground connector for the Mailsquad API (version 0.9).

Generated from: https://api.apis.guru/v2/specs/inboxroute.com/0.9/swagger.json<br/>
Generated at: 2019-05-07T17:42:26+03:00

## API Description

MailSquad offers an affordable and super easy way to create, send and track delightful emails.

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Get a paged result of contacts from a list

*Tags:* `contacts`

#### Input Parameters
* `listid` - _optional_ - Unique 16 characters ID of the contact list to get contacts of
* `offset` - _optional_ - Skip that many records
* `limit` - _optional_ - Maximum number of items in page
* `sort` - _optional_ - Property to sort by. Append '-' for descending order.

### Get a paged result of contact lists.

*Tags:* `lists`

#### Input Parameters
* `offset` - _optional_ - Skip that many records
* `limit` - _optional_ - Maximum number of items in page
* `sort` - _optional_ - Property to sort by. Append '-' for descending order.

### Add a new contact list

*Tags:* `lists`

### Delete an existing contact list

*Tags:* `lists`

#### Input Parameters
* `listid` - _required_ - Unique 16 characters ID of the contact list

### Update an existing contact list

*Tags:* `lists`

#### Input Parameters
* `listid` - _required_ - Unique 16 characters ID of the contact list

### Delete an existing contact

*Tags:* `contacts`

#### Input Parameters
* `contactid` - _required_ - Unique 16 characters ID of the contact

### Update an existing contact

*Tags:* `contacts`

#### Input Parameters
* `contactid` - _required_ - Unique 16 characters ID of the contact

### Subscribe an email address to a list. This api call has the same behavior as<br/>
> a regular subscribe form. However, single opt-in is allowed for system integration<br/>
> purposes.<br/>
> <br/>
> - If email address does not exist, a new contact will be added to the list.<br/>
> - If email address exists custom fields will be updated and status will be put<br/>
>   to unconfirmed or active depending of singleoptin value.<br/>
> - If current status if Active, this operation will only update the custom fields.<br/>
> - If singleoptin is true, no email confirmation will be sent. In that case,<br/>
>   you must provide the subscribe's origin ip and confirmation date-time.

*Tags:* `subscription`

#### Input Parameters
* `listid` - _required_ - Unique 16 characters ID of the contact list

## License

**flow**ground :- Telekom iPaaS / inboxroute-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
