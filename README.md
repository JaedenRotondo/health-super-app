
# IBDCare  

## IBDCare - Table of Contents
1. [Introduction](#introduction)
2. [Motivation](#motivation)
3. [Existing Solutions](#existing-solutions)
4. [User Research and Persona Creation](#user-research-and-persona-creation)
   - [Assessment of the Current Literature](#assessment-of-the-current-literature)
   - [Interview with Anonymous Patient 1](#interview-with-an-anonymous-patient-1)
   - [Interview with Anonymous Patient 2](#interview-with-an-anonymous-patient-2)
   - [Persona 1: Emily](#persona-1-emily)
   - [Persona 2: Antonio](#persona-2-antonio)
5. [User Journey Mapping](#user-journey-mapping)
6. [Research Conclusions and Design Decision Impact](#research-conclusions-and-design-decision-impact)
7. [Color Scheme](#color-scheme)
8. [Wireframing and Prototype Design](#wireframing-and-prototype-design)
   - [Low-Fidelity Wireframes](#low-fidelity-wireframes)
   - [High-Fidelity Prototype](#high-fidelity-prototype)
     - [Sign-up and Login](#sign-up-and-login)
     - [Appointments and Booking](#appointments-and-booking)
     - [Symptoms](#symptoms)
     - [Medication Tracker](#medication-tracker)
     - [Quiz](#quiz)
     - [Summary Available to Doctor](#summary-available-to-doctor)
     - [Analysis](#analysis)
9. [Usability Testing](#usability-testing)
   - [Goals and Methods](#goals-and-methods)
10. [Reflection](#reflection)



### Introduction  
Welcome! My name is Jaeden, and this is a guide to developing the UI behind a telemedicine app for individuals with chronic illnesses. Below, I've shared my process in designing a **UI and UX** tailored to its users using research methods. The point of this blog is to highlight the correct approach to developing UI/UX using Design Thinking. Design Thinking is a non-linear yet iterative approach to design as follows: 
![image](https://github.com/user-attachments/assets/cfc67bd8-7bef-4e12-a472-f0f68f1a9acb)

For the sake of this project, I will only include the first iteration and explain how I would continue testing my prototype and future steps. Also, although the app would have a practitioner side, this blog will only look into the research and UI/UX development for the patient side.

### Motivation  
This app serves as a centralized platform for patients with Inflammatory Bowel Disease (IBD) to:  
- Contact their healthcare practitioners  
- Manage their disease activity  
- Track their medication  

IBD is rising in Canada, with a 2.44% year-over-year increase, according to the NIH ([source](https://pmc.ncbi.nlm.nih.gov/articles/PMC10478802/#:~:text=In%20Canada%2C%20the%20prevalence%20of,year%20over%20the%20next%20decade.)). Being a **chronic illness**, IBD requires **lifelong medical monitoring**, with disease activity fluctuating over time. Since many patients live in rural areas, telemedicine has emerged as a crucial tool.  

According to a **Springer Nature** article ([source](https://link.springer.com/article/10.1007/s11894-020-0751-0)), telemedicine in **IBD care** is:  
- **Safe and effective**  
- **Financially beneficial** for chronic disease management  
- **Enhances patient quality of life**  
- **Improves clinical outcomes**

The reason behind implementing a specific chronic illness for the Health Super App is that all chronic diseases have specific pain points, challenges, and features that might not be scalable between different diseases. For example, the symptom tracker cannot be generalized because different diseases affect different body parts. Less obviously, however, even the medication tracker would not necessarily be scalable since some medications are self-administered and others are administered at hospitals. 

### Understanding the Issue 
IBD is on the rise in Canada and around the world. With more patients, new assessment techniques and forms of communication will have to be established. It is already well known that many chronic patients have issues with medication adherence, and many healthcare professionals are looking into the possibility of tackling these issues with telemedicine. In creating a user-friendly app, it is important to understand the users and their accessibility needs. The IBD population is not necessarily the same as the general population or even the population of those with a chronic illness. The purpose of the below research is to determine the specific needs of IBD patients and create an accessible health app that will be effective for both patients and health professionals. 


### Existing Solutions 
Looking into the existing telemedicine apps that exist for patients with IBD, there is one large contender called MyGut created by Chrons and Colitis Canada. This app allows users to track their symptoms and export a report to their healthcare practitioners. MyGut allows users to track pain, washroom usage, and lifestyle habits (sleep, diet and nutrition) [source](https://crohnsandcolitis.ca/Support-for-You/MyGut). Also, the MyGut app acts as a resource center for patients where they can find information and resources for their illnesses. Where this app stands out in my opinion is the ability to export a document about their health, this is especially useful because it shows the history of the patient in detail. 

The issue with MyGut that could be capitalized on with IBDCare is the integration of its features within the hospital context. I am proposing that this app be used by both healthcare professionals as well as patients. This would allow doctors to interpret the results of the disease tracking natively on the app, and allow for appointment booking based on hospital availability as well as direct message support. 

## User Research and Persona Creation  

To conduct user research, I used interviews and secondary research. The small user base for an IBD-focused chronic health app made these the most viable options. Secondary literature on IBD and telemedicine is extensive, and interviews can provide qualitative insights from a targeted audience. Below I will outline some of my findings that will become useful in designing the UI/UX of IBDCare. 

### Assessment of the current literature 
The major research article for my secondary resource analysis is from: 
>Incidence, Prevalence, and Racial and Ethnic Distribution of Inflammatory Bowel Disease in the United States
>Lewis, James D. et al.
>Gastroenterology, Volume 165, Issue 5, 1197 - 1205.e2

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

##### UI/UX Preferences:

**Booking Appointments:** Should be 5 clicks or less.

**Appointment Reminders:** Prefers SMS with details.

**Symptom Tracking:**

Finds it important and useful, especially if it generates a history or graph to avoid repeating information.
Preferred Dashboard Features: Test result history (e.g., biopsy, blood tests), upcoming appointments.

**Accessibility & Design:**
Preferred Mode: Dark mode for readability.

**Comfort with Technology:** 7/10 (reasonably comfortable).

**Preferred Device for Telemedicine:** Mobile phone.

**#1 Desired Feature:** Direct contact with a doctor’s office, ideally a nurse, for quick responses—better than calling.


### Interview with an anonymous patient 2
[Read the full interview](interview-two.md){:target="_blank"}

#### Summary
General Information:
**Age:** 23

**Diagnosis:** Ulcerative Colitis (~10 years)

**Current Treatment:** Oral Pentasa and mesalamine

**Telemedicine Experience:**

Uses telemedicine because their doctor’s office primarily operates through Medeo Health for virtual appointments and test requisitions.
**Biggest frustration:** Lack of support from the doctor, which can feel isolating and impersonal.

**UI/UX Preferences:**

**Appointment Booking:** Should be relatively easy, as calling is difficult (voicemail restrictions).

**Appointment Reminders:** Prefers SMS messages.

**Symptom Tracking:** Would use it if the doctor finds it useful for monitoring flares.

P**referred Dashboard Features:** Appointment booking, test results, and test result availability status.

**Accessibility & Design:**

**Medical Information Display Preference:** Both summary and detailed reports from the doctor.

**Preferred Mode:** Light mode for readability.

**Comfort with Technology:** Very high.

**Preferred Device for Telemedicine:** Phone.

**Final Thoughts:**

**#1 Desired Feature:** Integration with the hospital network and access to personal feedback to avoid feeling isolated.

**Overall View on Telemedicine:** Helpful for long-distance care, as they don't live in the same city as their doctor.



### Persona 1: Emily  
<img width="968" alt="Screenshot 2025-02-23 at 11 27 05 PM" src="https://github.com/user-attachments/assets/b8fea1ca-cf5d-457f-abe7-ea18c9e1e394" />

### Persona 2: Antonio  
<img width="969" alt="Screenshot 2025-02-23 at 11 25 06 PM" src="https://github.com/user-attachments/assets/b6af6cc9-15e7-4791-b808-8f28d714bcc3" />

## User Journey Mapping  
- **Map the user journey**: Create a user journey map illustrating the **typical process** a user undergoes when interacting with the app.  
- Identify **key touchpoints**, **emotions**, and **potential pain points** at each stage.  
![Health Super App](https://github.com/user-attachments/assets/41af09ab-e47a-4955-9937-cdaaa0fe185a)

## Research conclusions and Design Decision Impact
Based on the Journey Map, we can conclude that some of the important considerations in making an efficient UI/UX are: 
1. Easy onboarding & setup – Users want a smooth and simple account creation process, ideally integrated with hospital systems.
2. Easy symptom tracking – Users aim to monitor their condition with minimal friction, ensuring easy data entry and visualization.
3. Help with adherence – Users need timely reminders and a simple way to log medication intake while ensuring they can track its effectiveness.
4. Reliable appointment booking – Users want quick and easy doctor appointments with clear availability.

There are also some pain points we need to watch out for:  
1. Users struggle with technical setup and connecting to hospital systems.
2. Users not tracking symptoms because it is convoluted or takes too long.
3. Since users are mostly older, a simple and large-text design will increase accessibility

## Color Scheme 
![IBDCare Color Pallete](https://github.com/user-attachments/assets/b382b9b2-07bb-49be-8db3-70f68b7884cd)

Above is the color scheme I decided to implement in my app. The green can be associated with hospital uniforms and the light pastel colors are not only easy on the eyes but give the user a calming effect that reminds them of healthcare. Even though one of the interviewees notes that he preferred dark mode, I do not think dark mode would be suitable for a healthcare app. Light mode feels more serious in clinical settings. 

## Wireframing and Prototype Design  

### Low-fidelity wireframes: 
<img width="667" alt="Screenshot 2025-02-23 at 6 09 58 PM" src="https://github.com/user-attachments/assets/735116f9-3fa8-4cf7-b8c4-be38241ca1ae" />
<img width="668" alt="Screenshot 2025-02-23 at 6 10 15 PM" src="https://github.com/user-attachments/assets/974da9a6-2484-4cf8-a2c4-2bbc5b581915" />


### High-fidelity prototype: 
#### Sign-up and login: 
The sign-up page includes some necessary information needed from the user to link their accounts to the hospital's account. 

<img width="867" alt="Screenshot 2025-02-23 at 11 09 08 PM" src="https://github.com/user-attachments/assets/bb6d0667-914f-4d10-a14d-8c40a1c6374d" />

#### Appointments and booking 
The user can see upcoming and past appointments with summaries. They are also able to edit future appointments if they are unable to make it. There is a "Take Quiz" button on top of the future appointment card because users are prompted to do a Disease Activity Index (DAI) test which can be a useful diagnostic tool for their doctors. 

<img width="726" alt="Screenshot 2025-02-23 at 11 09 26 PM" src="https://github.com/user-attachments/assets/be17fe78-c22c-4d9c-b873-d97cbfd4466a" />

#### Quiz
This page shows the Disease Activity Index (DAI) tool previously mentioned. 

<img width="348" alt="Screenshot 2025-02-23 at 11 10 49 PM" src="https://github.com/user-attachments/assets/bbd25f50-bb46-4d1a-b815-b740a983efe7" />

#### Symptoms 
The symptoms page was created keeping in mind the pain points of users who do not want to spend much time tracking their symptoms. This symptom tracker allows 1-click logging where a user can tap on an image that best describes them.

<img width="355" alt="Screenshot 2025-02-23 at 11 11 28 PM" src="https://github.com/user-attachments/assets/d3f852e6-7825-448e-9cea-9437378bbd2c" />

#### Summary available to doctor
Summary of medical history using AI: this lets doctors and users briefly review medical records in quick-paced appointments.

<img width="375" alt="Screenshot 2025-02-23 at 11 12 10 PM" src="https://github.com/user-attachments/assets/d1478b9a-8986-4f66-915c-f255d772e78c" />

#### Medication Tracker
The medication tracker is a simple 1-click a day tracking feature that was implemented similarly to the symptom tracker. The idea is that as long as the process is quick and intuitive, the chances of the user completing the 30-second activity based on a daily notification are higher. 

<img width="431" alt="Screenshot 2025-02-23 at 11 12 43 PM" src="https://github.com/user-attachments/assets/83c97b86-29aa-43c8-bf44-1d46bdb8d815" />

#### Analysis
Based on the statistics that are tracked on the application, graphs are produced for both doctors and users. This is another opportunity for AI to shine in creating a summarized analysis. 

<img width="756" alt="Screenshot 2025-02-23 at 11 13 05 PM" src="https://github.com/user-attachments/assets/2b709bc8-e028-46eb-a8ca-671aad4ac808" />

## Usability Testing  
### Goals and Methods
According to [digitical.gov](https://digital.gov), usability is "how easily and effectively people can accomplish their goals using a product or system, while having a positive experience."

Based on this, the goal of usability testing should be to see if the users were able to accomplish what they wanted to do in the app. For example, if they were able to sign up, log in, book an appointment, track symptoms and take symptom tests. Here are some survey questions we can ask users after user-testing the app: 

1. How intuitive do you rank the application overall? Was it positive or negative?
2. How was your experience tracking symptoms? Were there symptoms you had that were missing?
3. How was your experience booking an appointment? Was there anything which confused you?
4. How was your experience signing up and logging in? Was there anything which confused you?
5. Did you understand all of the terminology used in the Disease Activity Index scoring test?


## Reflection 
By following the User Design Process, we were able to come to conclusions about app design that took into consideration the needs of our consumers. A proper design process allows developers to be empathetic towards their users and consider accessibility issues, users' prior experience with such applications and pain points they might face from poor design choices. In the case of IBDCare, the secondary research was important because it gave insight into the age, gender, and background of the population which has IBD. Knowing these demographic statistics led us to create a simple UI that would be user-friendly for an aging population. 

Secondly, the interviews helped in the design process as they gave insight into what level of experience patients with IBD have with telemedicine and how it was for them. Phone calls were highlighted as being a poor means of communication, therefore IBDCare should use video calls for online appointments and SMS messaging for reminders. Patients said that they would use a symptom tracker and suggested that it might be important for medical professionals, thus on the app we included medically up-to-date symptom quizzes such as the Mayo Index Score. 


### Challenges in the design process and how they were overcome
During the design process, there were some challenges faced. Chiefly among them was the small sample size of people who were diagnosed with IBD. Since IBD only affects 0.72 percent of Canadians, it was not easy to find many people with the illness. Despite this, I was able to interview 2 people with IBD and create a model which was empathetic to their needs. Another way I was able to overcome this issue was by looking into secondary research. The [James Lewis](https://www.gastrojournal.org/article/S0016-5085(23)04776-5/fulltext) text was very helpful because of its large (over 14 million) sample size. 
