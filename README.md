# twilio-sdk

Developer-friendly & type-safe Typescript SDK specifically catered to leverage *twilio-sdk* API.

<div align="left">
    <a href="https://www.speakeasy.com/?utm_source=twilio-sdk&utm_campaign=typescript"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
    <a href="https://opensource.org/licenses/MIT">
        <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
    </a>
</div>


<br /><br />
> [!IMPORTANT]
> This SDK is not yet ready for production use. To complete setup please follow the steps outlined in your [workspace](https://app.speakeasy.com/org/ritza-rzx/ritza). Delete this section before > publishing to a package manager.

<!-- Start Summary [summary] -->
## Summary

Twilio - Api: This is the public Twilio REST API.
<!-- End Summary [summary] -->

<!-- Start Table of Contents [toc] -->
## Table of Contents
<!-- $toc-max-depth=2 -->
* [twilio-sdk](#twilio-sdk)
  * [SDK Installation](#sdk-installation)
  * [Requirements](#requirements)
  * [SDK Example Usage](#sdk-example-usage)
  * [Authentication](#authentication)
  * [Available Resources and Operations](#available-resources-and-operations)
  * [Standalone functions](#standalone-functions)
  * [Retries](#retries)
  * [Error Handling](#error-handling)
  * [Server Selection](#server-selection)
  * [Custom HTTP Client](#custom-http-client)
  * [Debugging](#debugging)
* [Development](#development)
  * [Maturity](#maturity)
  * [Contributions](#contributions)

<!-- End Table of Contents [toc] -->

<!-- Start SDK Installation [installation] -->
## SDK Installation

> [!TIP]
> To finish publishing your SDK to npm and others you must [run your first generation action](https://www.speakeasy.com/docs/github-setup#step-by-step-guide).


The SDK can be installed with either [npm](https://www.npmjs.com/), [pnpm](https://pnpm.io/), [bun](https://bun.sh/) or [yarn](https://classic.yarnpkg.com/en/) package managers.

### NPM

```bash
npm add <UNSET>
```

### PNPM

```bash
pnpm add <UNSET>
```

### Bun

```bash
bun add <UNSET>
```

### Yarn

```bash
yarn add <UNSET> zod

# Note that Yarn does not install peer dependencies automatically. You will need
# to install zod as shown above.
```
<!-- End SDK Installation [installation] -->

<!-- Start Requirements [requirements] -->
## Requirements

For supported JavaScript runtimes, please consult [RUNTIMES.md](RUNTIMES.md).
<!-- End Requirements [requirements] -->

<!-- Start SDK Example Usage [usage] -->
## SDK Example Usage

### Example

```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->

<!-- Start Authentication [security] -->
## Authentication

### Per-Client Security Schemes

This SDK supports the following security scheme globally:

| Name                      | Type | Scheme     | Environment Variable                          |
| ------------------------- | ---- | ---------- | --------------------------------------------- |
| `username`<br/>`password` | http | HTTP Basic | `TWILIOSDK_USERNAME`<br/>`TWILIOSDK_PASSWORD` |

You can set the security parameters through the `security` optional parameter when initializing the SDK client instance. For example:
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End Authentication [security] -->

<!-- Start Available Resources and Operations [operations] -->
## Available Resources and Operations

<details open>
<summary>Available methods</summary>

### [api20100401Account](docs/sdks/api20100401account/README.md)

* [createAccount](docs/sdks/api20100401account/README.md#createaccount) - Create a new Twilio Subaccount from the account making the request
* [listAccount](docs/sdks/api20100401account/README.md#listaccount) - Retrieves a collection of Accounts belonging to the account used to make the request
* [fetchAccount](docs/sdks/api20100401account/README.md#fetchaccount) - Fetch the account specified by the provided Account Sid
* [updateAccount](docs/sdks/api20100401account/README.md#updateaccount) - Modify the properties of a given Account

### [api20100401AddOnResult](docs/sdks/api20100401addonresult/README.md)

* [fetchRecordingAddOnResult](docs/sdks/api20100401addonresult/README.md#fetchrecordingaddonresult) - Fetch an instance of an AddOnResult
* [deleteRecordingAddOnResult](docs/sdks/api20100401addonresult/README.md#deleterecordingaddonresult) - Delete a result and purge all associated Payloads
* [listRecordingAddOnResult](docs/sdks/api20100401addonresult/README.md#listrecordingaddonresult) - Retrieve a list of results belonging to the recording

### [api20100401Address](docs/sdks/api20100401address/README.md)

* [createAddress](docs/sdks/api20100401address/README.md#createaddress)
* [listAddress](docs/sdks/api20100401address/README.md#listaddress)
* [deleteAddress](docs/sdks/api20100401address/README.md#deleteaddress)
* [fetchAddress](docs/sdks/api20100401address/README.md#fetchaddress)
* [updateAddress](docs/sdks/api20100401address/README.md#updateaddress)

### [api20100401AllTime](docs/sdks/api20100401alltime/README.md)

* [listUsageRecordAllTime](docs/sdks/api20100401alltime/README.md#listusagerecordalltime)

### [api20100401Application](docs/sdks/api20100401application/README.md)

* [createApplication](docs/sdks/api20100401application/README.md#createapplication) - Create a new application within your account
* [listApplication](docs/sdks/api20100401application/README.md#listapplication) - Retrieve a list of applications representing an application within the requesting account
* [deleteApplication](docs/sdks/api20100401application/README.md#deleteapplication) - Delete the application by the specified application sid
* [fetchApplication](docs/sdks/api20100401application/README.md#fetchapplication) - Fetch the application specified by the provided sid
* [updateApplication](docs/sdks/api20100401application/README.md#updateapplication) - Updates the application's properties

### [api20100401AssignedAddOn](docs/sdks/api20100401assignedaddon/README.md)

* [fetchIncomingPhoneNumberAssignedAddOn](docs/sdks/api20100401assignedaddon/README.md#fetchincomingphonenumberassignedaddon) - Fetch an instance of an Add-on installation currently assigned to this Number.
* [deleteIncomingPhoneNumberAssignedAddOn](docs/sdks/api20100401assignedaddon/README.md#deleteincomingphonenumberassignedaddon) - Remove the assignment of an Add-on installation from the Number specified.
* [listIncomingPhoneNumberAssignedAddOn](docs/sdks/api20100401assignedaddon/README.md#listincomingphonenumberassignedaddon) - Retrieve a list of Add-on installations currently assigned to this Number.
* [createIncomingPhoneNumberAssignedAddOn](docs/sdks/api20100401assignedaddon/README.md#createincomingphonenumberassignedaddon) - Assign an Add-on installation to the Number specified.

### [api20100401AssignedAddOnExtension](docs/sdks/api20100401assignedaddonextension/README.md)

* [fetchIncomingPhoneNumberAssignedAddOnExtension](docs/sdks/api20100401assignedaddonextension/README.md#fetchincomingphonenumberassignedaddonextension) - Fetch an instance of an Extension for the Assigned Add-on.
* [listIncomingPhoneNumberAssignedAddOnExtension](docs/sdks/api20100401assignedaddonextension/README.md#listincomingphonenumberassignedaddonextension) - Retrieve a list of Extensions for the Assigned Add-on.

### [api20100401AuthCallsCredentialListMapping](docs/sdks/api20100401authcallscredentiallistmapping/README.md)

* [createSipAuthCallsCredentialListMapping](docs/sdks/api20100401authcallscredentiallistmapping/README.md#createsipauthcallscredentiallistmapping) - Create a new credential list mapping resource
* [listSipAuthCallsCredentialListMapping](docs/sdks/api20100401authcallscredentiallistmapping/README.md#listsipauthcallscredentiallistmapping) - Retrieve a list of credential list mappings belonging to the domain used in the request
* [fetchSipAuthCallsCredentialListMapping](docs/sdks/api20100401authcallscredentiallistmapping/README.md#fetchsipauthcallscredentiallistmapping) - Fetch a specific instance of a credential list mapping
* [deleteSipAuthCallsCredentialListMapping](docs/sdks/api20100401authcallscredentiallistmapping/README.md#deletesipauthcallscredentiallistmapping) - Delete a credential list mapping from the requested domain

### [api20100401AuthCallsIpAccessControlListMapping](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md)

* [createSipAuthCallsIpAccessControlListMapping](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#createsipauthcallsipaccesscontrollistmapping) - Create a new IP Access Control List mapping
* [listSipAuthCallsIpAccessControlListMapping](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#listsipauthcallsipaccesscontrollistmapping) - Retrieve a list of IP Access Control List mappings belonging to the domain used in the request
* [fetchSipAuthCallsIpAccessControlListMapping](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#fetchsipauthcallsipaccesscontrollistmapping) - Fetch a specific instance of an IP Access Control List mapping
* [deleteSipAuthCallsIpAccessControlListMapping](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#deletesipauthcallsipaccesscontrollistmapping) - Delete an IP Access Control List mapping from the requested domain

### [api20100401AuthorizedConnectApp](docs/sdks/api20100401authorizedconnectapp/README.md)

* [fetchAuthorizedConnectApp](docs/sdks/api20100401authorizedconnectapp/README.md#fetchauthorizedconnectapp) - Fetch an instance of an authorized-connect-app
* [listAuthorizedConnectApp](docs/sdks/api20100401authorizedconnectapp/README.md#listauthorizedconnectapp) - Retrieve a list of authorized-connect-apps belonging to the account used to make the request

### [api20100401AuthRegistrationsCredentialListMapping](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md)

* [createSipAuthRegistrationsCredentialListMapping](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#createsipauthregistrationscredentiallistmapping) - Create a new credential list mapping resource
* [listSipAuthRegistrationsCredentialListMapping](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#listsipauthregistrationscredentiallistmapping) - Retrieve a list of credential list mappings belonging to the domain used in the request
* [fetchSipAuthRegistrationsCredentialListMapping](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#fetchsipauthregistrationscredentiallistmapping) - Fetch a specific instance of a credential list mapping
* [deleteSipAuthRegistrationsCredentialListMapping](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#deletesipauthregistrationscredentiallistmapping) - Delete a credential list mapping from the requested domain

### [api20100401AvailablePhoneNumberCountry](docs/sdks/api20100401availablephonenumbercountry/README.md)

* [listAvailablePhoneNumberCountry](docs/sdks/api20100401availablephonenumbercountry/README.md#listavailablephonenumbercountry)
* [fetchAvailablePhoneNumberCountry](docs/sdks/api20100401availablephonenumbercountry/README.md#fetchavailablephonenumbercountry)

### [api20100401Balance](docs/sdks/api20100401balance/README.md)

* [fetchBalance](docs/sdks/api20100401balance/README.md#fetchbalance) - Fetch the balance for an Account based on Account Sid. Balance changes may not be reflected immediately. Child accounts do not contain balance information

### [api20100401Call](docs/sdks/api20100401call/README.md)

* [createCall](docs/sdks/api20100401call/README.md#createcall) - Create a new outgoing call to phones, SIP-enabled endpoints or Twilio Client connections
* [listCall](docs/sdks/api20100401call/README.md#listcall) - Retrieves a collection of calls made to and from your account
* [deleteCall](docs/sdks/api20100401call/README.md#deletecall) - Delete a Call record from your account. Once the record is deleted, it will no longer appear in the API and Account Portal logs.
* [fetchCall](docs/sdks/api20100401call/README.md#fetchcall) - Fetch the call specified by the provided Call SID
* [updateCall](docs/sdks/api20100401call/README.md#updatecall) - Initiates a call redirect or terminates a call

### [api20100401CallNotification](docs/sdks/api20100401callnotification/README.md)

* [fetchCallNotification](docs/sdks/api20100401callnotification/README.md#fetchcallnotification)
* [listCallNotification](docs/sdks/api20100401callnotification/README.md#listcallnotification)

### [api20100401CallTranscription](docs/sdks/api20100401calltranscription/README.md)

* [createRealtimeTranscription](docs/sdks/api20100401calltranscription/README.md#createrealtimetranscription) - Create a Transcription
* [updateRealtimeTranscription](docs/sdks/api20100401calltranscription/README.md#updaterealtimetranscription) - Stop a Transcription using either the SID of the Transcription resource or the `name` used when creating the resource

### [api20100401Conference](docs/sdks/api20100401conference/README.md)

* [fetchConference](docs/sdks/api20100401conference/README.md#fetchconference) - Fetch an instance of a conference
* [updateConference](docs/sdks/api20100401conference/README.md#updateconference)
* [listConference](docs/sdks/api20100401conference/README.md#listconference) - Retrieve a list of conferences belonging to the account used to make the request

### [api20100401ConnectApp](docs/sdks/api20100401connectapp/README.md)

* [fetchConnectApp](docs/sdks/api20100401connectapp/README.md#fetchconnectapp) - Fetch an instance of a connect-app
* [updateConnectApp](docs/sdks/api20100401connectapp/README.md#updateconnectapp) - Update a connect-app with the specified parameters
* [deleteConnectApp](docs/sdks/api20100401connectapp/README.md#deleteconnectapp) - Delete an instance of a connect-app
* [listConnectApp](docs/sdks/api20100401connectapp/README.md#listconnectapp) - Retrieve a list of connect-apps belonging to the account used to make the request

### [api20100401Credential](docs/sdks/api20100401credential/README.md)

* [listSipCredential](docs/sdks/api20100401credential/README.md#listsipcredential) - Retrieve a list of credentials.
* [createSipCredential](docs/sdks/api20100401credential/README.md#createsipcredential) - Create a new credential resource.
* [fetchSipCredential](docs/sdks/api20100401credential/README.md#fetchsipcredential) - Fetch a single credential.
* [updateSipCredential](docs/sdks/api20100401credential/README.md#updatesipcredential) - Update a credential resource.
* [deleteSipCredential](docs/sdks/api20100401credential/README.md#deletesipcredential) - Delete a credential resource.

### [api20100401CredentialList](docs/sdks/api20100401credentiallist/README.md)

* [listSipCredentialList](docs/sdks/api20100401credentiallist/README.md#listsipcredentiallist) - Get All Credential Lists
* [createSipCredentialList](docs/sdks/api20100401credentiallist/README.md#createsipcredentiallist) - Create a Credential List
* [fetchSipCredentialList](docs/sdks/api20100401credentiallist/README.md#fetchsipcredentiallist) - Get a Credential List
* [updateSipCredentialList](docs/sdks/api20100401credentiallist/README.md#updatesipcredentiallist) - Update a Credential List
* [deleteSipCredentialList](docs/sdks/api20100401credentiallist/README.md#deletesipcredentiallist) - Delete a Credential List

### [api20100401CredentialListMapping](docs/sdks/api20100401credentiallistmapping/README.md)

* [createSipCredentialListMapping](docs/sdks/api20100401credentiallistmapping/README.md#createsipcredentiallistmapping) - Create a CredentialListMapping resource for an account.
* [listSipCredentialListMapping](docs/sdks/api20100401credentiallistmapping/README.md#listsipcredentiallistmapping) - Read multiple CredentialListMapping resources from an account.
* [fetchSipCredentialListMapping](docs/sdks/api20100401credentiallistmapping/README.md#fetchsipcredentiallistmapping) - Fetch a single CredentialListMapping resource from an account.
* [deleteSipCredentialListMapping](docs/sdks/api20100401credentiallistmapping/README.md#deletesipcredentiallistmapping) - Delete a CredentialListMapping resource from an account.

### [api20100401Daily](docs/sdks/api20100401daily/README.md)

* [listUsageRecordDaily](docs/sdks/api20100401daily/README.md#listusagerecorddaily)

### [api20100401Data](docs/sdks/api20100401data/README.md)

* [fetchRecordingAddOnResultPayloadData](docs/sdks/api20100401data/README.md#fetchrecordingaddonresultpayloaddata) - Fetch an instance of a result payload

### [api20100401DependentPhoneNumber](docs/sdks/api20100401dependentphonenumber/README.md)

* [listDependentPhoneNumber](docs/sdks/api20100401dependentphonenumber/README.md#listdependentphonenumber)

### [api20100401Domain](docs/sdks/api20100401domain/README.md)

* [listSipDomain](docs/sdks/api20100401domain/README.md#listsipdomain) - Retrieve a list of domains belonging to the account used to make the request
* [createSipDomain](docs/sdks/api20100401domain/README.md#createsipdomain) - Create a new Domain
* [fetchSipDomain](docs/sdks/api20100401domain/README.md#fetchsipdomain) - Fetch an instance of a Domain
* [updateSipDomain](docs/sdks/api20100401domain/README.md#updatesipdomain) - Update the attributes of a domain
* [deleteSipDomain](docs/sdks/api20100401domain/README.md#deletesipdomain) - Delete an instance of a Domain

### [api20100401Event](docs/sdks/api20100401event/README.md)

* [listCallEvent](docs/sdks/api20100401event/README.md#listcallevent) - Retrieve a list of all events for a call.

### [api20100401Feedback](docs/sdks/api20100401feedback/README.md)

* [createMessageFeedback](docs/sdks/api20100401feedback/README.md#createmessagefeedback) - Create Message Feedback to confirm a tracked user action was performed by the recipient of the associated Message

### [api20100401IncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md)

* [updateIncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md#updateincomingphonenumber) - Update an incoming-phone-number instance.
* [fetchIncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md#fetchincomingphonenumber) - Fetch an incoming-phone-number belonging to the account used to make the request.
* [deleteIncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md#deleteincomingphonenumber) - Delete a phone-numbers belonging to the account used to make the request.
* [listIncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md#listincomingphonenumber) - Retrieve a list of incoming-phone-numbers belonging to the account used to make the request.
* [createIncomingPhoneNumber](docs/sdks/api20100401incomingphonenumber/README.md#createincomingphonenumber) - Purchase a phone-number for the account.

### [api20100401IncomingPhoneNumberLocal](docs/sdks/api20100401incomingphonenumberlocal/README.md)

* [listIncomingPhoneNumberLocal](docs/sdks/api20100401incomingphonenumberlocal/README.md#listincomingphonenumberlocal)
* [createIncomingPhoneNumberLocal](docs/sdks/api20100401incomingphonenumberlocal/README.md#createincomingphonenumberlocal)

### [api20100401IncomingPhoneNumberMobile](docs/sdks/api20100401incomingphonenumbermobile/README.md)

* [listIncomingPhoneNumberMobile](docs/sdks/api20100401incomingphonenumbermobile/README.md#listincomingphonenumbermobile)
* [createIncomingPhoneNumberMobile](docs/sdks/api20100401incomingphonenumbermobile/README.md#createincomingphonenumbermobile)

### [api20100401IncomingPhoneNumberTollFree](docs/sdks/api20100401incomingphonenumbertollfree/README.md)

* [listIncomingPhoneNumberTollFree](docs/sdks/api20100401incomingphonenumbertollfree/README.md#listincomingphonenumbertollfree)
* [createIncomingPhoneNumberTollFree](docs/sdks/api20100401incomingphonenumbertollfree/README.md#createincomingphonenumbertollfree)

### [api20100401IpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md)

* [listSipIpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md#listsipipaccesscontrollist) - Retrieve a list of IpAccessControlLists that belong to the account used to make the request
* [createSipIpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md#createsipipaccesscontrollist) - Create a new IpAccessControlList resource
* [fetchSipIpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md#fetchsipipaccesscontrollist) - Fetch a specific instance of an IpAccessControlList
* [updateSipIpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md#updatesipipaccesscontrollist) - Rename an IpAccessControlList
* [deleteSipIpAccessControlList](docs/sdks/api20100401ipaccesscontrollist/README.md#deletesipipaccesscontrollist) - Delete an IpAccessControlList from the requested account

### [api20100401IpAccessControlListMapping](docs/sdks/api20100401ipaccesscontrollistmapping/README.md)

* [fetchSipIpAccessControlListMapping](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#fetchsipipaccesscontrollistmapping) - Fetch an IpAccessControlListMapping resource.
* [deleteSipIpAccessControlListMapping](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#deletesipipaccesscontrollistmapping) - Delete an IpAccessControlListMapping resource.
* [createSipIpAccessControlListMapping](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#createsipipaccesscontrollistmapping) - Create a new IpAccessControlListMapping resource.
* [listSipIpAccessControlListMapping](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#listsipipaccesscontrollistmapping) - Retrieve a list of IpAccessControlListMapping resources.

### [api20100401Key](docs/sdks/api20100401key/README.md)

* [fetchKey](docs/sdks/api20100401key/README.md#fetchkey)
* [updateKey](docs/sdks/api20100401key/README.md#updatekey)
* [deleteKey](docs/sdks/api20100401key/README.md#deletekey)
* [listKey](docs/sdks/api20100401key/README.md#listkey)

### [api20100401LastMonth](docs/sdks/api20100401lastmonth/README.md)

* [listUsageRecordLastMonth](docs/sdks/api20100401lastmonth/README.md#listusagerecordlastmonth)

### [api20100401Local](docs/sdks/api20100401local/README.md)

* [listAvailablePhoneNumberLocal](docs/sdks/api20100401local/README.md#listavailablephonenumberlocal)

### [api20100401MachineToMachine](docs/sdks/api20100401machinetomachine/README.md)

* [listAvailablePhoneNumberMachineToMachine](docs/sdks/api20100401machinetomachine/README.md#listavailablephonenumbermachinetomachine)

### [api20100401Media](docs/sdks/api20100401media/README.md)

* [deleteMedia](docs/sdks/api20100401media/README.md#deletemedia) - Delete the Media resource.
* [fetchMedia](docs/sdks/api20100401media/README.md#fetchmedia) - Fetch a single Media resource associated with a specific Message resource
* [listMedia](docs/sdks/api20100401media/README.md#listmedia) - Read a list of Media resources associated with a specific Message resource

### [api20100401Member](docs/sdks/api20100401member/README.md)

* [fetchMember](docs/sdks/api20100401member/README.md#fetchmember) - Fetch a specific member from the queue
* [updateMember](docs/sdks/api20100401member/README.md#updatemember) - Dequeue a member from a queue and have the member's call begin executing the TwiML document at that URL
* [listMember](docs/sdks/api20100401member/README.md#listmember) - Retrieve the members of the queue

### [api20100401Message](docs/sdks/api20100401message/README.md)

* [createMessage](docs/sdks/api20100401message/README.md#createmessage) - Send a message
* [listMessage](docs/sdks/api20100401message/README.md#listmessage) - Retrieve a list of Message resources associated with a Twilio Account
* [deleteMessage](docs/sdks/api20100401message/README.md#deletemessage) - Deletes a Message resource from your account
* [fetchMessage](docs/sdks/api20100401message/README.md#fetchmessage) - Fetch a specific Message
* [updateMessage](docs/sdks/api20100401message/README.md#updatemessage) - Update a Message resource (used to redact Message `body` text and to cancel not-yet-sent messages)

### [api20100401Mobile](docs/sdks/api20100401mobile/README.md)

* [listAvailablePhoneNumberMobile](docs/sdks/api20100401mobile/README.md#listavailablephonenumbermobile)

### [api20100401Monthly](docs/sdks/api20100401monthly/README.md)

* [listUsageRecordMonthly](docs/sdks/api20100401monthly/README.md#listusagerecordmonthly)

### [api20100401National](docs/sdks/api20100401national/README.md)

* [listAvailablePhoneNumberNational](docs/sdks/api20100401national/README.md#listavailablephonenumbernational)

### [api20100401NewKey](docs/sdks/api20100401newkey/README.md)

* [createNewKey](docs/sdks/api20100401newkey/README.md#createnewkey)

### [api20100401NewSigningKey](docs/sdks/api20100401newsigningkey/README.md)

* [createNewSigningKey](docs/sdks/api20100401newsigningkey/README.md#createnewsigningkey) - Create a new Signing Key for the account making the request.

### [api20100401Notification](docs/sdks/api20100401notification/README.md)

* [fetchNotification](docs/sdks/api20100401notification/README.md#fetchnotification) - Fetch a notification belonging to the account used to make the request
* [listNotification](docs/sdks/api20100401notification/README.md#listnotification) - Retrieve a list of notifications belonging to the account used to make the request

### [api20100401OutgoingCallerId](docs/sdks/api20100401outgoingcallerid/README.md)

* [fetchOutgoingCallerId](docs/sdks/api20100401outgoingcallerid/README.md#fetchoutgoingcallerid) - Fetch an outgoing-caller-id belonging to the account used to make the request
* [updateOutgoingCallerId](docs/sdks/api20100401outgoingcallerid/README.md#updateoutgoingcallerid) - Updates the caller-id
* [deleteOutgoingCallerId](docs/sdks/api20100401outgoingcallerid/README.md#deleteoutgoingcallerid) - Delete the caller-id specified from the account
* [listOutgoingCallerId](docs/sdks/api20100401outgoingcallerid/README.md#listoutgoingcallerid) - Retrieve a list of outgoing-caller-ids belonging to the account used to make the request

### [api20100401Participant](docs/sdks/api20100401participant/README.md)

* [fetchParticipant](docs/sdks/api20100401participant/README.md#fetchparticipant) - Fetch an instance of a participant
* [updateParticipant](docs/sdks/api20100401participant/README.md#updateparticipant) - Update the properties of the participant
* [deleteParticipant](docs/sdks/api20100401participant/README.md#deleteparticipant) - Kick a participant from a given conference
* [createParticipant](docs/sdks/api20100401participant/README.md#createparticipant)
* [listParticipant](docs/sdks/api20100401participant/README.md#listparticipant) - Retrieve a list of participants belonging to the account used to make the request

### [api20100401Payload](docs/sdks/api20100401payload/README.md)

* [fetchRecordingAddOnResultPayload](docs/sdks/api20100401payload/README.md#fetchrecordingaddonresultpayload) - Fetch an instance of a result payload
* [deleteRecordingAddOnResultPayload](docs/sdks/api20100401payload/README.md#deleterecordingaddonresultpayload) - Delete a payload from the result along with all associated Data
* [listRecordingAddOnResultPayload](docs/sdks/api20100401payload/README.md#listrecordingaddonresultpayload) - Retrieve a list of payloads belonging to the AddOnResult

### [api20100401Payment](docs/sdks/api20100401payment/README.md)

* [createPayments](docs/sdks/api20100401payment/README.md#createpayments) - create an instance of payments. This will start a new payments session
* [updatePayments](docs/sdks/api20100401payment/README.md#updatepayments) - update an instance of payments with different phases of payment flows.

### [api20100401Queue](docs/sdks/api20100401queue/README.md)

* [fetchQueue](docs/sdks/api20100401queue/README.md#fetchqueue) - Fetch an instance of a queue identified by the QueueSid
* [updateQueue](docs/sdks/api20100401queue/README.md#updatequeue) - Update the queue with the new parameters
* [deleteQueue](docs/sdks/api20100401queue/README.md#deletequeue) - Remove an empty queue
* [listQueue](docs/sdks/api20100401queue/README.md#listqueue) - Retrieve a list of queues belonging to the account used to make the request
* [createQueue](docs/sdks/api20100401queue/README.md#createqueue) - Create a queue

### [api20100401Record](docs/sdks/api20100401record/README.md)

* [listUsageRecord](docs/sdks/api20100401record/README.md#listusagerecord) - Retrieve a list of usage-records belonging to the account used to make the request

### [api20100401Recording](docs/sdks/api20100401recording/README.md)

* [createCallRecording](docs/sdks/api20100401recording/README.md#createcallrecording) - Create a recording for the call
* [listCallRecording](docs/sdks/api20100401recording/README.md#listcallrecording) - Retrieve a list of recordings belonging to the call used to make the request
* [updateCallRecording](docs/sdks/api20100401recording/README.md#updatecallrecording) - Changes the status of the recording to paused, stopped, or in-progress. Note: Pass `Twilio.CURRENT` instead of recording sid to reference current active recording.
* [fetchCallRecording](docs/sdks/api20100401recording/README.md#fetchcallrecording) - Fetch an instance of a recording for a call
* [deleteCallRecording](docs/sdks/api20100401recording/README.md#deletecallrecording) - Delete a recording from your account
* [listConferenceRecording](docs/sdks/api20100401recording/README.md#listconferencerecording) - Retrieve a list of recordings belonging to the call used to make the request
* [updateConferenceRecording](docs/sdks/api20100401recording/README.md#updateconferencerecording) - Changes the status of the recording to paused, stopped, or in-progress. Note: To use `Twilio.CURRENT`, pass it as recording sid.
* [fetchConferenceRecording](docs/sdks/api20100401recording/README.md#fetchconferencerecording) - Fetch an instance of a recording for a call
* [deleteConferenceRecording](docs/sdks/api20100401recording/README.md#deleteconferencerecording) - Delete a recording from your account
* [fetchRecording](docs/sdks/api20100401recording/README.md#fetchrecording) - Fetch an instance of a recording
* [deleteRecording](docs/sdks/api20100401recording/README.md#deleterecording) - Delete a recording from your account
* [listRecording](docs/sdks/api20100401recording/README.md#listrecording) - Retrieve a list of recordings belonging to the account used to make the request

### [api20100401SharedCost](docs/sdks/api20100401sharedcost/README.md)

* [listAvailablePhoneNumberSharedCost](docs/sdks/api20100401sharedcost/README.md#listavailablephonenumbersharedcost)

### [api20100401ShortCode](docs/sdks/api20100401shortcode/README.md)

* [fetchShortCode](docs/sdks/api20100401shortcode/README.md#fetchshortcode) - Fetch an instance of a short code
* [updateShortCode](docs/sdks/api20100401shortcode/README.md#updateshortcode) - Update a short code with the following parameters
* [listShortCode](docs/sdks/api20100401shortcode/README.md#listshortcode) - Retrieve a list of short-codes belonging to the account used to make the request

### [api20100401SigningKey](docs/sdks/api20100401signingkey/README.md)

* [listSigningKey](docs/sdks/api20100401signingkey/README.md#listsigningkey)
* [fetchSigningKey](docs/sdks/api20100401signingkey/README.md#fetchsigningkey)
* [updateSigningKey](docs/sdks/api20100401signingkey/README.md#updatesigningkey)
* [deleteSigningKey](docs/sdks/api20100401signingkey/README.md#deletesigningkey)

### [api20100401SipIpAddress](docs/sdks/api20100401sipipaddress/README.md)

* [listSipIpAddress](docs/sdks/api20100401sipipaddress/README.md#listsipipaddress) - Read multiple IpAddress resources.
* [createSipIpAddress](docs/sdks/api20100401sipipaddress/README.md#createsipipaddress) - Create a new IpAddress resource.
* [fetchSipIpAddress](docs/sdks/api20100401sipipaddress/README.md#fetchsipipaddress) - Read one IpAddress resource.
* [updateSipIpAddress](docs/sdks/api20100401sipipaddress/README.md#updatesipipaddress) - Update an IpAddress resource.
* [deleteSipIpAddress](docs/sdks/api20100401sipipaddress/README.md#deletesipipaddress) - Delete an IpAddress resource.

### [api20100401Siprec](docs/sdks/api20100401siprec/README.md)

* [createSiprec](docs/sdks/api20100401siprec/README.md#createsiprec) - Create a Siprec
* [updateSiprec](docs/sdks/api20100401siprec/README.md#updatesiprec) - Stop a Siprec using either the SID of the Siprec resource or the `name` used when creating the resource

### [api20100401Stream](docs/sdks/api20100401stream/README.md)

* [createStream](docs/sdks/api20100401stream/README.md#createstream) - Create a Stream
* [updateStream](docs/sdks/api20100401stream/README.md#updatestream) - Stop a Stream using either the SID of the Stream resource or the `name` used when creating the resource

### [api20100401ThisMonth](docs/sdks/api20100401thismonth/README.md)

* [listUsageRecordThisMonth](docs/sdks/api20100401thismonth/README.md#listusagerecordthismonth)

### [api20100401Today](docs/sdks/api20100401today/README.md)

* [listUsageRecordToday](docs/sdks/api20100401today/README.md#listusagerecordtoday)

### [api20100401Token](docs/sdks/api20100401token/README.md)

* [createToken](docs/sdks/api20100401token/README.md#createtoken) - Create a new token for ICE servers

### [api20100401TollFree](docs/sdks/api20100401tollfree/README.md)

* [listAvailablePhoneNumberTollFree](docs/sdks/api20100401tollfree/README.md#listavailablephonenumbertollfree)

### [api20100401Transcription](docs/sdks/api20100401transcription/README.md)

* [fetchRecordingTranscription](docs/sdks/api20100401transcription/README.md#fetchrecordingtranscription)
* [deleteRecordingTranscription](docs/sdks/api20100401transcription/README.md#deleterecordingtranscription)
* [listRecordingTranscription](docs/sdks/api20100401transcription/README.md#listrecordingtranscription)
* [fetchTranscription](docs/sdks/api20100401transcription/README.md#fetchtranscription) - Fetch an instance of a Transcription
* [deleteTranscription](docs/sdks/api20100401transcription/README.md#deletetranscription) - Delete a transcription from the account used to make the request
* [listTranscription](docs/sdks/api20100401transcription/README.md#listtranscription) - Retrieve a list of transcriptions belonging to the account used to make the request

### [api20100401Trigger](docs/sdks/api20100401trigger/README.md)

* [fetchUsageTrigger](docs/sdks/api20100401trigger/README.md#fetchusagetrigger) - Fetch and instance of a usage-trigger
* [updateUsageTrigger](docs/sdks/api20100401trigger/README.md#updateusagetrigger) - Update an instance of a usage trigger
* [deleteUsageTrigger](docs/sdks/api20100401trigger/README.md#deleteusagetrigger)
* [createUsageTrigger](docs/sdks/api20100401trigger/README.md#createusagetrigger) - Create a new UsageTrigger
* [listUsageTrigger](docs/sdks/api20100401trigger/README.md#listusagetrigger) - Retrieve a list of usage-triggers belonging to the account used to make the request

### [api20100401UserDefinedMessage](docs/sdks/api20100401userdefinedmessage/README.md)

* [createUserDefinedMessage](docs/sdks/api20100401userdefinedmessage/README.md#createuserdefinedmessage) - Create a new User Defined Message for the given Call SID.

### [api20100401UserDefinedMessageSubscription](docs/sdks/api20100401userdefinedmessagesubscription/README.md)

* [createUserDefinedMessageSubscription](docs/sdks/api20100401userdefinedmessagesubscription/README.md#createuserdefinedmessagesubscription) - Subscribe to User Defined Messages for a given Call SID.
* [deleteUserDefinedMessageSubscription](docs/sdks/api20100401userdefinedmessagesubscription/README.md#deleteuserdefinedmessagesubscription) - Delete a specific User Defined Message Subscription.

### [api20100401ValidationRequest](docs/sdks/api20100401validationrequest/README.md)

* [createValidationRequest](docs/sdks/api20100401validationrequest/README.md#createvalidationrequest)

### [api20100401Voip](docs/sdks/api20100401voip/README.md)

* [listAvailablePhoneNumberVoip](docs/sdks/api20100401voip/README.md#listavailablephonenumbervoip)

### [api20100401Yearly](docs/sdks/api20100401yearly/README.md)

* [listUsageRecordYearly](docs/sdks/api20100401yearly/README.md#listusagerecordyearly)

### [api20100401Yesterday](docs/sdks/api20100401yesterday/README.md)

* [listUsageRecordYesterday](docs/sdks/api20100401yesterday/README.md#listusagerecordyesterday)


</details>
<!-- End Available Resources and Operations [operations] -->

<!-- Start Standalone functions [standalone-funcs] -->
## Standalone functions

All the methods listed above are available as standalone functions. These
functions are ideal for use in applications running in the browser, serverless
runtimes or other environments where application bundle size is a primary
concern. When using a bundler to build your application, all unused
functionality will be either excluded from the final bundle or tree-shaken away.

To read more about standalone functions, check [FUNCTIONS.md](./FUNCTIONS.md).

<details>

<summary>Available standalone functions</summary>

- [`api20100401AccountCreateAccount`](docs/sdks/api20100401account/README.md#createaccount) - Create a new Twilio Subaccount from the account making the request
- [`api20100401AccountFetchAccount`](docs/sdks/api20100401account/README.md#fetchaccount) - Fetch the account specified by the provided Account Sid
- [`api20100401AccountListAccount`](docs/sdks/api20100401account/README.md#listaccount) - Retrieves a collection of Accounts belonging to the account used to make the request
- [`api20100401AccountUpdateAccount`](docs/sdks/api20100401account/README.md#updateaccount) - Modify the properties of a given Account
- [`api20100401AddOnResultDeleteRecordingAddOnResult`](docs/sdks/api20100401addonresult/README.md#deleterecordingaddonresult) - Delete a result and purge all associated Payloads
- [`api20100401AddOnResultFetchRecordingAddOnResult`](docs/sdks/api20100401addonresult/README.md#fetchrecordingaddonresult) - Fetch an instance of an AddOnResult
- [`api20100401AddOnResultListRecordingAddOnResult`](docs/sdks/api20100401addonresult/README.md#listrecordingaddonresult) - Retrieve a list of results belonging to the recording
- [`api20100401AddressCreateAddress`](docs/sdks/api20100401address/README.md#createaddress)
- [`api20100401AddressDeleteAddress`](docs/sdks/api20100401address/README.md#deleteaddress)
- [`api20100401AddressFetchAddress`](docs/sdks/api20100401address/README.md#fetchaddress)
- [`api20100401AddressListAddress`](docs/sdks/api20100401address/README.md#listaddress)
- [`api20100401AddressUpdateAddress`](docs/sdks/api20100401address/README.md#updateaddress)
- [`api20100401AllTimeListUsageRecordAllTime`](docs/sdks/api20100401alltime/README.md#listusagerecordalltime)
- [`api20100401ApplicationCreateApplication`](docs/sdks/api20100401application/README.md#createapplication) - Create a new application within your account
- [`api20100401ApplicationDeleteApplication`](docs/sdks/api20100401application/README.md#deleteapplication) - Delete the application by the specified application sid
- [`api20100401ApplicationFetchApplication`](docs/sdks/api20100401application/README.md#fetchapplication) - Fetch the application specified by the provided sid
- [`api20100401ApplicationListApplication`](docs/sdks/api20100401application/README.md#listapplication) - Retrieve a list of applications representing an application within the requesting account
- [`api20100401ApplicationUpdateApplication`](docs/sdks/api20100401application/README.md#updateapplication) - Updates the application's properties
- [`api20100401AssignedAddOnCreateIncomingPhoneNumberAssignedAddOn`](docs/sdks/api20100401assignedaddon/README.md#createincomingphonenumberassignedaddon) - Assign an Add-on installation to the Number specified.
- [`api20100401AssignedAddOnDeleteIncomingPhoneNumberAssignedAddOn`](docs/sdks/api20100401assignedaddon/README.md#deleteincomingphonenumberassignedaddon) - Remove the assignment of an Add-on installation from the Number specified.
- [`api20100401AssignedAddOnExtensionFetchIncomingPhoneNumberAssignedAddOnExtension`](docs/sdks/api20100401assignedaddonextension/README.md#fetchincomingphonenumberassignedaddonextension) - Fetch an instance of an Extension for the Assigned Add-on.
- [`api20100401AssignedAddOnExtensionListIncomingPhoneNumberAssignedAddOnExtension`](docs/sdks/api20100401assignedaddonextension/README.md#listincomingphonenumberassignedaddonextension) - Retrieve a list of Extensions for the Assigned Add-on.
- [`api20100401AssignedAddOnFetchIncomingPhoneNumberAssignedAddOn`](docs/sdks/api20100401assignedaddon/README.md#fetchincomingphonenumberassignedaddon) - Fetch an instance of an Add-on installation currently assigned to this Number.
- [`api20100401AssignedAddOnListIncomingPhoneNumberAssignedAddOn`](docs/sdks/api20100401assignedaddon/README.md#listincomingphonenumberassignedaddon) - Retrieve a list of Add-on installations currently assigned to this Number.
- [`api20100401AuthCallsCredentialListMappingCreateSipAuthCallsCredentialListMapping`](docs/sdks/api20100401authcallscredentiallistmapping/README.md#createsipauthcallscredentiallistmapping) - Create a new credential list mapping resource
- [`api20100401AuthCallsCredentialListMappingDeleteSipAuthCallsCredentialListMapping`](docs/sdks/api20100401authcallscredentiallistmapping/README.md#deletesipauthcallscredentiallistmapping) - Delete a credential list mapping from the requested domain
- [`api20100401AuthCallsCredentialListMappingFetchSipAuthCallsCredentialListMapping`](docs/sdks/api20100401authcallscredentiallistmapping/README.md#fetchsipauthcallscredentiallistmapping) - Fetch a specific instance of a credential list mapping
- [`api20100401AuthCallsCredentialListMappingListSipAuthCallsCredentialListMapping`](docs/sdks/api20100401authcallscredentiallistmapping/README.md#listsipauthcallscredentiallistmapping) - Retrieve a list of credential list mappings belonging to the domain used in the request
- [`api20100401AuthCallsIpAccessControlListMappingCreateSipAuthCallsIpAccessControlListMapping`](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#createsipauthcallsipaccesscontrollistmapping) - Create a new IP Access Control List mapping
- [`api20100401AuthCallsIpAccessControlListMappingDeleteSipAuthCallsIpAccessControlListMapping`](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#deletesipauthcallsipaccesscontrollistmapping) - Delete an IP Access Control List mapping from the requested domain
- [`api20100401AuthCallsIpAccessControlListMappingFetchSipAuthCallsIpAccessControlListMapping`](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#fetchsipauthcallsipaccesscontrollistmapping) - Fetch a specific instance of an IP Access Control List mapping
- [`api20100401AuthCallsIpAccessControlListMappingListSipAuthCallsIpAccessControlListMapping`](docs/sdks/api20100401authcallsipaccesscontrollistmapping/README.md#listsipauthcallsipaccesscontrollistmapping) - Retrieve a list of IP Access Control List mappings belonging to the domain used in the request
- [`api20100401AuthorizedConnectAppFetchAuthorizedConnectApp`](docs/sdks/api20100401authorizedconnectapp/README.md#fetchauthorizedconnectapp) - Fetch an instance of an authorized-connect-app
- [`api20100401AuthorizedConnectAppListAuthorizedConnectApp`](docs/sdks/api20100401authorizedconnectapp/README.md#listauthorizedconnectapp) - Retrieve a list of authorized-connect-apps belonging to the account used to make the request
- [`api20100401AuthRegistrationsCredentialListMappingCreateSipAuthRegistrationsCredentialListMapping`](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#createsipauthregistrationscredentiallistmapping) - Create a new credential list mapping resource
- [`api20100401AuthRegistrationsCredentialListMappingDeleteSipAuthRegistrationsCredentialListMapping`](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#deletesipauthregistrationscredentiallistmapping) - Delete a credential list mapping from the requested domain
- [`api20100401AuthRegistrationsCredentialListMappingFetchSipAuthRegistrationsCredentialListMapping`](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#fetchsipauthregistrationscredentiallistmapping) - Fetch a specific instance of a credential list mapping
- [`api20100401AuthRegistrationsCredentialListMappingListSipAuthRegistrationsCredentialListMapping`](docs/sdks/api20100401authregistrationscredentiallistmapping/README.md#listsipauthregistrationscredentiallistmapping) - Retrieve a list of credential list mappings belonging to the domain used in the request
- [`api20100401AvailablePhoneNumberCountryFetchAvailablePhoneNumberCountry`](docs/sdks/api20100401availablephonenumbercountry/README.md#fetchavailablephonenumbercountry)
- [`api20100401AvailablePhoneNumberCountryListAvailablePhoneNumberCountry`](docs/sdks/api20100401availablephonenumbercountry/README.md#listavailablephonenumbercountry)
- [`api20100401BalanceFetchBalance`](docs/sdks/api20100401balance/README.md#fetchbalance) - Fetch the balance for an Account based on Account Sid. Balance changes may not be reflected immediately. Child accounts do not contain balance information
- [`api20100401CallCreateCall`](docs/sdks/api20100401call/README.md#createcall) - Create a new outgoing call to phones, SIP-enabled endpoints or Twilio Client connections
- [`api20100401CallDeleteCall`](docs/sdks/api20100401call/README.md#deletecall) - Delete a Call record from your account. Once the record is deleted, it will no longer appear in the API and Account Portal logs.
- [`api20100401CallFetchCall`](docs/sdks/api20100401call/README.md#fetchcall) - Fetch the call specified by the provided Call SID
- [`api20100401CallListCall`](docs/sdks/api20100401call/README.md#listcall) - Retrieves a collection of calls made to and from your account
- [`api20100401CallNotificationFetchCallNotification`](docs/sdks/api20100401callnotification/README.md#fetchcallnotification)
- [`api20100401CallNotificationListCallNotification`](docs/sdks/api20100401callnotification/README.md#listcallnotification)
- [`api20100401CallTranscriptionCreateRealtimeTranscription`](docs/sdks/api20100401calltranscription/README.md#createrealtimetranscription) - Create a Transcription
- [`api20100401CallTranscriptionUpdateRealtimeTranscription`](docs/sdks/api20100401calltranscription/README.md#updaterealtimetranscription) - Stop a Transcription using either the SID of the Transcription resource or the `name` used when creating the resource
- [`api20100401CallUpdateCall`](docs/sdks/api20100401call/README.md#updatecall) - Initiates a call redirect or terminates a call
- [`api20100401ConferenceFetchConference`](docs/sdks/api20100401conference/README.md#fetchconference) - Fetch an instance of a conference
- [`api20100401ConferenceListConference`](docs/sdks/api20100401conference/README.md#listconference) - Retrieve a list of conferences belonging to the account used to make the request
- [`api20100401ConferenceUpdateConference`](docs/sdks/api20100401conference/README.md#updateconference)
- [`api20100401ConnectAppDeleteConnectApp`](docs/sdks/api20100401connectapp/README.md#deleteconnectapp) - Delete an instance of a connect-app
- [`api20100401ConnectAppFetchConnectApp`](docs/sdks/api20100401connectapp/README.md#fetchconnectapp) - Fetch an instance of a connect-app
- [`api20100401ConnectAppListConnectApp`](docs/sdks/api20100401connectapp/README.md#listconnectapp) - Retrieve a list of connect-apps belonging to the account used to make the request
- [`api20100401ConnectAppUpdateConnectApp`](docs/sdks/api20100401connectapp/README.md#updateconnectapp) - Update a connect-app with the specified parameters
- [`api20100401CredentialCreateSipCredential`](docs/sdks/api20100401credential/README.md#createsipcredential) - Create a new credential resource.
- [`api20100401CredentialDeleteSipCredential`](docs/sdks/api20100401credential/README.md#deletesipcredential) - Delete a credential resource.
- [`api20100401CredentialFetchSipCredential`](docs/sdks/api20100401credential/README.md#fetchsipcredential) - Fetch a single credential.
- [`api20100401CredentialListCreateSipCredentialList`](docs/sdks/api20100401credentiallist/README.md#createsipcredentiallist) - Create a Credential List
- [`api20100401CredentialListDeleteSipCredentialList`](docs/sdks/api20100401credentiallist/README.md#deletesipcredentiallist) - Delete a Credential List
- [`api20100401CredentialListFetchSipCredentialList`](docs/sdks/api20100401credentiallist/README.md#fetchsipcredentiallist) - Get a Credential List
- [`api20100401CredentialListListSipCredentialList`](docs/sdks/api20100401credentiallist/README.md#listsipcredentiallist) - Get All Credential Lists
- [`api20100401CredentialListMappingCreateSipCredentialListMapping`](docs/sdks/api20100401credentiallistmapping/README.md#createsipcredentiallistmapping) - Create a CredentialListMapping resource for an account.
- [`api20100401CredentialListMappingDeleteSipCredentialListMapping`](docs/sdks/api20100401credentiallistmapping/README.md#deletesipcredentiallistmapping) - Delete a CredentialListMapping resource from an account.
- [`api20100401CredentialListMappingFetchSipCredentialListMapping`](docs/sdks/api20100401credentiallistmapping/README.md#fetchsipcredentiallistmapping) - Fetch a single CredentialListMapping resource from an account.
- [`api20100401CredentialListMappingListSipCredentialListMapping`](docs/sdks/api20100401credentiallistmapping/README.md#listsipcredentiallistmapping) - Read multiple CredentialListMapping resources from an account.
- [`api20100401CredentialListSipCredential`](docs/sdks/api20100401credential/README.md#listsipcredential) - Retrieve a list of credentials.
- [`api20100401CredentialListUpdateSipCredentialList`](docs/sdks/api20100401credentiallist/README.md#updatesipcredentiallist) - Update a Credential List
- [`api20100401CredentialUpdateSipCredential`](docs/sdks/api20100401credential/README.md#updatesipcredential) - Update a credential resource.
- [`api20100401DailyListUsageRecordDaily`](docs/sdks/api20100401daily/README.md#listusagerecorddaily)
- [`api20100401DataFetchRecordingAddOnResultPayloadData`](docs/sdks/api20100401data/README.md#fetchrecordingaddonresultpayloaddata) - Fetch an instance of a result payload
- [`api20100401DependentPhoneNumberListDependentPhoneNumber`](docs/sdks/api20100401dependentphonenumber/README.md#listdependentphonenumber)
- [`api20100401DomainCreateSipDomain`](docs/sdks/api20100401domain/README.md#createsipdomain) - Create a new Domain
- [`api20100401DomainDeleteSipDomain`](docs/sdks/api20100401domain/README.md#deletesipdomain) - Delete an instance of a Domain
- [`api20100401DomainFetchSipDomain`](docs/sdks/api20100401domain/README.md#fetchsipdomain) - Fetch an instance of a Domain
- [`api20100401DomainListSipDomain`](docs/sdks/api20100401domain/README.md#listsipdomain) - Retrieve a list of domains belonging to the account used to make the request
- [`api20100401DomainUpdateSipDomain`](docs/sdks/api20100401domain/README.md#updatesipdomain) - Update the attributes of a domain
- [`api20100401EventListCallEvent`](docs/sdks/api20100401event/README.md#listcallevent) - Retrieve a list of all events for a call.
- [`api20100401FeedbackCreateMessageFeedback`](docs/sdks/api20100401feedback/README.md#createmessagefeedback) - Create Message Feedback to confirm a tracked user action was performed by the recipient of the associated Message
- [`api20100401IncomingPhoneNumberCreateIncomingPhoneNumber`](docs/sdks/api20100401incomingphonenumber/README.md#createincomingphonenumber) - Purchase a phone-number for the account.
- [`api20100401IncomingPhoneNumberDeleteIncomingPhoneNumber`](docs/sdks/api20100401incomingphonenumber/README.md#deleteincomingphonenumber) - Delete a phone-numbers belonging to the account used to make the request.
- [`api20100401IncomingPhoneNumberFetchIncomingPhoneNumber`](docs/sdks/api20100401incomingphonenumber/README.md#fetchincomingphonenumber) - Fetch an incoming-phone-number belonging to the account used to make the request.
- [`api20100401IncomingPhoneNumberListIncomingPhoneNumber`](docs/sdks/api20100401incomingphonenumber/README.md#listincomingphonenumber) - Retrieve a list of incoming-phone-numbers belonging to the account used to make the request.
- [`api20100401IncomingPhoneNumberLocalCreateIncomingPhoneNumberLocal`](docs/sdks/api20100401incomingphonenumberlocal/README.md#createincomingphonenumberlocal)
- [`api20100401IncomingPhoneNumberLocalListIncomingPhoneNumberLocal`](docs/sdks/api20100401incomingphonenumberlocal/README.md#listincomingphonenumberlocal)
- [`api20100401IncomingPhoneNumberMobileCreateIncomingPhoneNumberMobile`](docs/sdks/api20100401incomingphonenumbermobile/README.md#createincomingphonenumbermobile)
- [`api20100401IncomingPhoneNumberMobileListIncomingPhoneNumberMobile`](docs/sdks/api20100401incomingphonenumbermobile/README.md#listincomingphonenumbermobile)
- [`api20100401IncomingPhoneNumberTollFreeCreateIncomingPhoneNumberTollFree`](docs/sdks/api20100401incomingphonenumbertollfree/README.md#createincomingphonenumbertollfree)
- [`api20100401IncomingPhoneNumberTollFreeListIncomingPhoneNumberTollFree`](docs/sdks/api20100401incomingphonenumbertollfree/README.md#listincomingphonenumbertollfree)
- [`api20100401IncomingPhoneNumberUpdateIncomingPhoneNumber`](docs/sdks/api20100401incomingphonenumber/README.md#updateincomingphonenumber) - Update an incoming-phone-number instance.
- [`api20100401IpAccessControlListCreateSipIpAccessControlList`](docs/sdks/api20100401ipaccesscontrollist/README.md#createsipipaccesscontrollist) - Create a new IpAccessControlList resource
- [`api20100401IpAccessControlListDeleteSipIpAccessControlList`](docs/sdks/api20100401ipaccesscontrollist/README.md#deletesipipaccesscontrollist) - Delete an IpAccessControlList from the requested account
- [`api20100401IpAccessControlListFetchSipIpAccessControlList`](docs/sdks/api20100401ipaccesscontrollist/README.md#fetchsipipaccesscontrollist) - Fetch a specific instance of an IpAccessControlList
- [`api20100401IpAccessControlListListSipIpAccessControlList`](docs/sdks/api20100401ipaccesscontrollist/README.md#listsipipaccesscontrollist) - Retrieve a list of IpAccessControlLists that belong to the account used to make the request
- [`api20100401IpAccessControlListMappingCreateSipIpAccessControlListMapping`](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#createsipipaccesscontrollistmapping) - Create a new IpAccessControlListMapping resource.
- [`api20100401IpAccessControlListMappingDeleteSipIpAccessControlListMapping`](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#deletesipipaccesscontrollistmapping) - Delete an IpAccessControlListMapping resource.
- [`api20100401IpAccessControlListMappingFetchSipIpAccessControlListMapping`](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#fetchsipipaccesscontrollistmapping) - Fetch an IpAccessControlListMapping resource.
- [`api20100401IpAccessControlListMappingListSipIpAccessControlListMapping`](docs/sdks/api20100401ipaccesscontrollistmapping/README.md#listsipipaccesscontrollistmapping) - Retrieve a list of IpAccessControlListMapping resources.
- [`api20100401IpAccessControlListUpdateSipIpAccessControlList`](docs/sdks/api20100401ipaccesscontrollist/README.md#updatesipipaccesscontrollist) - Rename an IpAccessControlList
- [`api20100401KeyDeleteKey`](docs/sdks/api20100401key/README.md#deletekey)
- [`api20100401KeyFetchKey`](docs/sdks/api20100401key/README.md#fetchkey)
- [`api20100401KeyListKey`](docs/sdks/api20100401key/README.md#listkey)
- [`api20100401KeyUpdateKey`](docs/sdks/api20100401key/README.md#updatekey)
- [`api20100401LastMonthListUsageRecordLastMonth`](docs/sdks/api20100401lastmonth/README.md#listusagerecordlastmonth)
- [`api20100401LocalListAvailablePhoneNumberLocal`](docs/sdks/api20100401local/README.md#listavailablephonenumberlocal)
- [`api20100401MachineToMachineListAvailablePhoneNumberMachineToMachine`](docs/sdks/api20100401machinetomachine/README.md#listavailablephonenumbermachinetomachine)
- [`api20100401MediaDeleteMedia`](docs/sdks/api20100401media/README.md#deletemedia) - Delete the Media resource.
- [`api20100401MediaFetchMedia`](docs/sdks/api20100401media/README.md#fetchmedia) - Fetch a single Media resource associated with a specific Message resource
- [`api20100401MediaListMedia`](docs/sdks/api20100401media/README.md#listmedia) - Read a list of Media resources associated with a specific Message resource
- [`api20100401MemberFetchMember`](docs/sdks/api20100401member/README.md#fetchmember) - Fetch a specific member from the queue
- [`api20100401MemberListMember`](docs/sdks/api20100401member/README.md#listmember) - Retrieve the members of the queue
- [`api20100401MemberUpdateMember`](docs/sdks/api20100401member/README.md#updatemember) - Dequeue a member from a queue and have the member's call begin executing the TwiML document at that URL
- [`api20100401MessageCreateMessage`](docs/sdks/api20100401message/README.md#createmessage) - Send a message
- [`api20100401MessageDeleteMessage`](docs/sdks/api20100401message/README.md#deletemessage) - Deletes a Message resource from your account
- [`api20100401MessageFetchMessage`](docs/sdks/api20100401message/README.md#fetchmessage) - Fetch a specific Message
- [`api20100401MessageListMessage`](docs/sdks/api20100401message/README.md#listmessage) - Retrieve a list of Message resources associated with a Twilio Account
- [`api20100401MessageUpdateMessage`](docs/sdks/api20100401message/README.md#updatemessage) - Update a Message resource (used to redact Message `body` text and to cancel not-yet-sent messages)
- [`api20100401MobileListAvailablePhoneNumberMobile`](docs/sdks/api20100401mobile/README.md#listavailablephonenumbermobile)
- [`api20100401MonthlyListUsageRecordMonthly`](docs/sdks/api20100401monthly/README.md#listusagerecordmonthly)
- [`api20100401NationalListAvailablePhoneNumberNational`](docs/sdks/api20100401national/README.md#listavailablephonenumbernational)
- [`api20100401NewKeyCreateNewKey`](docs/sdks/api20100401newkey/README.md#createnewkey)
- [`api20100401NewSigningKeyCreateNewSigningKey`](docs/sdks/api20100401newsigningkey/README.md#createnewsigningkey) - Create a new Signing Key for the account making the request.
- [`api20100401NotificationFetchNotification`](docs/sdks/api20100401notification/README.md#fetchnotification) - Fetch a notification belonging to the account used to make the request
- [`api20100401NotificationListNotification`](docs/sdks/api20100401notification/README.md#listnotification) - Retrieve a list of notifications belonging to the account used to make the request
- [`api20100401OutgoingCallerIdDeleteOutgoingCallerId`](docs/sdks/api20100401outgoingcallerid/README.md#deleteoutgoingcallerid) - Delete the caller-id specified from the account
- [`api20100401OutgoingCallerIdFetchOutgoingCallerId`](docs/sdks/api20100401outgoingcallerid/README.md#fetchoutgoingcallerid) - Fetch an outgoing-caller-id belonging to the account used to make the request
- [`api20100401OutgoingCallerIdListOutgoingCallerId`](docs/sdks/api20100401outgoingcallerid/README.md#listoutgoingcallerid) - Retrieve a list of outgoing-caller-ids belonging to the account used to make the request
- [`api20100401OutgoingCallerIdUpdateOutgoingCallerId`](docs/sdks/api20100401outgoingcallerid/README.md#updateoutgoingcallerid) - Updates the caller-id
- [`api20100401ParticipantCreateParticipant`](docs/sdks/api20100401participant/README.md#createparticipant)
- [`api20100401ParticipantDeleteParticipant`](docs/sdks/api20100401participant/README.md#deleteparticipant) - Kick a participant from a given conference
- [`api20100401ParticipantFetchParticipant`](docs/sdks/api20100401participant/README.md#fetchparticipant) - Fetch an instance of a participant
- [`api20100401ParticipantListParticipant`](docs/sdks/api20100401participant/README.md#listparticipant) - Retrieve a list of participants belonging to the account used to make the request
- [`api20100401ParticipantUpdateParticipant`](docs/sdks/api20100401participant/README.md#updateparticipant) - Update the properties of the participant
- [`api20100401PayloadDeleteRecordingAddOnResultPayload`](docs/sdks/api20100401payload/README.md#deleterecordingaddonresultpayload) - Delete a payload from the result along with all associated Data
- [`api20100401PayloadFetchRecordingAddOnResultPayload`](docs/sdks/api20100401payload/README.md#fetchrecordingaddonresultpayload) - Fetch an instance of a result payload
- [`api20100401PayloadListRecordingAddOnResultPayload`](docs/sdks/api20100401payload/README.md#listrecordingaddonresultpayload) - Retrieve a list of payloads belonging to the AddOnResult
- [`api20100401PaymentCreatePayments`](docs/sdks/api20100401payment/README.md#createpayments) - create an instance of payments. This will start a new payments session
- [`api20100401PaymentUpdatePayments`](docs/sdks/api20100401payment/README.md#updatepayments) - update an instance of payments with different phases of payment flows.
- [`api20100401QueueCreateQueue`](docs/sdks/api20100401queue/README.md#createqueue) - Create a queue
- [`api20100401QueueDeleteQueue`](docs/sdks/api20100401queue/README.md#deletequeue) - Remove an empty queue
- [`api20100401QueueFetchQueue`](docs/sdks/api20100401queue/README.md#fetchqueue) - Fetch an instance of a queue identified by the QueueSid
- [`api20100401QueueListQueue`](docs/sdks/api20100401queue/README.md#listqueue) - Retrieve a list of queues belonging to the account used to make the request
- [`api20100401QueueUpdateQueue`](docs/sdks/api20100401queue/README.md#updatequeue) - Update the queue with the new parameters
- [`api20100401RecordingCreateCallRecording`](docs/sdks/api20100401recording/README.md#createcallrecording) - Create a recording for the call
- [`api20100401RecordingDeleteCallRecording`](docs/sdks/api20100401recording/README.md#deletecallrecording) - Delete a recording from your account
- [`api20100401RecordingDeleteConferenceRecording`](docs/sdks/api20100401recording/README.md#deleteconferencerecording) - Delete a recording from your account
- [`api20100401RecordingDeleteRecording`](docs/sdks/api20100401recording/README.md#deleterecording) - Delete a recording from your account
- [`api20100401RecordingFetchCallRecording`](docs/sdks/api20100401recording/README.md#fetchcallrecording) - Fetch an instance of a recording for a call
- [`api20100401RecordingFetchConferenceRecording`](docs/sdks/api20100401recording/README.md#fetchconferencerecording) - Fetch an instance of a recording for a call
- [`api20100401RecordingFetchRecording`](docs/sdks/api20100401recording/README.md#fetchrecording) - Fetch an instance of a recording
- [`api20100401RecordingListCallRecording`](docs/sdks/api20100401recording/README.md#listcallrecording) - Retrieve a list of recordings belonging to the call used to make the request
- [`api20100401RecordingListConferenceRecording`](docs/sdks/api20100401recording/README.md#listconferencerecording) - Retrieve a list of recordings belonging to the call used to make the request
- [`api20100401RecordingListRecording`](docs/sdks/api20100401recording/README.md#listrecording) - Retrieve a list of recordings belonging to the account used to make the request
- [`api20100401RecordingUpdateCallRecording`](docs/sdks/api20100401recording/README.md#updatecallrecording) - Changes the status of the recording to paused, stopped, or in-progress. Note: Pass `Twilio.CURRENT` instead of recording sid to reference current active recording.
- [`api20100401RecordingUpdateConferenceRecording`](docs/sdks/api20100401recording/README.md#updateconferencerecording) - Changes the status of the recording to paused, stopped, or in-progress. Note: To use `Twilio.CURRENT`, pass it as recording sid.
- [`api20100401RecordListUsageRecord`](docs/sdks/api20100401record/README.md#listusagerecord) - Retrieve a list of usage-records belonging to the account used to make the request
- [`api20100401SharedCostListAvailablePhoneNumberSharedCost`](docs/sdks/api20100401sharedcost/README.md#listavailablephonenumbersharedcost)
- [`api20100401ShortCodeFetchShortCode`](docs/sdks/api20100401shortcode/README.md#fetchshortcode) - Fetch an instance of a short code
- [`api20100401ShortCodeListShortCode`](docs/sdks/api20100401shortcode/README.md#listshortcode) - Retrieve a list of short-codes belonging to the account used to make the request
- [`api20100401ShortCodeUpdateShortCode`](docs/sdks/api20100401shortcode/README.md#updateshortcode) - Update a short code with the following parameters
- [`api20100401SigningKeyDeleteSigningKey`](docs/sdks/api20100401signingkey/README.md#deletesigningkey)
- [`api20100401SigningKeyFetchSigningKey`](docs/sdks/api20100401signingkey/README.md#fetchsigningkey)
- [`api20100401SigningKeyListSigningKey`](docs/sdks/api20100401signingkey/README.md#listsigningkey)
- [`api20100401SigningKeyUpdateSigningKey`](docs/sdks/api20100401signingkey/README.md#updatesigningkey)
- [`api20100401SipIpAddressCreateSipIpAddress`](docs/sdks/api20100401sipipaddress/README.md#createsipipaddress) - Create a new IpAddress resource.
- [`api20100401SipIpAddressDeleteSipIpAddress`](docs/sdks/api20100401sipipaddress/README.md#deletesipipaddress) - Delete an IpAddress resource.
- [`api20100401SipIpAddressFetchSipIpAddress`](docs/sdks/api20100401sipipaddress/README.md#fetchsipipaddress) - Read one IpAddress resource.
- [`api20100401SipIpAddressListSipIpAddress`](docs/sdks/api20100401sipipaddress/README.md#listsipipaddress) - Read multiple IpAddress resources.
- [`api20100401SipIpAddressUpdateSipIpAddress`](docs/sdks/api20100401sipipaddress/README.md#updatesipipaddress) - Update an IpAddress resource.
- [`api20100401SiprecCreateSiprec`](docs/sdks/api20100401siprec/README.md#createsiprec) - Create a Siprec
- [`api20100401SiprecUpdateSiprec`](docs/sdks/api20100401siprec/README.md#updatesiprec) - Stop a Siprec using either the SID of the Siprec resource or the `name` used when creating the resource
- [`api20100401StreamCreateStream`](docs/sdks/api20100401stream/README.md#createstream) - Create a Stream
- [`api20100401StreamUpdateStream`](docs/sdks/api20100401stream/README.md#updatestream) - Stop a Stream using either the SID of the Stream resource or the `name` used when creating the resource
- [`api20100401ThisMonthListUsageRecordThisMonth`](docs/sdks/api20100401thismonth/README.md#listusagerecordthismonth)
- [`api20100401TodayListUsageRecordToday`](docs/sdks/api20100401today/README.md#listusagerecordtoday)
- [`api20100401TokenCreateToken`](docs/sdks/api20100401token/README.md#createtoken) - Create a new token for ICE servers
- [`api20100401TollFreeListAvailablePhoneNumberTollFree`](docs/sdks/api20100401tollfree/README.md#listavailablephonenumbertollfree)
- [`api20100401TranscriptionDeleteRecordingTranscription`](docs/sdks/api20100401transcription/README.md#deleterecordingtranscription)
- [`api20100401TranscriptionDeleteTranscription`](docs/sdks/api20100401transcription/README.md#deletetranscription) - Delete a transcription from the account used to make the request
- [`api20100401TranscriptionFetchRecordingTranscription`](docs/sdks/api20100401transcription/README.md#fetchrecordingtranscription)
- [`api20100401TranscriptionFetchTranscription`](docs/sdks/api20100401transcription/README.md#fetchtranscription) - Fetch an instance of a Transcription
- [`api20100401TranscriptionListRecordingTranscription`](docs/sdks/api20100401transcription/README.md#listrecordingtranscription)
- [`api20100401TranscriptionListTranscription`](docs/sdks/api20100401transcription/README.md#listtranscription) - Retrieve a list of transcriptions belonging to the account used to make the request
- [`api20100401TriggerCreateUsageTrigger`](docs/sdks/api20100401trigger/README.md#createusagetrigger) - Create a new UsageTrigger
- [`api20100401TriggerDeleteUsageTrigger`](docs/sdks/api20100401trigger/README.md#deleteusagetrigger)
- [`api20100401TriggerFetchUsageTrigger`](docs/sdks/api20100401trigger/README.md#fetchusagetrigger) - Fetch and instance of a usage-trigger
- [`api20100401TriggerListUsageTrigger`](docs/sdks/api20100401trigger/README.md#listusagetrigger) - Retrieve a list of usage-triggers belonging to the account used to make the request
- [`api20100401TriggerUpdateUsageTrigger`](docs/sdks/api20100401trigger/README.md#updateusagetrigger) - Update an instance of a usage trigger
- [`api20100401UserDefinedMessageCreateUserDefinedMessage`](docs/sdks/api20100401userdefinedmessage/README.md#createuserdefinedmessage) - Create a new User Defined Message for the given Call SID.
- [`api20100401UserDefinedMessageSubscriptionCreateUserDefinedMessageSubscription`](docs/sdks/api20100401userdefinedmessagesubscription/README.md#createuserdefinedmessagesubscription) - Subscribe to User Defined Messages for a given Call SID.
- [`api20100401UserDefinedMessageSubscriptionDeleteUserDefinedMessageSubscription`](docs/sdks/api20100401userdefinedmessagesubscription/README.md#deleteuserdefinedmessagesubscription) - Delete a specific User Defined Message Subscription.
- [`api20100401ValidationRequestCreateValidationRequest`](docs/sdks/api20100401validationrequest/README.md#createvalidationrequest)
- [`api20100401VoipListAvailablePhoneNumberVoip`](docs/sdks/api20100401voip/README.md#listavailablephonenumbervoip)
- [`api20100401YearlyListUsageRecordYearly`](docs/sdks/api20100401yearly/README.md#listusagerecordyearly)
- [`api20100401YesterdayListUsageRecordYesterday`](docs/sdks/api20100401yesterday/README.md#listusagerecordyesterday)

</details>
<!-- End Standalone functions [standalone-funcs] -->

<!-- Start Retries [retries] -->
## Retries

Some of the endpoints in this SDK support retries.  If you use the SDK without any configuration, it will fall back to the default retry strategy provided by the API.  However, the default retry strategy can be overridden on a per-operation basis, or across the entire SDK.

To change the default retry strategy for a single API call, simply provide a retryConfig object to the call:
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  }, {
    retries: {
      strategy: "backoff",
      backoff: {
        initialInterval: 1,
        maxInterval: 50,
        exponent: 1.1,
        maxElapsedTime: 100,
      },
      retryConnectionErrors: false,
    },
  });

  // Handle the result
  console.log(result);
}

run();

```

If you'd like to override the default retry strategy for all operations that support retries, you can provide a retryConfig at SDK initialization:
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  retryConfig: {
    strategy: "backoff",
    backoff: {
      initialInterval: 1,
      maxInterval: 50,
      exponent: 1.1,
      maxElapsedTime: 100,
    },
    retryConnectionErrors: false,
  },
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End Retries [retries] -->

<!-- Start Error Handling [errors] -->
## Error Handling

If the request fails due to, for example 4XX or 5XX status codes, it will throw a `APIError`.

| Error Type      | Status Code | Content Type |
| --------------- | ----------- | ------------ |
| errors.APIError | 4XX, 5XX    | \*/\*        |

```typescript
import { TwilioSDK } from "twilio-sdk";
import { SDKValidationError } from "twilio-sdk/models/errors";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  let result;
  try {
    result = await twilioSDK.api20100401Account.createAccount({
      friendlyName: "friendly_name",
    });

    // Handle the result
    console.log(result);
  } catch (err) {
    switch (true) {
      // The server response does not match the expected SDK schema
      case (err instanceof SDKValidationError):
        {
          // Pretty-print will provide a human-readable multi-line error message
          console.error(err.pretty());
          // Raw value may also be inspected
          console.error(err.rawValue);
          return;
        }
        apierror.js;
      // Server returned an error status code or an unknown content type
      case (err instanceof APIError): {
        console.error(err.statusCode);
        console.error(err.rawResponse.body);
        return;
      }
      default: {
        // Other errors such as network errors, see HTTPClientErrors for more details
        throw err;
      }
    }
  }
}

run();

```

Validation errors can also occur when either method arguments or data returned from the server do not match the expected format. The `SDKValidationError` that is thrown as a result will capture the raw value that failed validation in an attribute called `rawValue`. Additionally, a `pretty()` method is available on this error that can be used to log a nicely formatted multi-line string since validation errors can list many issues and the plain error string may be difficult read when debugging.

In some rare cases, the SDK can fail to get a response from the server or even make the request due to unexpected circumstances such as network conditions. These types of errors are captured in the `models/errors/httpclienterrors.ts` module:

| HTTP Client Error                                    | Description                                          |
| ---------------------------------------------------- | ---------------------------------------------------- |
| RequestAbortedError                                  | HTTP request was aborted by the client               |
| RequestTimeoutError                                  | HTTP request timed out due to an AbortSignal signal  |
| ConnectionError                                      | HTTP client was unable to make a request to a server |
| InvalidRequestError                                  | Any input used to create a request is invalid        |
| UnexpectedClientError                                | Unrecognised or unexpected error                     |
<!-- End Error Handling [errors] -->

<!-- Start Server Selection [server] -->
## Server Selection

### Override Server URL Per-Client

The default server can also be overridden globally by passing a URL to the `serverURL: string` optional parameter when initializing the SDK client instance. For example:
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  serverURL: "https://api.twilio.com",
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  });

  // Handle the result
  console.log(result);
}

run();

```

### Override Server URL Per-Operation

The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
```typescript
import { TwilioSDK } from "twilio-sdk";

const twilioSDK = new TwilioSDK({
  security: {
    username: "",
    password: "",
  },
});

async function run() {
  const result = await twilioSDK.api20100401Account.createAccount({
    friendlyName: "friendly_name",
  }, {
    serverURL: "https://api.twilio.com",
  });

  // Handle the result
  console.log(result);
}

run();

```
<!-- End Server Selection [server] -->

<!-- Start Custom HTTP Client [http-client] -->
## Custom HTTP Client

The TypeScript SDK makes API calls using an `HTTPClient` that wraps the native
[Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). This
client is a thin wrapper around `fetch` and provides the ability to attach hooks
around the request lifecycle that can be used to modify the request or handle
errors and response.

The `HTTPClient` constructor takes an optional `fetcher` argument that can be
used to integrate a third-party HTTP client or when writing tests to mock out
the HTTP client and feed in fixtures.

The following example shows how to use the `"beforeRequest"` hook to to add a
custom header and a timeout to requests and how to use the `"requestError"` hook
to log errors:

```typescript
import { TwilioSDK } from "twilio-sdk";
import { HTTPClient } from "twilio-sdk/lib/http";

const httpClient = new HTTPClient({
  // fetcher takes a function that has the same signature as native `fetch`.
  fetcher: (request) => {
    return fetch(request);
  }
});

httpClient.addHook("beforeRequest", (request) => {
  const nextRequest = new Request(request, {
    signal: request.signal || AbortSignal.timeout(5000)
  });

  nextRequest.headers.set("x-custom-header", "custom value");

  return nextRequest;
});

httpClient.addHook("requestError", (error, request) => {
  console.group("Request Error");
  console.log("Reason:", `${error}`);
  console.log("Endpoint:", `${request.method} ${request.url}`);
  console.groupEnd();
});

const sdk = new TwilioSDK({ httpClient });
```
<!-- End Custom HTTP Client [http-client] -->

<!-- Start Debugging [debug] -->
## Debugging

You can setup your SDK to emit debug logs for SDK requests and responses.

You can pass a logger that matches `console`'s interface as an SDK option.

> [!WARNING]
> Beware that debug logging will reveal secrets, like API tokens in headers, in log messages printed to a console or files. It's recommended to use this feature only during local development and not in production.

```typescript
import { TwilioSDK } from "twilio-sdk";

const sdk = new TwilioSDK({ debugLogger: console });
```

You can also enable a default debug logger by setting an environment variable `TWILIOSDK_DEBUG` to true.
<!-- End Debugging [debug] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this SDK, this library is generated programmatically. Any manual changes added to internal files will be overwritten on the next generation. 
We look forward to hearing your feedback. Feel free to open a PR or an issue with a proof of concept and we'll do our best to include it in a future release. 

### SDK Created by [Speakeasy](https://www.speakeasy.com/?utm_source=twilio-sdk&utm_campaign=typescript)
