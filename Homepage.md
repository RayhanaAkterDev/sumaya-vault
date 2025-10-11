---
title: Homepage
---
# Homepage

_Welcome, Sumaya!_  
📅 [[2025-10-01|2025-10-01]]  

```button
name New note
type command
action Create new note
color blue
```
^button-balp

---

##### Calendar View

```dataview
CALENDAR date(file.name)
FROM "@journal/@daily-notes"
```

---

## Goals & Progress

 ##### Motto & Goals:

- Academic Excellence [^1]
- Personal & Spiritual Growth [^2]
- Skill Development [^3]
- Work Ethic [^4]
 
 ##### Learning Progress:
 
> **Current**: Phase 2 – JavaScript Core Concepts 

- [[02 Coding Roadmap|See the full roadmap →]]
- [[03 Select Niche|See your niche roadmap]]



---

## Quick Access

> [!multi-column]
> 
>> [!quote]+ 
>> ##### Folder Notes
>> ```dataview
>> list
>> from "/"
>> where length(split(file.folder, "/")) = 1
>> and file.name = regexreplace(file.folder, ".*/", "")
>> or file.folder = ""
>> sort file.name asc
>> ```
>
>> [!abstract]+
>> ##### Dataview Records
>> ```dataview
>> 	list from "@trailhead"
>> 	where file.name != "@trailhead"
>>```

---

## Study Materials — _[[5th Semester|DIIT 5th Semester]]_

> [!blank]
> ```dataview
> 	table from "@questhub/5th Semester"
> 	where contains(file.folder, file.name)
> 	  and length(split(file.folder, "/")) = length(split("@questhub/5th Semester", "/")) + 1
>  ```

[^1]: - Beat Rafi in Mid and External Finals  
	- Get 4.00 CGPA in 5th Semester Final  
	- Get 4.00 CGPA in 7th Semester Final  
	- Prove my worth to Tushar & Alvi  

[^2]: - Proper diet & exercise
	- Follow skin & hair care 
	- Pray 5 times Salat daily

[^3]:  - Master JavaScript  
	 - Master React  
	 - Master Laravel  
	 - Master Database Systems  
	 - Become confident in Full-Stack (Frontend + Backend)  
	 - Build and complete Real-World Projects  

[^4]: _Maintain 14-hour daily study + coding sessions _
