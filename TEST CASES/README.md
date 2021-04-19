# TEST PLAN FOR HIGH LEVEL REQUIREMENTS:
|**Serial Number**|**TEST ID**|**TESTING FUNCTION**|**EXPECTED INPUT**|**EXPECTED OUTPUT**|
| :- | :- | :- | :- | :- | 
|1|HLR_1|Interior lighting|Any kind of motion detected in the PIR Motion Sensor (for example when the door is open then the motion is detected)|The interior lighting will work properly|
|2|HLR_2|Seat Control Feature|Any kind of displacement of the knob in the potentiometer sensor|Based on the ADC value of the pot sensor, the seat will move accordingly.|


# TEST PLAN FOR LOW LEVEL REQUIREMENTS:
|**Serial Number**|**TEST ID**|**TESTING FUNCTION**|**EXPECTED INPUT**|**EXPECTED OUTPUT**|
| :- | :- | :- | :- | :- | 
|1|HLR_1_LLR_1|Interior lighting|When the input Is 1 i.e. when the motion is detected|The blue LED will glow i.e. the GPIO pin 15 will be set.|
|2|HLR_1_LLR_2|Interior lighting|When the input Is 0 i.e. when no motion is detected|The blue LED will stop i.e. the GPIO pin 15 will be reset.|
|3|HLR_2_LLR_3|Seat Control Feature|When the ADC value is from 0 to 1500 |The GPIO pin 14 will be set i.e. the red LED will glow.The GPIO pin 15 will be reset.|
|4|HLR_2_LLR_4|Seat Control Feature|When the ADC value is greater than 3000 |The GPIO pin 15 will be set i.e. the blue LED will glow.The GPIO pin 14 will be reset.|

