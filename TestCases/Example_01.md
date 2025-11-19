-	PASSED TC 1.7 Clear AVB for [DateFrom= “2024-08-01” - DateTo="2024-08-04"]
<br><br>

WHEN in REDACTED the room has Rate 1<br>
AND avb DateFrom= “2024-08-01” and DateTo="2024-08-04" is modified as 2 instead of 1<br>
AND set method is executed for the date range 2024-08-01 - 2024-08-04<br>
AND API response is a success<br>
AND get method is executed for REDACTED and the date range 2024-08-01 - 2024-08-04<br>
THEN avb returned for the date range 2024-08-01 - 2024-08-04 is equal 2<br>
AND clear method is executed for REDACTED and the date 2024-08-02<br>
AND get method is executed for REDACTED and the date range 2024-08-01 - 2024-08-04<br>
THEN avb returned for Rate 1 and the date 2024-08-01 is equal 2<br>
AND avb returned for Rate 1 and the date 2024-08-02 is equal 1<br>
AND avb returned for Rate 1 and the date 2024-08-03 is equal 2<br>
AND avb returned for Rate 1 and the date 2024-08-04 is equal 2<br>


Date: Jul 9, 2024<br>
Test result: PASSED	<br>
Comment:<br>
	
```
<CM_Push_ClearManualRateOverrides_RS>
    <Status ID="0">Success</Status>
    <ResponseID>349fc09db7b24caebc83644089c4b7cf</ResponseID>
</CM_Push_ClearManualRateOverrides_RS>


<CM_Pull_ListManualRateOverrides_RS>
    <Status ID="0">Success</Status>
    <ResponseID>cc021b884b504502b0b734ae9355663a</ResponseID>
    <Channels>
        <Channel Id="421402">
            <Overrides>
                <Override RateId="1275549" DateFrom="2024-08-01" DateTo="2024-08-01">
                    <Availability>2</Availability>
                </Override>
                <Override RateId="1275549" DateFrom="2024-08-03" DateTo="2024-08-03">
                    <Availability>2</Availability>
                </Override>
            </Overrides>
        </Channel>
    </Channels>
</CM_Pull_ListManualRateOverrides_RS>
```
