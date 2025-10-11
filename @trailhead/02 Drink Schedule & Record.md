## 🥤 Daily Drink Schedule

| **Morning (empty stomach)**            | **Afternoon (30–40 min after lunch)**        | **Night (before bed)**      |
| -------------------------------------- | -------------------------------------------- | --------------------------- |
| Fenugreek + Jeera water                | Beetroot juice / Turmeric tea / Lemon water  | Cinnamon tea / Senna tea    |

_Timeline review:_

- **Morning (Fenugreek + Jeera water)** 
	- On empty stomach
- **Afternoon (Beetroot juice / Turmeric tea / Lemon water)**    
    - **Beetroot juice** → 2× week        
    - **Turmeric tea** → 2× week        
    - **Lemon water** → 3× week        
        
- **Night (Cinnamon tea / Senna tea)**    
    - **Cinnamon tea** → 5× week                
    - **Senna tea** → 2× week (in beetroot days)

---

## Drink Record

```dataview
table water_intake as "Water", dinner_by_8 as "Dinner at 8", drink_record as "Drink Record"
from "02 Journal/Daily_Notes"
where contains(aliases, "drink_record")
sort file.day desc
```