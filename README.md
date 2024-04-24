# windows-eda-ai

Used winlogfile to send logs to kafka




Payload from Kafka: 

Example of Event - json:

{"@timestamp":"2023-10-06T00:06:05.388Z","@metadata":{"beat":"winlogbeat","type":"_doc","version":"8.10.2"},"event":{"kind":"event","provider":"Microsoft-Windows-Security-Auditing","outcome":"success","action":"User Account Management","created":"2023-10-06T00:06:07.111Z","code":"4722"},"agent":{"type":"winlogbeat","version":"8.10.2","ephemeral_id":"2b9c058f-34ed-4c75-a5ec-12bc3da17947","id":"a6957f95-a905-403f-bb3a-3b7d19ed8db2","name":"wenad"},"ecs":{"version":"8.0.0"},"log":{"level":"information"},"message":"A user account was enabled.\n\nSubject:\n\tSecurity ID:\t\tS-1-5-21-1710834816-1814834527-228447583-500\n\tAccount Name:\t\tAdministrator\n\tAccount Domain:\t\tWINDOWS01\n\tLogon ID:\t\t0x3D956\n\nTarget Account:\n\tSecurity ID:\t\tS-1-5-21-1710834816-1814834527-228447583-1114\n\tAccount Name:\t\tses\n\tAccount Domain:\t\tWINDOWS01","host":{"name":"wenad","mac":["52-54-00-34-15-27"],"hostname":"wenad","architecture":"x86_64","os":{"build":"20348.1970","type":"windows","platform":"windows","version":"10.0","family":"windows","name":"Windows Server 2022 Datacenter Evaluation","kernel":"10.0.20348.1970 (WinBuild.160101.0800)"},"id":"b2ee90f1-d4e1-4ba3-962e-5b5e5a0b936f","ip":["fe80::d706:39bb:7a8d:ffb1","192.168.89.209"]},"winlog":{"computer_name":"wenad.prometheus.io","record_id":155252,"keywords":["Audit Success"],"provider_name":"Microsoft-Windows-Security-Auditing","api":"wineventlog","channel":"Security","event_id":"4722","task":"User Account Management","process":{"pid":652,"thread":{"id":5836}},"opcode":"Info","provider_guid":"{54849625-5478-4994-a5ba-3e3b0328c30d}","event_data":{"SubjectDomainName":"WINDOWS01","SubjectLogonId":"0x3d956","TargetUserName":"ses","TargetDomainName":"WINDOWS01","TargetSid":"S-1-5-21-1710834816-1814834527-228447583-1114","SubjectUserSid":"S-1-5-21-1710834816-1814834527-228447583-500","SubjectUserName":"Administrator"}}}
