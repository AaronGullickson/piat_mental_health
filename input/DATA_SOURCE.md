---
editor: visual
---

# Data Source Description

The data we will use come from the 2021 [Youth Risk Behavior Surveillance System](https://www.cdc.gov/healthyyouth/data/yrbs/index.htm) (YRBS) data. The YRBS data is a set of surveys of high school students that track a variety of risk behaviors that can lead to poor health. We will use the nationally based survey (there are additional surveys conducted at the state and local level).

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.qmd quarto document. The name of the dataset in R is `yrbs`.

-   **mental_health**: Students were asked "Over the last 30 days, how often was your mental health not good?" They could respond on a five point scale from "Never" to "Always." We will treat this scale as a score from 1-5 where higher values indicate poorer mental health. This is the key dependent variable.
-   **screen_time**: The amount of hours that students report being on screens on an average day. The data is recorded as an ordinal variable that goes from "less than 1 hr/day" to "5 or more hrs/day." This is the key independent variable.
-   **age**: The age of the student in years.
-   **gender**: The gender of the student (only choices were male or female).
-   **race**: The reported race of the student in six categories.
-   **bully_electronic**: The student's yes/no response to a question about whether they have been electronically bullied (i.e. online) in the last 12 months.
-   **sleep**: The hours of sleep that the student gets on an average school night.
-   **physical_activity**: The number of days out of the past week that the student was physically active for at least one hour.
