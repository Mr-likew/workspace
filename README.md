# workspace
auto answer modes

There are 3 modes of auto answer:
1.	Interphony  
2.	3PCC (using notify event)
3.	Answer mode according to RFC 5373.

And four parameters need to be set according the following table:

                           Interphony(local)	   3pcc (notify event)客户端	Answer mode RFC 5373（服务器）.
TelephonyInterphonyAllowed	TRUE		
TelephonyInterphonyStatus	TRUE		
SIPAutoAnsweredAllowed		                        TRUE                      TRUE
RFC5373Allowed	

		                                                                  TRUE

showSetting RFC5373Allowed

showSetting SIPAutoAnsweredAllowed
showSetting TelephonyInterphonyAllowed

call SettingsManager:setSettingValue 'SIPPreferredVocoder' string:'119'

call SettingsManager:setSettingValue 'SIPAutoAnsweredAllowed' string:'true'
call SettingsManager:setSettingValue 'TelephonyInterphonyStatus' string:'true'

call SettingsManager:setSettingValue 'SIPAutoAnsweredAllowed' string:'true'
call SettingsManager:setSettingValue 'RFC5373Allowed' string:'true'
