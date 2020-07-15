# FREECAUSE
mpacts and Grades
DeepScan calculates a project's overall grade by the issues detected and their impacts. This is then represented as a grade which is "Poor", "Normal", and "Good".

Impacts
By its severity, each rule has impacts as the following.

High	High impact alarms cause immediate problems.
When the code is executed, an exception is thrown and the execution is interrupted immediately.
Medium	Medium impact alarms are detected when the code will not run as expected.
These alarms do not cause immediate problems.
However, later in the execution, it is likely that the code will not behave as intended in various ways.
Low	Low impact alarms cause code quality and maintenance issues although not directly related to problematic execution.
These alarms include commonly known pitfalls that should be avoided when possible.
Grade Rating
Below Rating means the number of issues per thousand lines of code ("issue density").

For example, 10 high and medium-impact issues in a 10,000 lines of code would be issue density 1.

Lines of code includes only the user code base where issues are counted.
Each empirical threshold for issue density was derived from our benchmark for 150 GitHub open source projects.
Grade	Rating	Remarks
Good
High and medium-impact issue density <= 0.3
and
Low-impact issue density <= 1.5

Rated 30% of the 150 GitHub projects as Good
Normal
When one of the following conditions is met:

0.3 < High and medium-impact issue density <= 0.7
High and medium-impact issue density <= 0.3
and
Low-impact issue density > 1.5
Rated 40% of the 150 GitHub projects as Normal
Poor
High and medium-impact issue density > 0.7

Rated 30% of the 150 GitHub projects as Poor
N/A
Not rated.

It might be the case that there are no files to analyze or analysis becomes failed.
[![DeepScan grade](https://deepscan.io/api/teams/10093/projects/12875/branches/205851/badge/grade.svg)](https://deepscan.io/dashboard#view=project&tid=10093&pid=12875&bid=205851)
<a href="https://deepscan.io/dashboard#view=project&tid=10093&pid=12875&bid=205851"><img src="https://deepscan.io/api/teams/10093/projects/12875/branches/205851/badge/grade.svg" alt="DeepScan grade"></a>
