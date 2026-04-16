# DAX Measures - Student Success Dashboard

In order to generate the charts showing the analysis on average attendance and GPA, we first had to calculate the average attendance rate and average GPA from the attendance and GPA data columns.

```dax
Average Attendance Rate = AVERAGE(student_performance_data[AttendanceRate])
```

```dax
Average GPA = AVERAGE(student_performance_data[GPA])
```
