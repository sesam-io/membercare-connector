# membercare-connector

```
$ curl 'https://hoyre-rest-test.membercare.no/api/v1/token?clientApiKey=6ae1f9[..]52c3c44f&personToImpersonate=1'
{"value":"e9f77302-5060-498a-b0eb-4ffb82f06a59","expiration":"2024-02-14T15:34:50"}

$ curl 'https://hoyre-rest-test.membercare.no/api/v1/persons?pageSize=1' -H "token: 9e505ac7-43bc-4dc0-9664-200100ab47af" | jq .
{
  "totalCount": 74640,
  "totalPages": 74640,
  "previousPageUrl": null,
  "nextPageUrl": "https://hoyre-rest-test.membercare.no/api/v1/persons?pageSize=1&page=2",
  "result": [
    {
      "relationsLink": "https://hoyre-rest-test.membercare.no/api/v1/persons/2/family",
      "firstname": "Konvertering",
      "gender": 0,
      "birthDate": null,
      "age": null,
      "lastname": "Membercare",
      "nameHistory": null,
      "honorific": null,
      "customFieldValuesLink": "https://hoyre-rest-test.membercare.no/api/v1/persons/2/customFields/values",
      "membershipsLink": "https://hoyre-rest-test.membercare.no/api/v1/persons/2/memberships",
      "boardmembershipsLink": "https://hoyre-rest-test.membercare.no/api/v1/persons/2/boardMemberships",
      "password": null,
      "webUserId": null,
      "socialSecurityNumber": {
        "number": null,
        "iso2Letter": "NO"
      },
      "internalUserInfo": null,
      "externalSystemInfo": {
        "groupcareCommunityId": "2Per",
        "url": null
      },
      "loginToken": null,
      "allowSms": false,
      "allowEmail": true,
      "unionRepresentatives": null,
      "unionGroups": null,
      "employments": null,
      "memberships": null,
      "boardMemberships": null,
      "identity": null,
      "anonymizedOn": null,
      "text": null,
      "consents": [],
      "acceptedTerms": null,
      "foreignSystemMappings": [],
      "preferredAddress": null,
      "preferredContact": 1,
      "salarySystemIdentification": null,
      "temporary": false,
      "interests": [],
      "bankRegistrationNumber": null,
      "bankAccountNumber": null,
      "profilePictureIdentification": null,
      "debtorAccountNumber": "2",
      "name": "Konvertering Membercare",
      "contacts": [],
      "addresses": [],
      "customFieldValues": [],
      "invoicesLink": null,
      "memberType": 1,
      "defaultPayerLink": null,
      "dafualtPayerRule": 1,
      "closeDate": null,
      "einvoiceEan": null,
      "einvoiceEmail": null,
      "closeReason": null,
      "defaultAddressType": null,
      "externalId": null,
      "lastChange": "2016-01-01T00:00:00",
      "financeType": 0,
      "url": "https://hoyre-rest-test.membercare.no/api/v1/persons/2"
    }
  ]
}
```
