---
layout: default
---

# Overview

The IT project idea is to create a text-to-speech robot confidential mental health examination to a person in their own home. The robot, Dr Jane, seeks to overcome to barrier that people with existing mental health disorders already have, in particular, anxiety related disorders, which prevents them from having an initial consultation with their general practitioner (GP).

Dr Jane will ask a series of questions that a GP would normally ask during a mental health examination, then, adding up the numeric scores for each category of disorders, Dr Jane would provide an overview of her findings and provide a recommendation.

The recommendation provided by Dr Jane would not be a medical diagnosis, but instead a referral to invite the person in for an appointment to complete a clinical mental health examination or invite the person for a video conference with a GP.

## Motivation

In Australia, there are 3.9 million people who are experiencing a mental health issue. Our of a population of 24 million, this represents almost 16% of the country.

In addition, the Productivity Commission has estimated that the direct and indirect costs of mental health on the government is in the range of $10 billion and $15 billion each year.

Mental health disorders have an early onset, particularly beginning in young adults and teenagers. The prevalence of disorders developing due to social media is also increasing <fact something here> 

An inexpensive solution if to utilise a combination of Raspberry Pi technology and telemedicine to provide an alternative method for an initial mental health consultation, which in turns greatly improves the quality of life for people suffering from undiagnosed mental illness. At the same time also reducing the enormous public cost, which funds can be allocated elsewhere in the public system.

## Description

The robot, Dr Jane, will provide a medical disclaimer, followed by the option of immediately connecting to emergency services if the person is experiencing a crisis. The person will then be asked a series of questions on a numeric scale that a GP would ask during a mental health examination, and based on the score for each area, provide a recommendation.

The medical disclaimer will have a warning that the advice provided by Dr Jane is general in nature and should not be substituted for GP’s advice nor that it forms a medical opinion in any way.

Upon the person accepting this, it will ask them a series of question to determine if the person may be in danger of harming themselves or another individual. If yes, it will provide them with an option to seek immediate help.

If the user is not experiencing any form of mental crisis, they will be required to enter in their personal details, including their full name, date of birth, address and phone number.

Dr Jane will ask a series of question that focus on the realms of depressive disorders, anxiety disorders, psychosis and personality disorders. 

The first set of questions Dr Jane will ask are general questions based on the Standardised Mini-Mental State Examination (SMMSE) test to quickly evaluate the cognitive state of the individual. Should the person not be able to answer any of the below, they should not continue the test and instead be referred to a specialist:

| Question	                   | Answer            |
|:-----------------------------:------------------|
|What year is this?	           |2019              |
|What season is this?	       |Summer            |
|What month is this?	       |December          |
|What is today’s date?	       |15 December 2019  |
|What day of the week is this? |Sunday            |

The second component of the test is a sequence of 12 questions from the GHQ-12 to measure the psychological stress of the individual. The person will need to answer the questions on a numeric scale of 0 to 3, where 0 represents ‘not at all’ and 3 represents ‘all the time’.

“The 12-item General Health Questionnaire contains three factors, namely Anxiety and Depression, Social Dysfunction, and Loss of Confidence.”  https://hqlo.biomedcentral.com/articles/10.1186/1477-7525-2-63 

| Question	                                                            | Answer                                               |
|:----------------------------------------------------------------------:------------------------------------------------------|
|Have you recently been able to concentrate on whatever you are doing?	|0 – 3 with 0 being the worst and 3 being the greatest.|
|Have you recently lost much sleep due to some worry?                   |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently felt constantly under strain?	                    |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently felt that you could not overcome your difficulties?  |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently been feeling unhappy and depressed?                  |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently been losing confidence in yourself?	                |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently been thinking of yourself as a worthless person?	    |0 – 3 with 0 being the best and 3 being the worst.    |
|Have you recently felt that you are playing a useful role in life?	    |0 – 3 with 0 being the worst and 3 being the greatest.|
|Have you recently felt capable of making decisions about things?       |0 – 3 with 0 being the worst and 3 being the greatest.|
|Have you recently been able to enjoy your normal day-to-day activities?|0 – 3 with 0 being the worst and 3 being the greatest.|
|Have you recently been able to face up to your problems?	            |0 – 3 with 0 being the worst and 3 being the greatest.|
|Have you recently been feeling reasonably happy, all things considered?|0 – 3 with 0 being the worst and 3 being the greatest.|


