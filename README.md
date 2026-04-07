# cursor_trajectories
Time-resolved analysis of cursor trajectory data in a visual search task. Implements feature extraction and random forest models to predict errors, target presence, response type, and accuracy across multiple classification frameworks.


## Directory Structure

```
ts-ls-cursor-analysis/
├── Ts and Ls - S2_4-class_Prediction.ipynb
├── Ts and Ls - S2_ErrorVsCorrect.ipynb
├── Ts and Ls - S2_PresentVsAbsent.ipynb
├── Ts and Ls - S2_ResponseType.ipynb
├── Ts and Ls - S2_Target-Absent.ipynb
├── Ts and Ls - S2_Target-Present.ipynb
└── README.md
```

## Shared Pipeline
**All notebooks follow the same general pipeline:**
- Time-resolved decoding across response-locked bins
- Participant-level train/test split (70/30)
- Downsampling to balance classes
- Random forest classification across time bins
- Evaluation using accuracy and class-specific metrics
- Feature importance tracked across time



**Notebooks**

`S2_4-class_Prediction.ipynb`
- Multiclass classification: Hit, Miss, Correct Rejection, False Alarm
- Evaluates both overall accuracy and combined error accuracy


`S2_ErrorVsCorrect.ipynb`
- Binary classification: Correct vs Error
- Focuses on detecting errors from cursor behavior


`S2_PresentVsAbsent.ipynb`
- Binary classification: Target Present vs Absent
- Tests whether cursor dynamics reflect target presence


`S2_ResponseType.ipynb`
- Binary classification: Mouse click vs Spacebar response
- Examines differences in motor execution strategies
  

`S2_Target-Absent.ipynb`
- Binary classification: Correct Rejection vs False Alarm
- Focuses on decision-making when no target is present


`S2_Target-Present.ipynb`
- Binary classification: Hit vs Miss
- Focuses on failures to detect present targets

---

## Contact Information

For any questions regarding this project, please contact:

**Name:** Sarah Malykke  
**Email:** sarahmalykke@gwu.edu 
  
