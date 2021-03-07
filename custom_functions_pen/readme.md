
# Validation Library Functions
- IsValidEmail
- IsValidURL
- IsValidIPAddress
- IsValidInternationalPhoneNumber
- IsValidUKPhoneNumber
- IsValidUSPhoneNumber
- IsValidCanadianPhoneNumber
- IsValidUKNationalInsuranceNumber
- IsValidUKDrivingLicenceNumber
- IsValidUKPassport
- IsValidNHSNumber

## IsValidEmail
Regex to validate email address format using the following REGEX for validation:
> ^([a-zA-Z0-9_\-\.]+)@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.)|(([a-zA-Z0-9\-]+\.)+))([a-zA-Z]{2,4}|[0-9]{1,3})(\]?)$
### Syntax
IsValidEmail(EmailToCheck)
* EmailToCheck: Required
### Output
* Boolean
</br></br>

## IsValidURL
Regex to validate URLs format using the following REGEX for validation:
> ^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?
### Syntax
IsValidURL(URLToCheck)
* URLToCheck: Required
### Output
* Boolean
</br></br>

## IsValidIPAddress
Regex to validate IPv4 Addresses format using the following REGEX for validation:
> /^(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/
### Syntax
IsValidIPAddress(IPtoCheck)
* IPtoCheck: Required
### Output
* Boolean
</br></br>

## IsValidInternationalPhoneNumber
Regex to validate international phone numbers using the following REGEX for validation:
> \\+(9[976]\d|8[987530]\d|6[987]\d|5[90]\d|42\d|3[875]\d|2[98654321]\d|9[8543210]|8[6421]|6[6543210]|5[87654321]|4[987654310]|3[9643210]|2[70]|7|1)\d{1,14}$
### Syntax
IsValidInternationalPhoneNumber(InternationalPhoneNumberToCheck)
* InternationalPhoneNumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUKPhoneNumber
Regex to validate UK phone number format using the following REGEX for validation:
> ^(?:(?:\(?(?:0(?:0|11)\)?[\s-]?\(?|\+)44\)?[\s-]?(?:\(?0\)?[\s-]?)?)|(?:\(?0))(?:(?:\d{5}\)?[\s-]?\d{4,5})|(?:\d{4}\)?[\s-]?(?:\d{5}|\d{3}[\s-]?\d{3}))|(?:\d{3}\)?[\s-]?\d{3}[\s-]?\d{3,4})|(?:\d{2}\)?[\s-]?\d{4}[\s-]?\d{4}))(?:[\s-]?(?:x|ext\.?|\#)\d{3,4})?$
### Syntax
IsValidUKPhoneNumber(UKPhoneNumberToCheck)
* UKPhoneNumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUSPhoneNumber
Regex to validate US Phone number format using the following REGEX for validation:
> 1?\W*([2-9][0-8][0-9])\W*([2-9][0-9]{2})\W*([0-9]{4})(\se?x?t?(\d*))?
### Syntax
IsValidUSPhoneNumber(USPhoneNumberToCheck)
* USPhoneNumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidCanadianPhoneNumber
Regex to validate Canadian Phone numbers format using the following REGEX for validation:
> ^(?:(?:\+?1\s*(?:[.-]\s*)?)?(?:\(\s*([2-9]1[02-9]|[2-9][02-8]1|[2-9][02-8][02-9])\s*\)|([2-9]1[02-9]|[2-9][02-8]1|[2-9][02-8][02-9]))\s*(?:[.-]\s*)?)?([2-9]1[02-9]|[2-9][02-9]1|[2-9][02-9]{2})\s*(?:[.-]\s*)?([0-9]{4})(?:\s*(?:#|x\.?|ext\.?|extension)\s*(\d+))?$
### Syntax
IsValidCanadianPhoneNumber(CanadianPhoneNumberToCheck)
* CanadianPhoneNumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUKNationalInsuranceNumber
Regex to validate UK Ntional Insurance numbers format using the following REGEX for validation:
> ^(?!BG)(?!GB)(?!NK)(?!KN)(?!TN)(?!NT)(?!ZZ)(?:[A-CEGHJ-PR-TW-Z][A-CEGHJ-NPR-TW-Z])(?:\s*\d\s*){6}([A-D]|\s)$
### Syntax
IsValidUKNationalInsuranceNumber(UKNINumberToCheck)
* UKNINumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUKPassport
Regex to validate UK Passport Numbers format using the following REGEX for validation:
> ^[0-9]{10}GBR[0-9]{7}[U,M,F]{1}[0-9]{9}$
### Syntax
IsValidUKPassport(UKPassportToCheck)
* UKPassportToCheck: Required
### Output
* Boolean
</br></br>

## IsValidNHSNumber
Regex to validate UK NHS Numbers format using the following REGEX for validation:
> \b\d{3}\s\d{3}\s\d{4}\b
### Syntax
IsValidNHSNumber(NHSNumberToCheck)
* NHSNumberToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUKDrivingLicence
Regex to validate UK Passport Numbers format using the following REGEX for validation:
> ^([A-Z]{2}[9]{3}|[A-Z]{3}[9]{2}|[A-Z]{4}[9]{1}|[A-Z]{5})[0-9]{6}([A-Z]{1}[9]{1}|[A-Z]{2})[A-Z0,9]{3}$
### Syntax
IsValidUKDrivingLicence(UKDrivingLicenceToCheck)
* UKDrivingLicenceToCheck: Required
### Output
* Boolean
</br></br>

## IsValidUSSocialSecurityNumber
Regex to validate UK Passport Numbers format using the following REGEX for validation:
> \b[\d]{3} [\d]{2} [\d]{4}|([\d] ?){3}[\—\-_] ?([\d] ?){2}[\—\-_] ?([\d] ?){4}\b
### Syntax
IsValidUSSocialSecurityNumber(USSNToCheck)
* USSNToCheck: Required
### Output
* Boolean
</br></br>


## IsValidCreditCard
Regex to validate UK Passport Numbers format using the following REGEX for validation:
> \b[\d]{3} [\d]{2} [\d]{4}|([\d] ?){3}[\—\-_] ?([\d] ?){2}[\—\-_] ?([\d] ?){4}\b
### Syntax
IsValidCreditCard(CCtoCheck)
* CCtoCheck: Required
### Output
* Boolean
</br></br>
