# Application-1-Abarrass
Required resources for Application 1 submission
Application 1: Alexander Barrass 5346980

Theme: My security oriented system is in charge of observing an unknown anomaly after being contained within the secure faciltiy in which it is studied. It updates regularly as the behavior of said phenomenon has not be deciphered and could pose a large threat, alive or inanimate alike. The LED is changed Yellow to invoke a feeling of caution and I changed the GPIO pin to 4. This system needs to be real time system with tendencies of a hard RTS becuase of both the severity of it's task and the accuracy in which a fast response would require from the alert system.

Q1: After setting the priority of print to 2, we see that during moments where both tasks are simultaneosly prompted, we see the print statement come out first on our console. That means that if we add a delay to the print statement, and it executes first, we will see the timing of the LED thrown off slightly as our print statement occupies time before allowing the LED to execute. Additional characters typically will not effect this unless in massive amounts.

Q2: Period = 1/f
	LED: 1/2Hz = 0.5s
	Print: 1/0.1Hz = 10s
Q3: The system does meet the timing requirements, the online simulation software Wokwi shows a running stopwatch in which we can match the period of each task to its actual runtime reoccurance.

Q4:Yes using a single loop for both the LED and the Print statement can cause a miss on timing for the LED as occasionally, approximately every 10 seconds the print statement loads and can steal resources from the LED causing a slight delay in it's function of blinking. Since we use two functions/tasks for this assignment, when the period for both the LED and the print statement land on the same time, they both operate simultaneously rather linearly meaning that they cannot delay the other.
