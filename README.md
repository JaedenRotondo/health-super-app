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
#### Summary
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

#### Summary

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
