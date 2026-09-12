# HealthConnect_Clinic_Week6

## Project Overview

HealthConnect Clinic is a healthcare appointment management project focused on understanding and reducing missed appointments while improving the patient support experience.

In Week 6, the Data Analytics track extended the Week 5 analysis by investigating factors associated with appointment no-shows, identifying higher-risk appointment segments, improving the Power BI dashboard, and preparing analytical findings for collaboration with the Data Science track.

The analysis moved beyond individual variables to examine combinations of factors, particularly booking lead time and previous no-show history.

## Business Question

How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?

Week 6 focused on:

* Identifying factors associated with appointment no-shows
  
* Finding higher-risk appointment segments
  
* Validating and strengthening Week 5 findings
  
* Translating findings into practical recommendations
  
* Improving the existing Power BI dashboard
  
* Providing evidence and potential variables for predictive modelling

## Dataset

The analysis used a HealthConnect Clinic appointment dataset containing **5,000 appointment records**.

Key variables investigated included:
  
* booking lead time × reminder status;

*	previous no-show history × reminder status;

*	booking lead time × previous no-show history;

*	waiting time;

*	distance; and

*	age.

The Week 6 analysis continued from the validated Week 5 dataset and did not repeat the complete Week 5 exploratory analysis.

## Tools Used

* Python
  
* Pandas
  
* NumPy
  
* Jupyter Notebook
  
* Power BI
  
## Week 6 Analysis

### 1. Booking Lead Time

No-show rates increased as the time between booking and appointment became longer.

This strengthened the Week 5 finding that appointments booked further in advance may require additional attendance-support measures.

### 2. Previous No-Show History

Patients with previous no-show history showed higher current no-show rates.

This suggested that previous attendance behaviour could be useful when identifying appointments that may require additional follow-up.

### 3. Booking Lead Time × Previous No-Show History

The interaction between booking lead time and previous no-show history produced the most important segmentation finding.

The 46–60 day booking lead-time group with 2+ previous no-shows recorded an 82.11% no-show rate.

This combination was therefore treated as a high-value segment for further investigation and potential targeted attendance support.

### 4. Reminder Status

Reminder groups generally recorded lower no-show rates than corresponding groups without reminders.

However, this was treated as an observed association rather than proof that reminders directly cause lower no-show rates.

### 5. Distance to Clinic

No-show rates increased from 46.45% among patients travelling 0–5 km to 57.76% among patients travelling 20+ km.

Distance was therefore treated as a supporting factor rather than the primary risk indicator.

### 6. Waiting Time

Waiting time did not show a strong or consistent relationship with no-show behaviour.

The 60+ minute group recorded a high no-show rate, but it contained only three appointments. Therefore, it was not used as a major conclusion.

### 7. Age Group

Differences in no-show rates across age groups were relatively modest.

Age was therefore retained as a supporting variable rather than a primary risk factor.

## Key Findings

The major findings from Week 6 were:

* Longer booking lead time was associated with higher no-show rates.
  
* Previous no-show history was associated with higher current no-show rates.
  
* The combination of long booking lead time and previous no-show history identified substantially higher-risk segments.
  
* The 46–60 day and 2+ previous no-show segment recorded an 82.11% no-show rate.
  
* Reminder groups generally recorded lower no-show rates.
  
* Patients travelling 20+ km had a 57.76% no-show rate.
  
* Waiting time showed weak and inconsistent patterns.
  
* Age differences were relatively small and were therefore treated as a supporting finding.

Overall, Week 6 strengthened the main Week 5 conclusions while providing more detailed segmentation.

## Dashboard Improvements

The Week 6 findings were used to improve the existing Power BI dashboard.

The dashboard focus was shifted from reporting only overall no-show performance toward identifying actionable risk segments.

The improved analysis and dashboard placed greater emphasis on:

* Booking lead-time groups
  
* Previous no-show history
  
* Booking lead time × previous no-show segments
  
* Reminder status
  
* Distance-to-clinic groups

The 60+ minute waiting-time category was not highlighted as a major risk segment because it contained only three appointments.

## Recommendations

Based on the Week 6 analysis, the project recommends:

* Prioritising appointments with long booking lead times for additional attendance support.
  
* Identifying patients with previous no-show history for targeted follow-up.
  
* Combining booking lead time and previous no-show history when identifying higher-risk appointments.
  
* Maintaining effective reminder coverage, particularly for appointments with other identified risk factors.
  
* Considering additional attendance-support measures for patients travelling longer distances.
  
* Treating age as a supporting variable rather than a primary risk indicator.
  
* Not prioritising waiting time as a major intervention based on the current evidence.

These recommendations reflect observed associations and should be validated through further monitoring before being implemented as definitive operational policies.

## Data Science Collaboration

A major part of Week 6 was cross-track collaboration with the Data Science team.

The Data Analytics track shared findings relating to:

* booking lead time × reminder status;

*	previous no-show history × reminder status;

*	booking lead time × previous no-show history;

*	waiting time;

*	distance; and

*	age.
 
Potential modelling variables communicated included:

* booking_lead_days
* previous_no_shows
* reminder_sent
* distance_to_clinic_km
* appointment_type
* age_group

The interaction between booking lead time and previous no-show history was also highlighted because it produced substantially different risk segments.

These variables were communicated as potential modelling inputs, not confirmed predictive features. 

### Cross-Track Evidence Chain

The collaboration followed this process:

Data Analytics findings → Data Science comparison → validated priorities → refined decision support

This created an analytical bridge between descriptive analysis and predictive modelling.

## Limitations

The Week 6 analysis has several limitations:

* The analysis was primarily descriptive and segment-based.
  
* Formal statistical significance testing was not performed.
  
* The analysis does not establish causation.
  
* Some subgroups had small sample sizes.
  
* The dataset contains 5,000 records and represents a fictional HealthConnect Clinic scenario.
  
* The independent predictive strength of the identified variables has not yet been established.
  
* External generalisation has not been tested.
  
* Data Analytics and Data Science used different denominator definitions for some no-show calculations because Data Science excluded cancellations.

Therefore, the findings should be treated as evidence for further investigation rather than proof that a particular variable directly causes a patient to miss an appointment.

## Week 6 Outcome

Week 6 strengthened the HealthConnect Clinic project by moving the analysis from mainly individual-variable relationships toward combined-variable and segment-level analysis.

The most important analytical outcome was the identification of the 46–60 day booking lead-time and 2+ previous no-show segment, which recorded an 82.11% no-show rate.

The work also created an evidence-based foundation for predictive modelling and helped translate analytical findings into potential attendance-support interventions.

## Next Steps

The next phase of the project should focus on:

* Supporting predictive model development
  
* Validating selected features
  
* Evaluating model performance
  
* Further testing the lead-time × previous-no-show interaction
  
* Validating high-risk segments
  
* Testing the practical value of reminder interventions
  
* Integrating predictive insights into the Power BI dashboard
  
* Refining recommendations
  
* Conducting final data, dashboard and model consistency checks

## Conclusion

The Week 6 analysis provided deeper evidence about appointment no-show behaviour and identified higher-risk appointment segments that can support more targeted attendance interventions.

The strongest evidence came from the interaction between booking lead time and previous no-show history, while reminder status and distance provided additional supporting insights.

The project is now positioned to move from descriptive and diagnostic analytics toward predictive decision support, subject to further modelling, validation and responsible implementation.
