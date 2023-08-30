## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"humidity": "60"}
        - {"hall": "close"}
        - {"water_level": "5"}
        - {"saving_water": "5"}
        - {"water_pressure": "0"}
        - {"balance_position": "0"}
        - {"energy_efficiency": "2000"}
        - {"low_acoustic_noise": "10"}
        - {"uvc": "0"}
        - {"capacity": "10"}

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"Radar": "0"}
        - {"temperature": "26"}
        - {"humidity": "50"}
        - {"air_pressure": "medium"}
        - {"touch_mode": "cleaning"}
        - {"top_weight": "0"}
        - {"button": "on"}




