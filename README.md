# Healthcare-Appointment-No-show-Analysis-**[Project : healthcare](https://github.com/nafiya1236/Healthcare-Appointment-No-show-Analysis-?tab=readme-ov-file)**
Healthcare Appointment No-show Analysis Report

IntroductionMissed medical appointments, or no-shows, can significantly impact healthcare service efficiency and patient outcomes. This project analyzes a dataset containing historical appointment data to uncover patterns that contribute to patient no-shows. The aim is to provide actionable insights for reducing no-show rates using a combination of data cleaning in Python and interactive data visualization in Power BI.

Data Source and PreparationThe dataset used for this analysis was sourced in CSV format and contained information about patient demographics, appointment details, and attendance status. The data was first imported into a Jupyter Notebook using Python.

In Python, we conducted several data cleaning steps:

Renamed inconsistent column names for readability.

Converted date columns like ScheduledDay and AppointmentDay into datetime format.

Removed duplicate entries to ensure unique appointment records.

Handled invalid or suspicious values, such as negative ages.

Created new calculated columns including WaitDays (the difference between scheduling and appointment dates) and Weekday (day of the week the appointment occurred).

These cleaning steps ensured the data was consistent, accurate, and ready for analysis. The final cleaned dataset was exported as a CSV file and imported into Power BI for visualization.

Power BI Analysis and VisualizationsOnce loaded into Power BI, several calculated columns and DAX measures were created to facilitate deep analysis. Key measures included:

Total Appointments

Total No-shows

No-show Rate (%)

SMS Sent %

Average Age

Average Wait Days

Key calculated columns included:

ShowStatus (categorizing as "Showed up" or "No-show")

Weekday (from AppointmentDay)

AgeGroup (Child, Young Adult, Adult, Senior)

Multiple visuals were used to explore trends:

Bar Charts showing no-show distribution by SMS reminders, gender, and weekday.

Line Charts displaying no-show rates by age and wait days.

Heatmaps and Matrix Visuals to observe intersections like SMS received vs weekday.

Cards summarizing overall KPIs such as total appointments, no-show percentage, and SMS effectiveness.

Pie and Donut Charts giving a snapshot of attendance distribution.

Insights and ConclusionThe analysis revealed clear patterns. Patients who did not receive SMS reminders were more likely to miss appointments. Younger age groups and appointments scheduled with longer wait times also had higher no-show rates. No-shows were most frequent on specific weekdays, suggesting operational inefficiencies.

This end-to-end approach, starting from Python-based data cleaning to Power BI-driven insights, enabled a comprehensive understanding of no-show behavior. These insights can be used by healthcare providers to implement reminder systems, reschedule high-risk slots, and prioritize follow-ups, ultimately improving patient care and clinic performance.
