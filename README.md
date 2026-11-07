# Beyond Benefits: Is Workplace Mental Health Support Really Reaching Employees?

## Goal
Investigate the relation between the mental health benefits, knowledge about the available resources and the workers trust to talk about mental health at work.

## Main question

Are tech organisations doing enough to turn mental health support into a meaningful employee experience?

## Why it matters?
As seekers of the best working conditions possible and aspiring to begin a tech career, these findings may help understand what meaningful workplace support involves.


## Research Questions
******(Remark: we have to decide which questions to keep as not all of them can be answered by our data)

1. Does having mental health benefits means to know the available resources?
2. Does the employer offer resources to learn about mental health and how to seek help?
3. Have employees discussed their mental heslth with colleagues?
4. Being afraid of negative consequences is related with reducing or avoiding to seeking for treatment? / How does being afraid of negative consequences relate to a reduction or avoidance of seeking treatment?
5. What mental health topics are most publicly communicated by tech companies?
6. How do organisations communicate the different dimensions of support?
7. Do organisations communicate about the same issues that employees identify as important or challenging?
8. Does reporting the availability of mental health benefits also correspond to reporting the availability of educational and informational resources?
9. How do companies approach mental health?

## Hypothesis
1. Employees who report that their employer provides mental health benefits are more likely to know about available workplace mental health resources.
2. A significant proportion of employees do not know whether their employer provides mental health benefits.
3. Employees who discuss mental health with colleagues are more likely to discuss it with their employer.
4. The themes emphasised in companies' public mental health communications may differ from the concerns reported by employees.
5. Organisations highlight the availability of mental health resources more often than they communicate how employees can access them.

## Sources
- OSMI Mental Health in Tech Survey
- Official pages from tech companies

## Methodology 
Exploratory and descriptive analysis with Python, supplemented by web scraping.

## Integration plan and limitations:
Our data is investigating relations between variables, not causality, as the dataset focus on employee perceptions and self reported experiences. 
The web scraping is focused on themes related with the variables on the dataset. The companies webpages describe public organisational communication, not necessarily the internal policies employees receive.

- Organizational support
1. Healthcare and financial support
   - Dataset: benefits, medical_coverage
   - What organisations communicate about insurance, treatment coverage and access to professional care
2. Education and information
   - Dataset: workplace_resources
   - What organisations communicate about awareness, mental health education and where employees can seek help
3. Workplace dialogue
   - Dataset:mh_employer_discussion, mh_coworker_discussion
   - What organisations communicate about conversations with managers, colleagues and workplace culture

## Variables (original questions retrieved from the original survey)
Understanding what each column means

| Variable | Original Question | What it measures |
|---|---|---|
| benefits | Does your employer provide mental health benefits as part of healthcare coverage? | Perceived availability of benefits |
| workplace_resources | Does your employer offer resources to learn more about mental health disorders and options for seeking help? | Perceived availability of educational and informational resources|
| mh_employer_discussion | Have you ever discussed your mental health with your employer? | Previous disclosure/discussion |
| mh_coworker_discussion | Have you ever discussed your mental health with coworkers? | Previous disclosure/discussion with colleagues |
| medical_coverage | Do you have medical coverage that includes treatment of mental health disorders? | Personal access to medical coverage | 
| mental_health | Do you currently have a mental health disorder? | Self-reported current mental health status
| mh_share | How willing would you be to share with friends and family that you have a mental illness? | Willingness to disclose to personal contacts | 

