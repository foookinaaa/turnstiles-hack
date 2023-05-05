# turnstiles-hack
**Task:**   
Who's there? Predict who entered the building by time and turnstile.
To get into the building, you need to go through the turnstile. To open the parking lot, you need to open the barrier. To get to the floor, you need to attach a “pill”. All this is fixed - who, on what date, at what time.
Will we be able to learn how each of the visitors to the office arrives, and predict? “8 am Monday, turnstile 4? Director." “11am Saturday? Grisha. But Grisha never comes on the last day of the month.” What are the patterns in real data?

**Data:**
- user_id: Target. User number.
- ts: Date and time of passage through the turnstile.
- gate_id: Number of the turnstile (barrier, entrance to the floor)

**Metric:**  
percentage of correct answers (accuracy * 100)
