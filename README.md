# Beyond Benefits: Is Workplace Mental Health Support Really Reaching Employees?

## Goal
Investigate the relation between the mental health benefits, knowledge about the available resources and the workers trust to talk about mental health at work.

## Main question
Are employees aware of the mental health support their employees provide?

## Why it matters?
As seekers of the best working conditions possible and aspiring to begin a tech career, these findings may help understand what meaningful workplace support involves.
For companies, it is also important to understand if the investment they make in mental health benefits and resources effectively reaches the employees.

We expect to identify opportunities for organisations to make mental health support more visible and accessible.

## Hypothesis
1. Employees who report mental healh benefits are also more likely to report available menthal health resources.
2. A significant proportion of employees do not know whether their employer provides mental health benefits.
3. Employees who have discussed mental health with colleagues are more likely to have discussed it with their employer.
4. Organisations highlight the availability of mental health resources more often than they communicate how employees can access them.

## Sources
- OSMI Mental Health in Tech Survey
- Official pages from tech companies

## Methodology 
Exploratory and descriptive analysis with Python, supplemented by web scraping.

## Integration plan and limitations:
Our data is investigating relations between variables, not causality, as the dataset focus on employee perceptions and self reported experiences. 
The web scraping is focused on themes related with the variables on the dataset. The companies webpages describe public organisational communication, not necessarily the internal policies employees receive. Only the communication patterns.
Since the survey dataset has no company column, we could not make a direct comparision between the two data sources. 

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


## EMPLOYEE SURVEY: The Employee Perspective

Mental health benefits: Most respondents reported having mental health benefits at work (62.40%). However, 25.47% were unsure whether these benefits were available, while 12.12% reported having no benefits.

Workplace resources: The most common response was “No” (39.60%), indicating that many respondents did not believe their workplace provided mental health resources. 32.04% responded “Yes,” and 28.36% were unsure.

Discussion with employers: Most respondents reported that they did not discuss mental health with their employer (63.85%), compared with 36.15% who did.
Discussion with coworkers: Responses were more evenly divided. 51.84% did not discuss mental health with coworkers, while 48.16% did.

Medical coverage: A large majority of respondents reported having medical coverage (91.55%), while 8.45% did not.

Mental health status or experience: 43.60% selected “Yes,” 28.81% selected “No,” 20.24% selected “Possibly,” and 7.34% selected “Don’t Know.” This suggests that although “Yes” was the most common response, a substantial proportion of respondents were uncertain or did not identify with the condition represented by this variable.
Percentages may not total exactly 100% because of rounding.


Cross-tabulations: 
Benefits x Workplace Resources
Comparision between workplace resource availability across employees with and without benefits.
This analysis suggests a positive association between employer-provided benefits and access to workplace resources. Employees who report receiving benefits are substantially more likely to report that their employer provides access resources, while employees without benefits are much more likely to report that such resources are unavailable. The relatively high “I don’t know” responses also suggest that communication or employee awareness may be an important factor.
Among employees who were unsure whether their employer provided benefits, 43.23% were also unsure whether workplace resources were available. Additionally, 24.78% of employees who reported that their employer provided benefits still did not know whether workplace resources were available. This indicates that awareness of benefits and awareness of related workplace resources may not always align.

Benefits x Mental Health
Access to benefits vs Having a mental health condition: among the employees who are sure that teh company provides mental health benefits ("Yes"), about 50.7% report having a mental health condition.
No benefits: For the respondents who reported their company does not provide mental health benefits ("No"), 43.8% declares having a mental health condition, a high rate, as well.
"I don't know": Among the respondents that do not know if the company provides mental health benefits, the larger group is the one that stated not having a mental health condition.
The results suggest that having mental health benefits is significantly related with the group of people that clearly report having mental health conditions.

Workplace Resources × Mental Health
Key findings
Finding 1. Respondents reporting available resources also report the highest proportion of mental health conditions.
- Yes, resources available: 49.7% report a mental health condition.
- No, resources available: 44.4%.
- Don't know: 35.7%.


Finding 2. Respondents who report having no mental health condition are more represented in the group that reports available resources.
- Resources: Yes = 29.5%.
- Resources: No = 24.2%.
- Resources: Don't know = 34.5%.
The highest percentage is among respondents who don't know whether resources are available.

Finding 3. The percentage answering "Possibly" is relatively similar across the groups.
- Resources: Yes = 16.7%.
- Resources: No = 22.2%.
- Resources: Don't know = 21.6%.
This category represents respondents who are uncertain about their mental health status,  this is not a confirmed condition.
These findings suggest that making the workplace mental health resources more visible and easy to access is important.

Employer Discussion x Coworker Discussion
Among respondents in the “coworker discussion: No” category, 68.8% also reported that they did not discuss mental health with their employer. This suggests that most respondents who do not discuss mental health with their coworkers also avoid discussing it with their employer.

