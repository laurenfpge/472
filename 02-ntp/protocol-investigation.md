# NTP Protocol Design Investigation

## Investigation 1: [Topic You Chose]

### Implementation Context
```c
unix_seconds = ntp_seconds - NTP_EPOCH_OFFSET;
// Where NTP_EPOCH_OFFSET = 2208988800 (70 years in seconds)
```
When implementing this calculation, I kept confusing whether I add the difference or subtract it. I also wondered why we have two different times that we reference, and why don't have a single standard. 

### Investigation Journey  
1. [Me] "Why do we use unix and ntp time?" -> [ChatGPT] "Unix time is an efficient format for storing and calculating time internally, while NTP is a protocol for synchronizing computer clocks to an accurate, universal standard."
2. "What are leap seconds?" -> "A leap second is an extra second occasionally added to our clocks to keep atomic time aligned with Earth’s rotation."
3. "Was unix was invented after ntp? Why did we add unix when we already had ntp?" -> "It’s actually: Unix first → NTP later... When Unix was designed: Computers were mostly standalone, Networking was primitive or nonexistent... By the time NTP was invented: Unix time was deeply baked into operating systems, Filesystems, APIs, programs all assumed Unix time"
4. "Why does ntp start from 1900?" -> "NTP starts counting time from 1900 because it inherited its design from earlier scientific and military time systems, and that choice made engineering sense for long-running, high-precision clocks."
5. "Why don't we update unix to match ntp and start from 1900?" -> "We don’t update Unix time to start from 1900 because the cost of changing it would be catastrophic, while the benefit would be small."

### Design Rationale
[Your synthesis - why this design, what tradeoffs, why alternatives fail]

### Implementation Insight
[Your "aha moment" - how this changed your understanding]

---

## Investigation 2: [Your Second Topic]

### Implementation Context
[What you coded and what puzzled you]

### Investigation Journey
[Your research/exploration process]

### Design Rationale
[Your synthesis in your own words]

### Implementation Insight
[What you learned from implementing]