Upon completion of the test, Dr Jane will add up the results, including reversing some of the results as the numbers can mean a different result, then provide a general recommendation based on the following the best result as per Likert:


| Result        | Outcome                                                                                                                                                  |
|:--------------:----------------------------------------------------------------------------------------------------------------------------------------------------------|
|< 11       	|The answers provided do not indicate that you are under psychological distress or experiencing mental health issues.                                      |
|>= 11          |The answers that you have provided show that you may be under psychological distress which could indicate that you are experiencing a mental health issue.|

Would you like to book an appointment with your GP or videoconference a GP to discuss a treatment plan or further discuss the results?

The drawback to the above tests is that a questionnaire completed by a bot is no substitute to a trained and qualified medical practitioner or mental health nurse or specialist. Similarly, the bot, Dr Jane, does not have the emotional intelligence or capacity to make a medical evaluation independent of the questions in the context of the persons current personal situation.

For example, if the person taking the test is on the Autism spectrum or has a form of learning disorder, they may fail the cognitive test, but their cognitive levels are at level that is normal for themselves personally.

In addition, many physical problems such as a thyroid problem or sleep deficiency can greatly mimic the symptoms of anxiety, depression or psychosis; which can lead to an incorrect self-diagnosis.

## Tools and Technologies and Skills Required

Dr Jane will be an application that is developed in Java and runs on a Raspberry Pi 4 Model B with 4 GB random access memory (RAM), quad core 1.5GHz ARM processor and 32 GB SD Card for storage space. The Raspberry Pi is a micro-computer that is low cost and powerful, allowing mass production of Dr Jane’s for distribution, in a quick manner at minimal cost. The Raspbian Operating System (OS), which is a light weight and based on Debian Linux is standard OS for Raspberry Pi’s. Dr Jane will run the Raspbian OS with a command line interface (CLI) as the application will not utilise the graphical user interface (GUI).

* * *

The following hardware will need to be purchased for Dr Jane from Pi Australia (Trading As: Little Bird Electronics Pty Ltd)

| Question	                                    | Qty | Cost | Purpose                                                                                                                                 |
|:----------------------------------------------:-----:------:-----------------------------------------------------------------------------------------------------------------------------------------|
|Raspberry Pi 4 Model B (4 GB)	                |1    |$94.95|Main hardware device that Dr Jane runs on and will be developed on. Similar to the desktop box of a PC.                                  |
|Raspberry Pi Power Supply USB-C 5V 15W (White) |1    |$19.95|This will provide power to the Raspberry Pi as it does not have battery.                                                                 |
|Raspberry Pi 4 Case	                        |1    |$12.50|The Raspberry Pi case will protect Dr Jane and allow the device to be shipped and handled by other people.                               |
|32GB MicroSD card with NOOBS for Raspberry Pi 4|1    |$24.95|The 32 GB Micro SD card serves as the main disk (like C: drive on a PC) with NOOBS which is the OS installer for Raspbian.               |
|Official Raspberry Pi Keyboard                 |1    |$26.95|The Raspberry Pi keyboard is the compatible keyboard for the Raspberry Pi and the user will input their selections using this.           |
|Speaker Kit for Raspberry Pi	                |1    |$21.95|The speaker kit will provide an audio speaker which Dr Jane will provide a human voice response to the person completing the evaluation. |


Total cost, incl GST: $201.25

The Dr Jane application for the Raspberry Pi will need to be written in Java and requires intermediate Java skills from a Java programmer. In addition, the Java programmer needs to have some hardware skills or knowledge with setting up a Raspberry Pi, at a minimum, some Linux administration skills.

# Outcome
* * *

If the development and distribution of the Dr Jane mental health robot is successful, it will be another method available for all Australians to help them with their mental health diagnose. The earlier that a mental health disorder is diagnosed and treated, the better the outcome is, especially for younger adults to prevent further determination on missed educational, career and social opportunities; which in turn, provides a significant benefit to the public system by reducing costs which can be better spent elsewhere.

The impact of the Dr Jane mental health robot could pave the way for further development of psychological testing by non-humans, with further development inclusive of artificial intelligence (AI).

Overall, the impact could provide substantial benefits for all persons, governments and businesses, but at the same time, a fine line needs to be adhered to, ensuring that medical practitioners have independent control and oversight of similar robots.
