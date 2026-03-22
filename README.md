<<<<<<< HEAD
# DAT505_

#welcome to my repo




git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"

system2(git, c("config", "--local", "commit.gpgsign", "false"))

system2(git, c("config", "--local", "--unset", "gpg.program"))
system2(git, c("config", "--local", "--unset", "user.signingkey"))

system2(git, c("config", "--local", "--get", "commit.gpgsign"))

setwd("C:/Users/ADMIN/Desktop/DAT505")

system2(git, c("config", "--show-origin", "--get-all", "commit.gpgsign"))

system2(git, c("config", "--show-origin", "--get-all", "gpg.program"))
system2(git, c("config", "--show-origin", "--get-all", "user.signingkey"))
system2(git, c("config", "--show-origin", "--get-all", "commit.gpgsign", "--global"))

setwd("C:/Users/ADMIN/Desktop/DAT505")
git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"

system2(git, c("add", "-A"))

system2(git, c("commit", "--no-gpg-sign", "-m", "Update README / draft fixes"))

getwd()

setwd("C:/Users/ADMIN/Desktop/DAT505/DAT505_")
list.files(all.files = TRUE)

git <- "C:/Users/ADMIN/Desktop/DAT505/PortableGit/bin/git.exe"
system2(git, "status")

=======
# DAT505-2026
Course materials, datasets, and R scripts for DAT505 - Winter 2026


### Course description

The main objective of this course is to equip students with a comprehensive set of skills for conducting research in experimental psychology and the behavioral sciences. These skills extend beyond the acquisition of technical tools and are best understood as a way of thinking critically about data and scientific questions. On the technical side, the course develops proficiency in programming with R, as well as mastery of both basic and advanced statistical methods commonly used in behavioral research. However, equal emphasis is placed on non-technical competencies that are essential to sound data analysis. Students will learn how to formulate clear research questions, critically select methods, properly interpret statistical results, and communicate findings to both technical and non-technical audiences. To achieve these learning objectives, the course relies on a project-based pedagogy, through which students will produce two full research reports using real datasets from existing behavioral research.

### Learning outcomes

By the end of the semester, students will be able to:

*Programming and data management*

- Use R and RStudio at an advanced level for data cleaning, transformation and analysis.
Statistical methods
- Apply and interpret core statistical tools used in behavioral research, including hypothesis testing, linear and generalized linear models.

*Data visualization*

- Create informative data visualizations for exploratory analysis and communication of results.

*Analytical and research skills*

- Formulate research questions with clear, testable hypotheses.
- Operationalize theoretical constructs using appropriate measures.
- Select and justify analytical methods suited to the research question and data structure.
- Critically interpret statistical results.

*Communication and reporting*

- Communicate results effectively in oral presentations.
- Produce reproducible research reports using R Markdown and Quarto.
- (Optional) Develop interactive data visualizations and applications using Shiny.

*Workflow and collaboration*

- Use version control with Git and GitHub.

*Reproducible research and transparency*

- Write fully reproducible code.
- Understand and apply core open science practices, including pre-registration.


### Tools

* R/R Studio
* R packages (esp. tidyverse)
* Git/Github

### Weekly schedule

_Week 1: Getting started with R/R Studio_

* General course description (objectives, structure, evaluation)
* Presentation of R/RStudio, Quarto, Github, and open science practices
* Presentation of the report template
* Exercises
* (Optional tasks before the first class): Read Chapter 1 of From Questions to Knowledge: <https://bookdown.org/danielnettle2/data_analysis/building-blocks.html> Having installed the latest R and R Studio versions on computer: <https://cran.r-project.org/> and <https://posit.co/downloads/>

_Week 2: Variable types, descriptive statistics and data visualization_

* Class exercices
* Start of class projects
* Mandatory readings: Chapters 2.1-2.6 of Modern Statistics with R: <https://modernstatisticswithr.com/>
* Optional readings: Chapters 2.7-2.8 of Modern Statistics with R: <https://modernstatisticswithr.com/>

_Week 3: Intro to Git/Github workflow + Data transformation_

* Short lecture on Git/Github
* Class exercises
* Class projects 
* Mandatory readings: Sections 5 and 19 of R for data science: <https://r4ds.hadley.nz>

_Week 4: Class projects_

* This class is dedicated to personal work on the students' research reports, making sure that every students has settled on a research project.
* No mandatory readings

_Week 5: Introduction to the General Linear Model_

* Class exercises on the General Linear Model
* Class projects
* Mandatory readings:
    * Watch the following videos in order:
        * https://www.youtube.com/watch?v=7cSArk7tU4w
        * https://www.youtube.com/watch?v=wUT1qstylFQ
        * https://www.youtube.com/watch?v=IXYDMMBisr8
    * Read Sections 3 to 4.2 (included) of From Questions to Knowledge by Daniel Nettle: https://bookdown.org/danielnettle2/data_analysis/ (section 4.3 is optional)

_Week 6: Generalized linear models, mixed models and ANOVA_

* Class exercises on the generalized linear model and mixed models
* Class projects
* Mandatory readings:
    * Watch the following videos in order
        * On generalized linear models: Videos 1-6 from this playlist: https://youtube.com/playlist?list=PLblh5JKOoLUKxzEP5HA2d-Li7IJkHfXSe&si=wad7IsGlApLWXikD
        * On mixed models: https://www.youtube.com/watch?v=51SMnDN0ye0
    * Read Sections 6 and 7 of From Questions to Knowledge by Daniel Nettle: https://bookdown.org/danielnettle2/data_analysis/

**FEBRUARY 15: SUBMIT RESEARCH REPORT 1**

_Week 7: Model selection and sensitivity analysis_

* Class exercises on the generalized linear model and mixed models
* Class projects
* Mandatory readings: Sections 8 and 9 of From Questions to Knowledge by Daniel Nettle: https://bookdown.org/danielnettle2/data_analysis/

_Week 8: Class projects_

* This class is dedicated to personal work on the students' research reports, making sure that every students has settled on a research project.
* No mandatory readings

**_Week 9: Midterm_**

* Midterm exam (20%): Real-time, physical, open-book (with computers) project. 2 hours.

_Week 10: Content analysis for behavioral science (1)_

* Introduction to text analysis using tidytext
* Class projects
* Mandatory readings: Sections 1-9 of Text Mining with R https://www.tidytextmining.com/

_Week 11: Content analysis for behavioral science (2)_
* Introduction to text classification
* Class projects
* Mandatory readings:
    * The Augmented Social Scientist: https://journals.sagepub.com/eprint/QQGF4CWUMRDVYEQ8UVJ9/full

_Week 12: Intro to predictive modelling_

* TBD

_Week 13: Class projects_

* This class is dedicated to personal work on the students' research reports.
* Mandatory readings: Chapter 12 of From Question to Knowledge: <https://bookdown.org/danielnettle2/data_analysis/>

**APRIL 10: SUBMIT RESEARCH REPORT 2**

### Main references

* Modern statistics with R: <https://modernstatisticswithr.com/> 
* From Questions to Knowledge: Data Analysis for Psychology and Behavioural Science using R: <https://bookdown.org/danielnettle2/data_analysis/>



>>>>>>> 91dd4583b2b928ff919106a3cf4236372be46bdb
