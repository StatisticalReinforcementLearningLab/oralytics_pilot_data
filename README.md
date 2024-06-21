# Oralytics-Pilot-Data
Data from the pilot (phase 1) of the [Oralytics clinical trial](https://clinicaltrials.gov/study/NCT05624489). A total of 9 users participated in the pilot for a minimum of 35 days (or 70 decision points). The RL algorithm in Oralytics optimized the delivery of engagement prompts to participants at risk for dental disease to maximize their brushing quality (or oral self-care behaviors). This data was collected and maintained by the RL service for the RL algorithm. For more information about Oralytics, please see the following papers:
* [Designing Reinforcemnt Learning Algorithms for Digital Interventions: Pre-Implementation Guidelines](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=mAgilOsAAAAJ&citation_for_view=mAgilOsAAAAJ:u-x6o8ySG0sC)
* [Reward Design For An Online Reinforcement Learning Algorithm Supporting Oral Self-Care](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=mAgilOsAAAAJ&citation_for_view=mAgilOsAAAAJ:d1gkVwhDpl0C)
* [Oralytics Phase 1 Protocol Paper](https://www.sciencedirect.com/science/article/abs/pii/S1551714424000387)

Data is in [oralytics_pilot_data.csv](https://github.com/StatisticalReinforcementLearningLab/oralytics_pilot_data/blob/main/oralytics_pilot_data.csv).
Data with feature engineering (two additional features of `state_day_type` and `state_day_in_study` that were not used in the algorithm but could be helpful for building simulation environments) is in [pilot_data_with_feature_engineering.csv](https://github.com/StatisticalReinforcementLearningLab/oralytics_pilot_data/blob/main/pilot_data_with_feature_engineering.csv). 
Naming convention for column names is in [naming_convention.md](https://github.com/StatisticalReinforcementLearningLab/oralytics_pilot_data/blob/main/naming_convention.md)

## Citing Our Data
If you use our data in any way, please cite us:
```
@article{nahum2024optimizing,
  title={Optimizing an adaptive digital oral health intervention for promoting oral self-care behaviors: Micro-randomized trial protocol},
  author={Nahum-Shani, Inbal and Greer, Zara M and Trella, Anna L and Zhang, Kelly W and Carpenter, Stephanie M and Ruenger, Dennis and Elashoff, David and Murphy, Susan A and Shetty, Vivek},
  journal={Contemporary Clinical Trials},
  volume={139},
  pages={107464},
  year={2024},
  publisher={Elsevier}
}
```

```
@misc{trella2024oralytics,
      title={Oralytics Reinforcement Learning Algorithm}, 
      author={Anna L. Trella and Kelly W. Zhang and Stephanie M. Carpenter and David Elashoff and Zara M. Greer and Inbal Nahum-Shani and Dennis Ruenger and Vivek Shetty and Susan A. Murphy},
      year={2024},
      eprint={2406.13127},
      archivePrefix={arXiv},
      primaryClass={id='cs.AI' full_name='Artificial Intelligence' is_active=True alt_name=None in_archive='cs' is_general=False description='Covers all areas of AI except Vision, Robotics, Machine Learning, Multiagent Systems, and Computation and Language (Natural Language Processing), which have separate subject areas. In particular, includes Expert Systems, Theorem Proving (although this may overlap with Logic in Computer Science), Knowledge Representation, Planning, and Uncertainty in AI. Roughly includes material in ACM Subject Classes I.2.0, I.2.1, I.2.3, I.2.4, I.2.8, and I.2.11.'}
}
```
