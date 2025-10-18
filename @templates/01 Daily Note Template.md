---
title: Daily Note
class: journal
aliases:
  - daily_note
  - daily-review  
---

# <% moment(tp.file.title, "YYYY-MM-DD").format("ddd MMM DD YYYY") %>

> [!info]
> ##### 📅 Week No. [[@journal/@weekly-notes/<%moment(tp.file.title).format("gggg-[W]ww")%>|<%moment(tp.file.title).format("gggg-[W]ww")%>]]  
> [[ @journal/@daily-notes/<% moment(tp.file.title, "YYYY-MM-DD").subtract(1, "days").format("YYYY-MM-DD") %> | Yesterday ⏪ ]] | [[ @journal/@daily-notes/<% moment(tp.file.title, "YYYY-MM-DD").add(1, "days").format("YYYY-MM-DD") %> | ⏩ Next day ]]
> 
> `BUTTON[edit_daily_temp]`

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

---

## Daily Goals

_Define true outcome of the day:_

1. 

---

## Tasks Overview

> [!multi-column]
> 
>> [!todo]
>> #### 🧾 Today's Tasks List
>> ```todoist
>> name: "View tasks:"
>> filter: "<% moment(tp.file.title, "YYYY-MM-DD").format("YYYY-MM-DD") %>"
>> autorefresh: 30
>> sorting:
>>  - priorityAscending
>> groupBy: section
>> ```

---

> [!multi-column]
>
>> [!todo]
>> #### 📚 Study Overview
>> - 6th Semester Lab Exam
>> - 5th  Semester Retake
>> - current 7th Semester Courses
>> ##### Study notes 
>> - [[5th Semester]]
>> 	- [[01 Peripheral & Interfacing|Peripheral & Interfacing]]
>> 		- [[Chapter 1 - Interfacing Techniques]]
>> ---
>> ```todoist
>> name: "View study tasks:"
>> filter: "##Study & @study"
>> autorefresh: 30
>> sorting:
>>   - date
>>   - priority
>> groupBy: section
>> show: 
>>  - date
>>  - description
>> ```
>
>> [!todo]
>> #### 💻 Coding Tasks & Overview>> 
>> - **_Coding topics & status_** [^1]   
>> - **_[[@sandbox|Coding Notes]]_**
>> ---
>> ```todoist
>> name: "View coding tasks:"
>> filter: "##Code & @code"
>> autorefresh: 30
>> sorting:
>>  - date
>>  - priority
>> groupBy: section
>> show: 
>>  - date
>>  - description
>> ```

---

> [!multi-column]
> 
>> [!note]
>> #### 📌 Notes & Reminders
>> - For _persona verification_ need to wait 48 hours to 5 days to recover _LinkedIn_ id properly.
>> - _7 day skin care routine_ [^2]   
>> - _7 day hair care routine_ [^3]   

---

##  Daily Review

- 🌟 Highlight of the Day  
- ⚡ Challenges Encountered  
- 📌 Key Takeaways / Lessons Learned  

See all your daily reflections and progress — [[@daily-reviews|👉 click here]]

[^1]: ###### _Coding Topics & Status_
	
	- `tailwind`— ongoing 
	- `javascript`
	- `react`
	- `laravel`
	- `database`
	- `projects`
	- `frontend`
	- `backend`

[^2]: ##### 7 Day Skin Care:
	
	1.  **Saturday – Brightening & Tan Removal** 
		- besan + orange peel powder + turmeric + lemon juice (yogurt optional)
	2. **Sunday – Skip Day**    
	3. **Monday – Soothing & Repair** 
		- cucumber/potato juice + beetroot powder + oatmeal
	4. **Tuesday – Skip Day**    
	5. **Wednesday – Exfoliation + Healing** 
		- **Step1**: oatmeal scrub
		- **Step2**: besan + multani mitti + turmeric + yogurt + tomato/potato juice
	6. **Thursday – Skip Day**    
	7. **Friday – Anti-Aging & Glow** 
		- beetroot powder + besan + honey/yogurt/milk

[^3E]: ##### 7 Day Hair Care:
			
	1. **Saturday – Protein & Shine Pack**    
		  - whole egg + yogurt + fenugreek paste/powder (soaked overnight), wash with mild shampoo        
	2. **Sunday – Oiling / Light Nourishment**    
		  - rosemary oil (warm slightly), massage 10 mins, leave 1–2 hrs or overnight        
	3. **Monday – Skip / Rest Day**    
	4. **Tuesday – Herbal Growth Pack**    
		  - curry leaf powder + hibiscus leaves/henna + beetroot powder, mix with yogurt or water, wash with mild shampoo 
	5. **Wednesday – Skip / Rest Day**    
	6. **Thursday – Growth Booster Pack**    
		  - flaxseed gel + onion juice, rinse with plain water (no shampoo)        
	7. **Friday – Oiling / Light Nourishment**    
		  - rosemary oil (warm slightly), massage 10 mins, leave 1–2 hrs or overnight

