# Question 1

OptionA - Modify the Instructor dimension by adding special rows representing instructor teams.Forexample,CS276ais taught by
Manning and Raghavan, so there will be an Instructor row representing “Manning/Raghavan” (as well as separate
rows for Manning and Raghavan, assuming that they sometimes teach courses as sole instructors). In this way, the
Instructor dimension becomes true to the grain and we can include it in the fact table.

The reason to use this will be it is easy to make change in the static(dimension) tables jusy by adding more granularity, which might not be 
the case if we make changes in the fact table.
