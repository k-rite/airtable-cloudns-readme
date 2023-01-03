Trigger

API Only Trigger when "API Trigger" is marked tick & "Console Log" field is empty.
Remember

Do not change any field name.
Make sure data doesn't contain unintentional space.
Do not delete an unfullfilled row, Once API is triggered it will add that record.
Records:

caa_flag
0 - Non critical or 128 - Critical
caa_type
Type of CAA record. The available flags are issue, issuewild, iodef.
caa_value
If caa_type is issue, caa_value can be hostname or ";". If caa_type is issuewild, it can be hostname or ";". If caa_type is iodef, it can be "mailto:someemail@address.tld, http://example.tld or http://example.tld.
ttl
Available TTL's: 60 = 1 minute, 2592000 = 1 month
Priority
For MX / SRV Records
Port
For SRV Records
Weight
For SRV Records
Cert Type
Type of the Certificate/CRL.
Cert Key Tag
A numeric value (0-65535), used the efficiently pick a CERT record.
Cert Algorithm
A numeric value (0-65535), used the efficiently pick a CERT record.
Troubleshooting

Record isn't added?
Checkout what console log mentioned, It can be unwanted space somewhere in records, incorrect record value.
It stopped adding records!
Don't worry, Just wait for it to respond, Give it 5mins so it can resolve on it's own.
If there's a bulk record addition, then it takes record one at a time so it will eventually add that record too!
Make sure "Console log" is empty and API Trigger is tick marked.
Unwanted Record is added
Once API is triggered and values provide in feild are correct then it will add that record. Any change after that will not change the prev added record, It will be added again as a new record.
