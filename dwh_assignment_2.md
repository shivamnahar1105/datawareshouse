# Scenario 1

# Question 1. What are the strengths and weaknesses of each option?

# OptionA
Strengths: This option allows the Instructor dimension to be included in the fact table, which will enable users to easily query the data for information about speciﬁc instructors. It also allows the grain of the fact table to remain at one row per student per course, which will make it easy to aggregate data for analysis.

Weaknesses: This option requires the creation of special rows in the Instructor dimension to represent instructor teams, which could make the dimension more complex and potentially harder to understand and use. Additionally, this option may not accurately represent the actual enrollment of each instructor, as the enrollment will be split equally among the instructors in a team.

# Option B:

Strengths: This option allows for the inclusion of the Instructor dimension in the fact table and enables accurate representation of enrollments for each instructor. It also
allows for the possibility of querying data at the student-course-instructor grain, which may be useful for some analysis.

Weaknesses: This option requires changing the grain of the fact table to one row per student per course per instructor, which may make it more diﬃcult to aggregate data for analysis at higher levels. It also requires the use of fractional values in the
EnrollmentCount ﬁeld, which may be confusing for users.

# Option C:
Strengths: This option allows for the creation of two separate fact tables, one for
general enrollment data and one for data at the student-course-instructor grain. This allows users to choose the appropriate fact table for their speciﬁc analysis needs and ensures that the data is accurately represented in each table.

Weaknesses: This option requires the creation and maintenance of two separate fact tables, which may increase complexity and the burden on the warehouse. It may also require users to remember to use the appropriate fact table for their queries, which could lead to errors or incorrect results if they use the wrong table.

Given the options presented, I would choose Option C. This option allows for the
creation of two separate fact tables, one with the Instructor dimension and one without, which enables users to choose the appropriate table for their analysis needs. This
