## 1. Learning Process
(1-2 paragrpahs answering questions 1-4)

## 2. Real-World Failure 
(2 paragraphs, one describing the incident, one analyzing)

## 3. Physical vs Logical Time 
(2 paragraphs, one explaining lamport clocks, one why still need wall-clock time)

## 4. CAP & Eventual Consistency 
(2 paragraphs, one definitions, one connecting NTP)

## 5. Your NTP Client in Context 
(A)


(B)
**Synthesis questions - connect all the concepts:**

1. **Can your NTP client solve the logical ordering problem from Section 3?**
   - Yes or No?
   - Explain why in 1-2 sentences

2. **What does your NTP client actually provide?**
   
   Pick the BEST answer and explain your choice:
   - [ ] A way to order all events in a distributed system
   - [ ] A shared reference time for logs, certificates, and coordination
   - [ ] Perfect synchronization between all machines
   - [ ] A replacement for logical clocks like Lamport clocks
   
   **Your choice:** _____
   
   **Why?** (2-3 sentences)

3. **Complete the picture:**
   Fill in these statements based on everything you learned:
   
   - "Physical clocks (NTP) are needed for: _______________________"
   - "Logical clocks (Lamport) are needed for: _______________________"
   - "In a real distributed system, you typically need: _______________________"
