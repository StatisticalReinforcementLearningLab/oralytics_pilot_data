# Naming Convention For Oralytics Pilot Data CSV

This document explains the column names in the pilot data csv file.

* `user_id`: unique user id given to user in the form of `robas+{}@developers.pg.com`.
* `user_decision_t`: unique user decision time index [0, 139]
* `decision_time`: unique datetime (i.e., '%Y-%m-%d %H:%M:%S') for when the action was executed
* `schedule_id`: id of the schedule that this action came from
* `action`: \{0, 1\} where 1 denotes a message being sent and 0 denotes a message not being sent
* `prob`: action selection probability
* `quality`: brushing quality truncated at 180 seconds (outcome)
The following columns are flattened state (context) vector observed by the algorithm at decision time
* `state_tod`: time of day, 0 for morning, 1 for evening
* `state_b_bar`: exponential average of quality over past 7 days (normalized) (See [pilot code](https://github.com/StatisticalReinforcementLearningLab/Oralytics-RL-Service/blob/v0.pilot/reward_definition.py) for exact computation of b_bar)
* `state_a_bar`: exponential average of engagement prompts (action == 1) over past 7 days (normalized) (See [pilot code](https://github.com/StatisticalReinforcementLearningLab/Oralytics-RL-Service/blob/v0.pilot/reward_definition.py) for exact computation of a_bar)
* `state_app_engage`: prior day app engagement (i.e., if the participant has the app open and in focus / not in background), 1 if yes, 0 if no
* `state_day_type`: weekday or weekend, 0 for weekday, 1 for weekend
* `state_bias`: intercept term, always 1
* `state_day_in_study`: participant day in study normalized between [-1, 1] for a 70-day study. (Note: each participant was in the pilot study for 35 days, but this feature is normalized for a 70-day study because each participant is in the main phase of Oralytics for 70 days. 

