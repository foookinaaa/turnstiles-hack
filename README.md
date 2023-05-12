# turnstiles-hack
**Task:**   
Who's there? Predict who entered the building by time and turnstile.
To get into the building, you need to go through the turnstile. To open the parking lot, you need to open the barrier. To get to the floor, you need to attach a “pill”. All this is fixed - who, on what date, at what time.
Will we be able to learn how each of the visitors to the office arrives, and predict? “8 am Monday, turnstile 4? Director." “11am Saturday? Grisha. But Grisha never comes on the last day of the month.” What are the patterns in real data?
<img width="1050" alt="Screenshot 2023-05-12 at 12 08 58" src="https://github.com/foookinaaa/turnstiles-hack/assets/74900958/c8bd5852-9ac4-4a71-9760-1b04db9d5249">

**Data:**
- user_id: Target. User number. (57 unique users)
- ts: Date and time of passage through the turnstile   
train: [2022-07-29 - 2022-12-31]  
test: [2023-01-03 - 2023-02-24]
- gate_id: Number of the turnstile (barrier, entrance to the floor) (16 unique gates)

**Metric:**  
percentage of correct answers (accuracy * 100)
baseline public score: 0.1285794497
logreg public score: 0.1779898933
xgboost public score: 0.2810218978

**Decision:**
1) eda - look at the data and find some patterns or obvious answers
2) log_reg - thinking a lot of features (mostly binary) + add features from public notebook and put it to scaller + simple logistic regression
3) xgboost - take all features from log_reg, add smth more and put it to scaller + xgboost

**Competition page:**
https://ods.ai/tracks/linear-models-spring23/competitions/gates/leaderboard