In contrast, among respondents who reported discussing mental health with their coworkers, 78.15% also reported discussing it with their employer.

These results suggest that, in workplaces where employees discuss mental health with their coworkers, they may also be more likely to discuss it with their employer. However, this indicates an association rather than a causal relationship. 


## WEBSITE ANALYSIS: The Organisational Perspective
Investigating how organisations communicate the different dimensions of support

Websites scraped:
"GitLab": "https://handbook.gitlab.com/handbook/total-rewards/benefits/",
"Apple": "https://www.apple.com/careers/uk/life-at-apple/benefits.html",
"Salesforce": "https://www.salesforce.com/blog/complete-guide-salesforce-benefits/"

Keyword analysis
Professional support was the most frequently reported category across all three companies, particularly for Salesforce, with 18 responses, followed by GitLab with 12 and Apple with 4. Salesforce also had the highest number of responses for mental health and emotional support, with 10 and 6 responses respectively.

Medical support was reported relatively consistently across the companies, with 4 to 6 responses. Work-life balance appeared less frequently, with 0 responses for Apple and 2 responses each for GitLab and Salesforce. No emotional-support responses were recorded for Apple or GitLab.

Overall, the results suggest that professional support was the most prominent support-related theme in the dataset, while work-life balance and emotional support were less frequently mentioned. However, these values represent response counts rather than percentages, so the differences may partly reflect different numbers of responses collected from each company. The heatmap shows the frequency of reported categories, but it does not measure the quality or effectiveness of the support provided.
We have descriptive findings but the hypothesis 4 is still to be tested. The analysed categories do not specifically represent access instructions. 

A deeper look what is the organisation communicating - Focusing on Gitlab webscraped content:

Extracted headings (h2 from the HTML content) 
Looking into the h2 content, we can identify two main topics: 
1. Related Benefits Pages
2. We've Got You Covered: Our Benefits Philosophy

Topic 1: Communication Channels and Resources

This headline groups links to access specific benefits from the company
Relation with the benefits_mh_table: This website clearly shows specific channels to access the mental health benefits and, looking to the benefits_mh_table, we can find 25,76% of respondents who don't know if their employer provides benefits and state having a mental health condition. 
Even if a company has structures benefits pages, failing to effectively disseminate this information may lead workers elegible to these benefits to miss this information.

Topic 2: Corporate Culture and Processes

This topic presents the company's philosophy that the benefits should be easy to understand, transparent and available when necessary
Relation with the benefits_mh_table: The connection here seems to be strong. When the company have this philosophy active and the benefits are transparent (respondents on the survey that state they have benefits), 51,16% state they have a mental health condition, against 4,99% that don't know if they have a mental health condition. Open communication and a strong welcoming philosophy reduce the communication barriers in the workplace. 

Extracted sub-headings (h3 from the HTML content):

Workplace Resources and Philosophy
1. Clear Benefits, Real Support
2. Your Support Team and Resources
3. Our Global Approach
4. Our Guiding Principles
5. How We Continuously Improve Your Benefits
6. 7. We Celebrate Improvements Together

These headings suggest that the organisation communicates its benefits through several dimensions:
| Heading |	Possible interpretation | Relevance |
| Clear Benefits, Real Support | Benefits and employee support	| Communicating available support | 
| Your Support Team and Resources |	Access to support and resources | Employee assistance |
| Our Global Approach |	Organisation-wide benefits philosophy | Consistency across locations |
| Our Guiding Principles | Organisational values |	Culture and employee experience |
| How We Continuously Improve Your Benefits | Continuous improvement	| Adapting employee benefits |
| We Celebrate Improvements Together | Recognition and collective culture | Workplace environment |


### Thematic Comparision between the two data sources: Employee Survey and Tech Company Puplic Communication:

As we cannot match a survey response to a specific company website, we just compared the findings to look for similarities, differences and questions that emerge from two different sources.

| Theme	Employee survey | Company websites	| Question to investigate in the future | 
| Mental health benefits |	Do employees report benefits?	| Do companies mention mental health coverage? | Is this type of support prominent in both perspectives? |
| Support resources	| Do employees report available resources? |	Do companies communicate counselling, therapy or assistance?	| Are different types of resources being communicated? |
| Workplace well-being	| Do employees discuss mental health at work? |	Do companies mention wellbeing, stress or burnout?	| How much attention is given to workplace well-being? |

Key question: Are organisations not only providing support, but also ensuring that employees can identify and access the resources relevant to their needs?

Final Takeaway
Employees who report receiving benefits are more likely to report access to workplace resources.
However, many employees are still unsure about which benefits and resources are available to them.
Employers should improve the clarity, accessibility, and targeting of mental-health benefits communication.

To conclude, our analysis suggests that providing mental-health benefits is only part of the solution. Employees also need to know that these resources exist, understand how to access them, and feel that the information is easy to find. Clearer and more targeted communication could help employers ensure that available support reaches the people who need it.


