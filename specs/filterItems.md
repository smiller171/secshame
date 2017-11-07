`filterItems([], {})` takes an array of items and an `options` object as arguments and returns a filtered array of items.

## Options
{
  company: STRING,
  bizType: STRING,
  issueType: STRING,
  minReportDate: DATE,
  maxReportDate: DATE,
  isReportedResolved: BOOL,
  isResolved: BOOL,
  hasEmail: BOOL,
  hasTwitter: BOOL,
  hasGPlus: BOOL,
  hasFacebook: BOOL,
  hasPhone: BOOL,
  minSevRate: INT,
  maxSevRate: INT,
  minAnnoyRate: INT,
  maxAnnoyRate: INT,
  minFunnyRate: INT,
  maxFunnyRate: INT,
  reportedBy: STRING
}

| Option | example | Type | Default | Matches |
|--------------------|----------------------------------------------|--------------------------------------------------|---------|-----------------------------------------------------------------------|
| company | google / [ google, apple ] | STRING / ARRAY of STRINGs | none | exact match of string, any in array |
| bizType | financial / [ financial, commerce ] | STRING / ARRAY of STRINGs | none | exact match of string, any in array |
| issueType |  | STRING / ARRAY of STRINGs | none | exact match of string, any in array |
| minReportDate | 1464753600000 | DATE string | none | matches anything after DATE |
| maxReportDate | 1464753600000 | DATE string | none | matches anything before DATE |
| isReportedResolved | true / false | BOOL | none | match only issues reported resolved, or not |
| isResolved | true / false / any | BOOL / STRING("any") | false | match only issues confirmed resolved, or not |
| hasEmail | true / false | BOOL | none | match only issues with email address on file, or not |
| hasTwitter | true / false | BOOL | none | match only issues with Twitter handle on file, or not |
| hasGPlus | true / false | BOOL | none | match only issues with Google+ account on file, or not |
| hasFacebook | true / false | BOOL | none | match only issues with Facebook account on file, or not |
| hasPhone | true / false | BOOL | none | match only issues with phone number on file, or not |
| minSevRate | 1-10 | INT | none | match issues with severity above VAL |
| maxSevRate | 1-10 | INT | none | match issues with severity below VAL |
| minAnnoyRate | 1-10 | INT | none | match issues with annoyance above VAL |
| maxAnnoyRate | 1-10 | INT | none | match issues with annoyance below VAL |
| minFunnyRate | 1-10 | INT | none | match issues with funniness above VAL |
| maxFunnyRate | 1-10 | INT | none | match issues with funniness below VAL |
| reportedBy | Scott Miller | STRING | none | match issues reported by VAL |
