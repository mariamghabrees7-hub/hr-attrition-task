# HR Employee Attrition: Key Insights & Recommendations

## Data quality summary
- 1,470 employee records, zero missing values, zero duplicates.
- Three columns carried no information and were dropped: `EmployeeCount` (always 1), `Over18` (always "Y"), `StandardHours` (always 80).
- `PerformanceRating` only contains the values 3 and 4 in this dataset; ratings 1 and 2 never appear. This looks like a data collection quirk rather than an error, but it means "performance" can't really be analyzed on a full scale, only as a two-tier split.
- Added readable labels for the four 1-4 satisfaction scales (Job Satisfaction, Environment, Relationship, Work-Life Balance) alongside the original numeric codes.
- Overall attrition rate: 16.1% (237 of 1,470 employees).

## Department and job role
- Sales has the highest departmental attrition at 21.0%, followed by HR at 19.0% and R&D at 14.0%.
- The real story is at the role level: **Sales Representatives leave at 40%**, more than double any other role, while also earning the lowest average income ($2,626/month) of any role in the dataset.
- Managers and Research Directors, the highest-paid and most senior roles, have the lowest attrition (5% and 2%).

## Salary, experience, and performance
- Income rises consistently with job level, from $2,787/month at Level 1 to $19,192/month at Level 5, and correlates strongly with total working years (0.77).
- Salary hikes do track performance rating: employees rated 4 got an average 21.8% hike versus 14.0% for those rated 3. Pay increases are behaving as intended, this is not a broken process.

## Satisfaction
- All four satisfaction measures average close to the midpoint (around 2.7 out of 4), with no single dimension standing out as unusually low company-wide.
- Attrition drops steadily as satisfaction rises on every dimension. The steepest drop is in Environment Satisfaction: 25.4% attrition at the lowest level versus 13.5% at the highest.

## Attrition drivers, the core finding
- **Overtime is the strongest single driver in the data.** Employees working overtime leave at 30.5%, versus 10.4% for those who don't, nearly a 3x difference.
- The effect compounds with work-life balance: employees who work overtime **and** rate their work-life balance as "Bad" leave at 45.5%, the highest attrition segment in the entire dataset.
- Single employees leave at 25.5%, well above married (12.5%) or divorced (10.1%) employees.
- Frequent travelers leave at 24.9%, versus 8.0% for those who don't travel.
- Having any stock options at all sharply reduces attrition: 24.4% with none, dropping to 7.6% at the middle stock option level.

## Recommendations
1. **Investigate overtime load in Sales, especially the Sales Representative role.** This is where the two biggest risk factors (overtime and low pay) overlap, and it shows in the numbers: 40% attrition.
2. **Extend stock option eligibility further down the org**, since employees with zero stock options are 3x more likely to leave than those with even one level of options.
3. **Treat "overtime + poor work-life balance" as a specific at-risk segment**, not just two separate metrics. Nearly half of employees in that combined group leave.
4. **Review compensation at the Sales Representative and Laboratory Technician levels**, both combine low pay with above-average attrition.
