# Health Super App  

## IBDCare  

### Table of Contents  
1. [Introduction](#introduction)  
2. [Motivation](#motivation)  
3. [User Research and Persona Creation](#user-research-and-persona-creation)  
   - [Persona 1: Emily](#persona-1-emily)  
   - [Persona 2: Antonio](#persona-2-antonio)  
4. [User Journey Mapping](#user-journey-mapping)  
5. [Wireframing and Prototype Design](#wireframing-and-prototype-design)  
6. [Usability Testing](#usability-testing)  
7. [Reflection](#reflection)  

### Introduction  
Welcome! My name is **Jaeden**, and this is a guide to developing the UI behind a **telemedicine app** for individuals with **chronic illnesses**. Below, I've shared my process in designing a **UI and UX** tailored to its users using research methods.  

### Motivation  
This app serves as a **centralized platform** for **patients with Inflammatory Bowel Disease (IBD)** to:  
- Contact their healthcare practitioners  
- Manage their disease activity  
- Track their medication  

IBD is rising in **Canada**, with a **2.44% year-over-year increase**, according to the **NIH** ([source](https://pmc.ncbi.nlm.nih.gov/articles/PMC10478802/#:~:text=In%20Canada%2C%20the%20prevalence%20of,year%20over%20the%20next%20decade.)). Being a **chronic illness**, IBD requires **lifelong medical monitoring**, with disease activity fluctuating over time. Since many patients live in **rural areas**, **telemedicine** has emerged as a crucial tool.  

According to a **Springer Nature** article ([source](https://link.springer.com/article/10.1007/s11894-020-0751-0)), telemedicine in **IBD care** is:  
- **Safe and effective**  
- **Financially beneficial** for chronic disease management  
- **Enhances patient quality of life**  
- **Improves clinical outcomes**

The reason behind implementing a specific chronic illness for the Health Super App is that all chronic diseases have specific pain points, challenges, and features that might not be scalable between different diseases. For example, the symptom tracker cannot be generalized because different diseases affect different body parts. Less obviously, however, even the medication tracker would not necessarily be scalable since some medications are self-administered and others are administered at hospitals. 

### Existing Solutions 
Looking into the existing telemedicine apps that exist for patients with IBD, there is one large contender called MyGut created by Chrons and Colitis Canada. This app allows users to track their symptoms and export a report to their healthcare practitioners. MyGut allows users to track pain, washroom usage, and lifestyle habits (sleep, diet and nutrition) [source](https://crohnsandcolitis.ca/Support-for-You/MyGut). Also, the MyGut app acts as a resource center for patients where they can find information and resources for their illnesses. Where this app stands out in my opinion is the ability to export a document about their health, this is especially useful because it shows the history of the patient in detail. 

- What this app can add! 

## User Research and Persona Creation  

To conduct user research, I used interviews and secondary research. The small user base for an IBD-focused chronic health app made these the most viable options. Secondary literature on IBD and telemedicine is extensive, and interviews can provide qualitative insights from a targeted audience. Below I will outline some of my findings that will become useful in designing the UI/UX of IBDCare. 

### Assessment of the current literature 
Incidence, Prevalence, and Racial and Ethnic Distribution of Inflammatory Bowel Disease in the United States
Lewis, James D. et al.
Gastroenterology, Volume 165, Issue 5, 1197 - 1205.e2

According to this study which pooled over 14 million Americans with at least 4 years of health insurance history, IBD affects 721 per 100,000 people with a 95% confidence. When extrapolated to the American population as a whole, it totals around 2.4 million people who have IBD. 

After 42,964,750 person-years of follow-up, the study also highlights age trends, gender demographics, and race demographics of those who suffer from IBD. The peak incidence age is between 20 and 30 years of age, and there are stable levels of incidence between ages 30 and 80. After 80 years, the incidence rate decreases. Here is a table showing us the results: 
#### Incidence Chart (When the disease is diagnosed)
<img width="761" alt="Screenshot 2025-02-23 at 11 03 30 AM" src="https://github.com/user-attachments/assets/61eb01bc-4716-4285-9bdc-4a97c9920338" />
##### Including incidence rates is important because it will tell us at what age people would start using an app after diagnosis. 
From the data, we can also make some observations about the gender of those with IBD and their age groups. The data suggests that IBD incidence is slightly male-dominated as is shown in every age group in the above figure, but the difference is quite minimal. Regarding age, although the largest cohort is those between 20-30, teenagers also form a substantial cohort of those with IBD.

#### Prevalence Chart 
<img width="738" alt="Screenshot 2025-02-23 at 11 45 48 AM" src="https://github.com/user-attachments/assets/3755dde3-a469-4934-ba53-69fca0c71d35" />
###### The prevalence rate is important because it gives us an idea of our user base's age. Since the disease is chronic, the is an upward trend as age increases. 
From the data we can see that on average, women have a slightly higher prevalence of IBD compared to men, but the numbers are very similar. What's of note for the development of the app is the age groups of those with IBD - they are mostly in the older population. This is even though IBD incidences are increasing yearly. The largest age cohort is 65-79, but there is a steady increase as age increases. 


### Interview with an anonymous patient 1
[Read the full interview](interview.md){:target="_blank"}

Share


You said:
Give me a bibligoray of the literatue research pertaining to IBD care and telemedince, specifically user experience focused research
ChatGPT said:
Here is a selection of research articles focusing on user experiences in telemedicine for Inflammatory Bowel Disease (IBD) care:

"Telemedicine in Inflammatory Bowel Diseases: A New Brick in the Medicine of the Future?"
Authors: [Authors not specified]
Summary: This review discusses various telemedicine applications in IBD management, including telemonitoring, teleconsulting, teleducation, telenursing, telenutrition, and telepathology. It highlights the need for targeted studies to evaluate these applications and suggests future research directions, particularly in telepsychology and tele-endoscopy. 
PMC.NCBI.NLM.NIH.GOV

"International Organization for the Study of Inflammatory Bowel Disease: Global Strategies for Telemedicine and Inflammatory Bowel Diseases"
Authors: [Authors not specified]
Summary: This article provides insights into telemedicine practices among IBD specialists, sharing regulatory, financial, and practical considerations for incorporating telemedicine into clinical practice. It emphasizes the importance of government and payer support for sustaining telemedicine use beyond the COVID-19 pandemic. 
PMC.NCBI.NLM.NIH.GOV

"Applying Telemedicine to Multidisciplinary Pediatric Inflammatory Bowel Disease Care"
Authors: [Authors not specified]
Summary: This manuscript describes the transition of multidisciplinary pediatric and adolescent IBD care to a telemedicine model. It leverages technology, a multidisciplinary team, and quality improvement methods, and summarizes literature on telemedicine in pediatric IBD care with a focus on multidisciplinary approaches. 
PUBMED.NCBI.NLM.NIH.GOV

"Transforming Access to Specialist Care for Inflammatory Bowel Disease: The PACE Telemedicine Program"
Authors: [Authors not specified]
Summary: This article discusses the PACE Telemedicine Program at Mount Sinai Hospital in Toronto, which provides telemedicine consultations for IBD patients in underserved areas of Ontario. The program aims to reduce wait times and bridge geographic disparities in access to gastroenterologists. 
PMC.NCBI.NLM.NIH.GOV

"Placing Value on Telemedicine for Inflammatory Bowel Disease"
Authors: [Authors not specified]
Summary: This commentary examines a randomized controlled trial assessing a telemonitoring program for IBD patients. It discusses the importance of identifying appropriate outcomes for telemedicine interventions and suggests that demonstrating maintained quality of care at lower costs could enhance the value of such programs. 
PUBMED.NCBI.NLM.NIH.GOV

These articles provide valuable insights into the user experience and implementation of telemedicine in IBD care.


Sources








You said:
give me staticsitcs on the demographic of those with IBD
ChatGPT said:
Inflammatory Bowel Disease (IBD), encompassing Crohn's disease and ulcerative colitis, exhibits varying prevalence and incidence across different regions and demographics.

Global Statistics:

Prevalence: As of 2017, the prevalence of IBD exceeded 0.3% in North America, Oceania, and many European countries. 
PUBMED.NCBI.NLM.NIH.GOV

Incidence Trends: While the incidence in North America and Europe has stabilized or decreased, newly industrialized countries in Africa, Asia, and South America have reported rising incidence rates since 1990. 
PUBMED.NCBI.NLM.NIH.GOV

Canada-Specific Statistics:

Prevalence: In 2014, approximately 0.7% of Canadians were living with IBD, with projections suggesting this could reach nearly 1% by 2030. 
ACADEMIC.OUP.COM

Regional Variations: Nova Scotia has historically reported one of the highest incidences of IBD globally. 
BMCGASTROENTEROL.BIOMEDCENTRAL.COM

United States Statistics:

Prevalence: Estimates indicate that between 2.4 and 3.1 million adults in the U.S. were diagnosed with IBD as of 2015. 
CDC.GOV
Demographic Insights:

Age of Onset: IBD commonly manifests between the ages of 15 and 30, with a secondary onset peak in the sixth decade of life. 
EN.WIKIPEDIA.ORG

Gender Distribution: Both Crohn's disease and ulcerative colitis affect males and females in approximately equal proportions. 
EN.WIKIPEDIA.ORG

Ethnic Variations: Higher prevalence rates have been observed among individuals of Ashkenazi Jewish descent compared to other ethnic groups. 
EN.WIKIPEDIA.ORG

These statistics underscore the significant and evolving impact of IBD across various populations and regions.


Sources











You said:
what about age reanges, gender, is there a single ncbi article that goes into this
ChatGPT said:
A comprehensive study titled "Inflammatory Bowel Disease Prevalence by Age, Gender, Race, and Geographic Location in the U.S. Military Health Care Population" provides detailed demographic insights into Inflammatory Bowel Disease (IBD). This research analyzed data from the U.S. military health care system, encompassing over 10 million beneficiaries, to determine the prevalence of IBD, including Crohn's disease (CD) and ulcerative colitis (UC), across various demographic factors. 
PUBMED.NCBI.NLM.NIH.GOV

Key Findings:

Overall Prevalence: The study identified 35,404 cases of IBD, resulting in an overall prevalence of 348 per 100,000 individuals. Specifically, UC had a prevalence of 202 per 100,000, while CD was at 146 per 100,000.

Age Distribution: IBD prevalence varied with age, peaking among individuals aged 35–44 years.

Gender Differences: Females exhibited a higher prevalence of IBD compared to males, with rates of 417 versus 284 per 100,000, respectively.

Racial Variations: The prevalence of IBD was highest among Caucasians, followed by African Americans, Hispanics, and Asians.

Geographic Distribution: Variations in IBD prevalence were observed across different geographic locations within the United States.

These findings underscore the importance of considering demographic factors in the diagnosis, management, and research of IBD.


Sources







You said:
i want the broader population not us military
ChatGPT said:
Inflammatory Bowel Disease (IBD), encompassing Crohn's disease and ulcerative colitis, affects various demographic groups differently. While previous data indicated that IBD affects men and women equally, more recent studies suggest a higher prevalence in women. This disparity may be attributed to factors such as hormonal influences, immune system differences, and anatomical variations. 
TIME.COM

Age Distribution:

Common Age of Onset: IBD is frequently diagnosed between the ages of 15 and 35. 
CROHNSCOLITISFOUNDATION.ORG

Incidence in Older Adults: Recent studies have shown that the incidence rate of IBD in the elderly population in the U.S. is similar to that in younger adults, indicating that IBD can develop at any age. 
NCBI.NLM.NIH.GOV

Gender Differences:

Prevalence: Recent studies have shown that digestive issues, including IBD, are more prevalent among women than men. 
TIME.COM
Geographic Variations:

Canada: Ontario has one of the highest prevalence rates of IBD globally. Between 1999 and 2008, the incidence of IBD increased, particularly among children and adults, while rates remained stable in the elderly population. 
PUBMED.NCBI.NLM.NIH.GOV

United States: In 2015, an estimated 3.1 million U.S. adults (1.3%) had received an IBD diagnosis, with prevalence varying across different sociodemographic groups. 
CDC.GOV

These findings highlight the importance of considering demographic factors such as age, gender, and geographic location in the diagnosis, management, and research of IBD.

Recent Insights into IBD Demographics and Risk Factors
time.com
Why Gut Health Issues Are More Common in Women
163 days ago
couriermail.com.au
Revealed: Everyday foods causing sharp rise in debilitating condition
13 days ago

Sources











You said:
parse this data for me: 
We analyzed data for 14,420,692 individuals with ≥4 years of continuous insurance, of whom 115,715 met the primary definition of IBD requiring ≥2 diagnoses or 1 diagnosis and a prescription for an IBD medication. The age-, sex-, and insurance-standardized prevalence per 100,000 population was 721 (95% CI, 717–726) for IBD, 378 (95% CI, 375–382) for ulcerative colitis, and 305 (95% CI, 302–308) for Crohn’s disease. Extrapolated to the 2020 US Census estimate of 331,449,281 US population, there are an estimated 2.390 million Americans with IBD, 1.253 million with ulcerative colitis, and 1.011 million with Crohn’s disease. The combined estimates for ulcerative colitis and Crohn’s disease do not total that of IBD due to patients identified with IBD but who could not be assigned specifically to either ulcerative colitis or Crohn’s disease. Prevalence estimates using a range of other assumptions are included in Table 1.
ChatGPT said:
Here's a breakdown of the data:

Study Population:

Analyzed 14,420,692 individuals with at least 4 years of continuous insurance.
Out of these, 115,715 met the criteria for having Inflammatory Bowel Disease (IBD) based on medical diagnoses and prescriptions.
Prevalence Rates (per 100,000 people):

IBD overall: 721 (95% Confidence Interval: 717–726)
Ulcerative Colitis (UC): 378 (95% CI: 375–382)
Crohn’s Disease (CD): 305 (95% CI: 302–308)
Extrapolated Estimates for the 2020 U.S. Population (331.4 million people):

Total IBD Cases: 2.390 million
Ulcerative Colitis Cases: 1.253 million
Crohn’s Disease Cases: 1.011 million
Discrepancy: The total number of UC + CD cases is less than the overall IBD estimate because some individuals were diagnosed with IBD but could not be definitively classified as having either UC or CD.
Additional Data:

The study includes other prevalence estimates based on different assumptions (found in Table 1 of the original source).
Key Takeaways:
About 0.72% (or 1 in 139) of the U.S. population has IBD.
Ulcerative colitis is slightly more common than Crohn’s disease.
Some IBD cases remain unclassified into UC or CD.
These estimates are based on insured individuals, which may not fully represent the general population.
Would you like any further insights or visualizations?







You said:
Incidence of Inflammatory Bowel Disease in the United States
In the primary analysis of incidence, where we required 4 years of enrollment before the start of follow-up, the combined cohort contributed 42,964,750 person-years of follow-up, during which 4747 met the high-probability definition of a newly diagnosed IBD and 2221 met the lower-probability definition. The age- and sex-standardized incidence of IBD per 100,000 person-years in the United States was 10.9 (95% CI, 10.6–11.2). In a sensitivity analysis including both the high- and lower-probability algorithms, the pooled incidence rate per 100,000 person-years was 15.9 (95% CI, 15.5–16.3). The incidence of IBD, ulcerative colitis, and Crohn’s disease peaked in the third decade of life, decreased to a stable relatively stable level across the fourth to eighth decades, and declined further beyond age 80 (Figure 1 and Supplementary Table 1). Overall, the incidence of ulcerative colitis (6.3; 95% CI, 6.1–6.6) was higher than that of Crohn’s disease (4.1; 95% CI, 3.9–4.3). However, among children, the incidence of Crohn’s disease was higher than ulcerative colitis (Figure 1 and Supplementary Table 1).
ChatGPT said:
Here's a breakdown of the incidence data:

Study Parameters
Follow-up Data:
Total 42,964,750 person-years of follow-up.
4747 cases met the high-probability definition of newly diagnosed IBD.
2221 additional cases met a lower-probability definition.
Incidence Rates (per 100,000 person-years)
Primary Analysis (High-Probability Cases Only):
Overall IBD Incidence: 10.9 (95% CI: 10.6–11.2).
Sensitivity Analysis (Including Lower-Probability Cases):
Overall IBD Incidence: 15.9 (95% CI: 15.5–16.3).
Ulcerative Colitis: 6.3 (95% CI: 6.1–6.6).
Crohn’s Disease: 4.1 (95% CI: 3.9–4.3).
Age Trends
Peak Incidence: 3rd decade of life (ages 20–30).
Stable Levels: Across 4th to 8th decades (ages 30–80).
Decline: After age 80.
Children: Higher incidence of Crohn’s disease compared to ulcerative colitis.
Key Takeaways
IBD incidence in the U.S. is estimated at ~11 per 100,000 person-years (up to ~16 per 100,000 in sensitivity analysis).
Ulcerative colitis is more common than Crohn’s disease overall, except in children, where Crohn’s is more frequent.
Peak age of onset is in young adulthood (20s), with a gradual decline in later decades.
Would you like further analysis or visual representation of this data?







You said:
summarize this interview: 

---
layout: default
title: Interview with an IBD Patient
---

# Interview with an IBD Patient

## Section 1: General Information



**1. How old are you?**
Answer: 53 years old. 

**2. How long have you been diagnosed with IBD?**
Answer: Since 2007. 

**3. What type of IBD do you have?**
Answer: Ulcerative Colitis. 

**4. What treatments are you currently using?**
Answer: Mezavant. 

## Section 2: Telemedicine Experience
**5. Have you ever used a telemedicine service for IBD care?**
Answer: No. 


**6. If yes, what was your main reason for using telemedicine?**
Answer: N/A


**7. What are your biggest frustrations with telemedicine for IBD?**
Answer: Yeah. Almost every interaction leads to a referral to the ER. 

Followup question: 
What was the nature of the telehealth app you were using? 
Telehealth Ontario call line. Where I spoke to a nurse on the phone. The information was useful because at least it confirmed that I needed to see a doctor. 


## Section 3: UI/UX Preferences
**8. How easy should it be to book an appointment on a telemedicine app?**
Answer: Very easy, 5 clicks or less. 


**9. What is your preferred method for receiving appointment reminders?**
Sms? Email? Notification? 
Answer: SMS text with appointment details. 


**10. How important is it for you to have built-in symptom tracking in a telemedicine app?**
Answer: I would use it. It's important because it can help me understand the severity of the current situation. 

Would you find a history or a graph of your symptoms useful? 
answer: I think it would be useful for the doctor, I wouldn't have to retell all of that information again. 


**11. What features would you want in a telemedicine dashboard?**
Answer: Hmm. Test result history (biopsy results, blood test results), Upcoming appointments. 



## Section 4: Accessibility & Design
**12. How would you prefer a telemedicine app to display medical information?**
Answer: 


**13. Do you find dark mode or light mode easier to read?**
Answer: Dark mode. 


**14. How would you rate your comfort level with technology?**
Answer: Out of ten I would say 7. Reasonably comfortable. 


**15. What device would you most likely use for telemedicine visits?**
Answer: Mobile phone. 


## Section 5: Final Thoughts
**16. What’s the #1 feature that would make a telemedicine app more useful for managing IBD?**
Contact with the doctor's office. Quick response with a nurse for example. This would be better than phoning. 



[Back to Main Page](./README.md)

Summary: Interview with an IBD Patient
General Information:
**Age:** 53
**Diagnosis:** Ulcerative Colitis (since 2007)
**Current Treatment:** Mezavant
**Telemedicine Experience:**
Has not used telemedicine for IBD care but has used Telehealth Ontario (nurse call line) for medical advice.
Frustration with telemedicine: Most interactions lead to ER referrals.
Found telehealth useful in confirming the need for medical attention.
**UI/UX Preferences:**
Booking Appointments: Should be 5 clicks or less.
Appointment Reminders: Prefers SMS with details.
Symptom Tracking: Finds it important and useful, especially if it generates a history or graph to avoid repeating information.
Preferred Dashboard Features: Test result history (e.g., biopsy, blood tests), upcoming appointments.
**Accessibility & Design:**
Preferred Mode: Dark mode for readability.
Comfort with Technology: 7/10 (reasonably comfortable).
**Preferred Device for Telemedicine:** Mobile phone.
**Final Thoughts:**
#1 Desired Feature: Direct contact with a doctor’s office, ideally a nurse, for quick responses—better than calling.


### Interview with an anonymous patient 2
[Read the full interview](interview-two.md){:target="_blank"}

Summary: 

### Persona 1: Emily  
<img width="1081" alt="Screenshot 2025-02-23 at 4 14 24 PM" src="https://github.com/user-attachments/assets/65d32118-8816-435e-945d-cc4a821c74d2" />

### Persona 2: Antonio  
<img width="1076" alt="Screenshot 2025-02-20 at 5 07 35 PM" src="https://github.com/user-attachments/assets/9ba89196-ac04-45d1-863d-b5162978211e" />

## User Journey Mapping  
- **Map the user journey**: Create a user journey map illustrating the **typical process** a user undergoes when interacting with the app.  
- Identify **key touchpoints**, **emotions**, and **potential pain points** at each stage.  
![Health Super App](https://github.com/user-attachments/assets/41af09ab-e47a-4955-9937-cdaaa0fe185a)

## Research conclusions and Design Decision Impact


## Wireframing and Prototype Design  
- **Create wireframes**: Design **low-fidelity wireframes** for key screens (e.g., home screen, medication reminder, doctor appointment scheduling).
### Low-fidelity wireframes: 
<img width="667" alt="Screenshot 2025-02-23 at 6 09 58 PM" src="https://github.com/user-attachments/assets/735116f9-3fa8-4cf7-b8c4-be38241ca1ae" />
<img width="668" alt="Screenshot 2025-02-23 at 6 10 15 PM" src="https://github.com/user-attachments/assets/974da9a6-2484-4cf8-a2c4-2bbc5b581915" />


- **Prototype**: Develop a **clickable prototype** using **Figma, Adobe XD, or another tool** to showcase the main features and user flow.  

## Usability Testing  
- **Plan a usability test**: Define a usability testing plan including goals, user tasks, and how feedback is collected.  
- **Analyze feedback**: Outline methods to interpret user feedback and iterate on the design.  

## Reflection  
- How the **UX design process** helped identify **user needs** and improve the product.  
- Challenges encountered during the **design process** and how they were overcome.  
