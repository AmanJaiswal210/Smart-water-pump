# Smart-water-pump
• Turn on the system; the Arduino will self-diagnose the circuit (which can be witnessed via LCD display) and sends an SMS saying “Motor OFF, System is ready”. Only then you can make call to the GSM module.
• Now, make a call to the GSM module from the mobile number which you entered in the program code.
• The relay turns ON and returns with an SMS acknowledgement saying “Motor is ON”.
• Now make another call it will de-energize the relay and returns with acknowledgement SMS saying “Motor is OFF / System is ready”.
• After making a call to the GSM module, Arduino automatically hang the call after a couple of rings.
• If you hear the voice info “The subscriber is switched OFF” after a call, there might be a power outage.
• If you hear anything per-recorded voice info related to network issue, the call might not reach the GSM module and will not trigger the relay.
• If you get “Motor is ON”acknowledgement SMSfor the second time after sometime you turned on the motor pump, you can assume the system and the motor just resumed after a power outage. Same applies,if you get “Motor is OFF / System ready” acknowledgement for the seconds time.
