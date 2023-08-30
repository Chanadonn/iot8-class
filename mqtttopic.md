## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6420301002/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}

1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6420301002/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"fabric": "cotton"}
        - {"weight": "13"}
        - {"filter": "normal"}
        - {"flow": "75"}
        - {"level": "medium"}
        - {"foam": "36"}
        - {"voice": "1.9"}
        - {"air": "428"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6420301002/model-01/sn-001
    - payload
        - {"human": "none"}
        - {"voice": "start"}
        - {"lid": "lock"}
        - {"gesture": "pause"}
        - {"door": "close"}
        - {"pump": "loading"}
        - {"heat": "37"}



