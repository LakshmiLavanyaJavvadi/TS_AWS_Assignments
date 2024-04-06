[IAM POLICY JSON.docx](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/files/14894642/IAM.POLICY.JSON.docx)


<ins>**Version:**</ins>
Specifies the version of the policy language. In this case, it's "2012-10-17".

<ins>**Statement:**</ins>
Contains one or more statements defining permissions.

<ins>**a. First Statement:**</ins>

**- Action:** Lists the actions allowed for S3 operations, such as PutObject, GetObject, ListBucket, etc.

**- Resource:** Specifies the ARN (Amazon Resource Name) of S3 buckets and objects to which the actions apply. The "*" wildcard is used for matching multiple resources.

**- Effect:** Indicates whether the actions are allowed or denied. In this case, it's "Allow".

<ibns>**b. Second Statement:**</ins>

**- Action:** Lists the actions allowed for S3 operations, similar to the first statement.

**- Resource:** Specifies the ARN of specific S3 buckets and objects in the "us/washington" directory.

**- Effect:** Indicates whether the actions are allowed or denied. In this case, it's "Allow".
