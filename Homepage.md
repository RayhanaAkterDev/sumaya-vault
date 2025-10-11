---
Title: Homepage
---
# Homepage

_Welcome, Sumaya!_  
📅 [[2025-10-01|2025-10-01]]  

 `BUTTON[new_note]` 

```button
name Create Discovery Note
type note(My New Note, tab) template
action discovery_log
color purple
folder 19 Discovery Logs
```
^button-hkyn

 ```meta-bind-embed
 [[MetaBindEmbeds Spaces Buttons]]
 ```

---

**Calendar View:**

```dataview
CALENDAR date(file.name)
FROM "02 Journal/Daily_Notes"
```

---

## Goals & Progress

> [!multi-column]
> 
>> [!quote]+ ✨ Motto & Goals
>> - Academic Excellence [^1]
>> - Personal & Spiritual Growth [^2]
>> - Skill Development [^3]
>> - Work Ethic [^4]
>
>> [!abstract] Learning Progress
>> **Current**: Phase 2 – JavaScript Core Concepts 
>> - [[02 Coding Roadmap|See the full roadmap →]]
>> - [[03 Select Niche|See your niche roadmap]]

---

## Dataview Records

> [!blank]
> ```dataview
> 	table from "16 DataViews"
> 	where file.name != "16 DataViews"
>  ```

---

## Folder Notes

> [!note]+
> ```dataview
> list
> from "/"
> where length(split(file.folder, "/")) = 1
> and file.name = regexreplace(file.folder, ".*/", "")
> or file.folder = ""
> sort file.name asc
> ```

---

## Study Materials — _[[5th Semester|DIIT 5th Semester]]_

> [!blank]
> ```dataview
> 	table from "06 CSE DIIT/5th Semester"
> 	where contains(file.folder, file.name)
> 	  and length(split(file.folder, "/")) = length(split("06 CSE DIIT/5th Semester", "/")) + 1
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
