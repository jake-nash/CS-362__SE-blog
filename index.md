# SE blog

 
 
 

#### HW0: Introduction

Hi, I'm Jacob Nash, a junior at CofC. This is my second attempt at getting a degree, so far it's going better than the first try. I'm enjoying learning new things again. I work as a math tutor, so if you need help in any math class feel free to reach out; my email is nashjr@g.cofc.edu, and my phone is (843) 847-1338.





#### HW1: Chapter 1

_1.3:  What are the four important attributes that all professional software should possess? Suggest four other attributes that may sometimes be significant._

Ans: Acceptability, Dependability/Security, Efficiency, and Maintainability. I also think that all software should be economically feasibile (can be made within a pre-defined budget), ethically sound, unintrusive (concerning users' private information), and, to some extent, future-proof (this is obviously not guaranteed, but software should continue to receive support/maintainence while it is still in use).

_1.8:  Discuss whether professional software engineers should be licensed in the same way as doctors or lawyers._

Ans: I think that it would be very difficult to create some license that would certify that a software engineer is qualified to work on software; as the book mentions repeatedly throughout chapter 1, software can take on many different forms, each with their own set of necessities and priorities. The license would either be far too specific, requiring all software engineers to be proficient in engineering all possible types of software, or it would be so broad in scope that licesure would not convey any sense of certification because of the lack of specific skill/knowledge checks. 

_1.9:  For each of the clauses in the ACM/IEEE Code of Ethics shown in Figure 1.4, propose an appropriate example that illustrates that clause._

Ans:
PUBLIC - a software engineer should not create software to exploit users' personal data, as this is in no way to the public's interest.
CLIENT AND EMPLOYER - a software engineer should strive to create software that meets or exceeds their client's/employer's specifications.
PRODUCT - software engineers should take pride in their work and ensure that their software is (at least) acceptable, dependable/secure, efficient, and maintainable.
JUDGMENT - software engineers must use thier good judgement to ensure the integrity of their efforts and of the finished product.
MANAGEMENT - anyone managing software engineers should be sure to promote (and themselves follow) professional and ethical work standards.
PROFESSION - software engineers should consider how their actions reflect on the practice of software engineering, and strive to uphold the professionalism of the job.
COLLEAGUES - all software engineers should treat colleagues as equals.
SELF - a software engineer should be dedicated to improving their skills and knowledge of the craft for as long as they practice it, while holding themselves to the ethical standards put forth in the ACM/IEEE-CS code of ethics.

_1.10: To help counter terrorism, many countries are planning or have developed computer systems that track large numbers of their citizens and their actions. Clearly, this has privacy implications. Discuss the ethics of working on the development of this type of system._

Ans: In many ways, creating/maintaining software like this (or in practically any military use) would require the individual to ensure that they follow their own personal ethical values first and foremost. Everyone's personal ethics on military action (even in the "preventative" sense) differ; their is no common answer to the ethicality of such actions. I feel that it would be the responsibility of all parties involved to regularly and often check the ethicality of what they are working on, in order to be sure that no lines have been crossed; any software engineers involved in such a project should know where that line is, for them personally, and respect it.





### HW2: Reflections on Software Engineering Practices

I think that the biggest commonality between all three of the readings was that software development has become more and more complex through the years, and shows no signs of becoming simpler due to ever-increasing and ever-changing demands of software. The first article (“No Silver Bullet”) surprised me as a reader, because I would have thought that a computer science article from 1986 couldn’t possibly be relevant today—in some ways, I do feel that it was obsolete (the specific technologies and methodologies for designing and coding software have in some ways changed), but at the same time some of the information was still relevant. I would say the two most interesting ideas of this article were the ideas that (a) software is essentially complex, and there is no way to address that inherent complexity, and (b) that software is essentially abstract, and difficult/impossible to model graphically. The author gave no proof that either of these traits are in fact essential to software, and I’m not sure that I agree with those assumptions; yes, graphical depiction of many concepts is difficult, but I feel that is no more the case than for other sciences, and yes, software is typically quite complex—but is it inherently so? I would like to see some sort of demonstration (not even a formal proof) of these ideas, and I think it would be interesting to contact this author today to ask his thoughts now on this article he wrote in 1986. The second article, which was really more of an advice column, didn’t really offer much new info to me. It addressed specific problems from two individuals, and I think that it was relatively good advice, but I don’t think it was very generalizable to all of software engineering. My most useful takeaway from this article is that people should always be comfortable to ask questions, and that doing so indicates a desire to improve; I also liked the idea that computer science is indeed a science, and therefore the scientific model is applicable. The last article, about Google’s giant codebase, was very interesting to me and also made me think about some aspects of software engineering that I haven’t before. Since I am now learning about Git and VC software in general, I was surprised to read that Google, one of the largest software companies on the planet, does not use Git or some other distributed VC; the reasons put forth in the article now make sense, but I was still surprised to read that after just learning about the advantages of Git. The enormity and complexity of managing Google’s codebase was impressive to read about, and also made me consider the idea of software designed and used specifically for managing other software—this sort of “meta” software development sounded useful, certainly, but also I think very difficult. To some extent I was already aware of this idea (essentially, an OS is a piece of software meant to manage the flow of control between the user and different softwares); but the idea of creating a software (eg Piper) so that it could be used at such a large scale, and then on top of that creating a software (eg Clipper) to help manage and control and simplify the other software that had just been created, seems very complex to me, not the concept but the actual practice of it.





#### HW3: Chapters 11 & 12

_11.4:  What is the common characteristic of all architectural styles that are geared to supporting software fault tolerance?_

Ans: All of the architectures to support fault tolerance use a diverse array of software to test the system, so that two different system checks would be unlikely to fail in the same way.

_11.7:  It has been suggested that the control software for a radiation therapy machine, used to treat patients with cancer, should be implemented using N-version programming. Comment on whether or not you think this is a good suggestion._

Ans: I don't think this is necessarily the best option, because it would be very expensive to build N versions of the software; I think it would be better to use a protection system.

_11.9:  Explain why you should explicitly handle all exceptions in a system that is intended to have a high level of availability._

Ans: In order to prevent an exception arrising that would cause the system to fail; if all exceptions are handled, then all possible (software level) errors are explicitly dealt with.

_12.5 A train protection system automatically applies the brakes of a train if the speed limit for a segment of track is exceeded, or if the train enters a track segment that is currently signaled with a red light (i.e., the segment should not be entered). There are two critical-safety requirements for this train protection system:_ 
>1--The train shall not enter a segment of track that is signaled with a red light.

>2--The train shall not exceed the specified speed limit for a section of track.

_Assuming that the signal status and the speed limit for the track segment are transmitted to on-board software on the train before it enters the track segment, propose five possible functional system requirements for the onboard software that may be generated from the system safety requirements._

Ans: (1) The software will check track status once per second. (2) The software will check train speed once per second. (3) The train's speed will be compared to the track's speed limit every time the train speed is checked. (4) If train speed exceeds speed limit, software will apply train brakes until speed is 5mph less than limit. (5) If track status indicates a red light, brakes will be applied until train comes to a full stop.





#### HW4: Reflections on software failures

In reading chapters 11-14, which discuss the reliability, safety, security, and resiliency of software, as well as all the other supplemental readings, my biggest takeaway is that no one really knows the best way to make software; or at least, no one has a methodology figured out for creating software that will be reliable, safe, secure, and resilient. I’m not saying that there isn’t good software out there, or that the people who made it just got lucky; I understand that by the nature of this, good software can’t really be reported on in the same way that faulty software can. That being said, there were so many high-profile failures across so many decades, that I’m left astonished. Surely, the reason for this must be the relative youth of software itself, which began complex and has also only grown more complex since the start. Several times, in the book and in some of the readings, it was mentioned that there are so many possible paths that software can take that it would be impossible to even list them all, let alone understand them all. It’s kind of strange to me that software, which (again, repeatedly mentioned) is purely thoughts and ideas, would be the most difficult aspect of many system engineering projects to master. It also is kind of logical, since the process of thought and creation has been the hallmark of humanity even back to history’s earliest philosophers. I think that it must be this intangibility of software that makes it so complex and challenging to master. On this note, I think that formal mathematical modelling and proofs of software would be incredibly useful to all software engineers, because it would take the abstract and immaterial and make it both visual and codifiable. The book mentions the idea of formal modelling many times, in discussions of safety as well as security and even simply correctness, but spends very little time discussing it; each time it mentions it, it says that there are some advocates of it, but that it is too difficult for people to learn. While I have absolutely no experience whatsoever with the topic, it seems very foolish to me to dismiss something so potentially valuable because it is hard to understand. After all, the focus of many of the readings (besides discussing the specifics of whatever event they were describing) was to say that software engineering is far too complex to be done without using incredibly specific oversight and checking and rechecking. This is already clearly a very complex area of study, and so I think that it would be worthwhile to learn something that could help with the process, even if that something is very mathematical and potentially hard to learn. On another subject, I think the textbook could be more useful than I first thought it would be. It seemed to me that the first many chapters I read were so general, in order to be applicable to any type of software engineering, that they said basically nothing. However, reading specifically chapters 13 and 14 I was able to see the usefulness of what the author was saying—yes, sometimes it was still very general, but I also saw the wisdom in the advice it gave (most notably on resilience, and the discussion of how resilience means different things for different software, and how to decide what attributes take priority).





#### HW5: Chapter 4 and reflections
 
_4.5) Using the technique suggested here, where natural language descriptions are presented in a standard format, write plausible user requirements for the following functions:_
>An unattended gas pump system that includes a credit card reader. The customer swipes
the card through the reader, then specifies the amount of fuel required. The fuel is
delivered and the customer's account debited.

>The cash-dispensing function in a bank ATM.

>In an internet banking system, a facility that allows customers to transfer funds from one
account held with the bank to another account with the same bank.

Ans: (a) Function: charge customer for gas delivered. Inputs: card info, gas amount. Outputs: gas delivered, customer card charged. Action: customer card info found using card swipe, customer account charged for fuel amount * price per unit. Fuel is output up to the amount the user has paid for. When user indicates end of fueling, price of remaining unused fuel reimbursed to user card; receipt printed. (b) Function: dispense cash from ATM and subtract amount dispensed from user account. Precondition: customer account accessed and open. Input: amount of cash desired. Output: cash delivered, sum taken out of user's account. Action: Check desired amount against current account balance. Dispence cash in multiples of $20, not to exceed $500. (c) Function: transfer funds between separate accounts within the same bank. Inputs: account to draw funds from, account to give funds to, amount of funds. Precondition: both accounts are valid accounts within the same bank, and fund ammount does not exceed balance of account to draw from. Outputs: funds transfered, user given confirmation message of transfer. Action: check that both accounts are valid and that transfer ammount does not exceed balance of account to draw from. In both accounts, leave a record of the transfer (date, time, ammount, account to/from #). Inform user that funds have been transferred.

_4.6) Suggest how an engineer responsible for drawing up a system requirements specification might keep track of the relationships between functional and non-functional requirements._

Ans: Start by writing non-functional requirements, and number them. Every functional requirement generated from a non-funtional requirement is numbered as a sub-item of the non-functional requirement (ie 1.1, 1.2, etc).

_4.7) Using your knowledge of how an ATM is used, develop a set of use cases that could serve as a basis for understanding the requirements for an ATM system._

Ans: Case 1: deposit money; case 2: withdraw money; case 3: check balance; case 4: maintence/repair/stocking of ATM; case 5: can be used as an emergency phone

##### Reflections on reading: 

I thought that all of the articles/reports dealing with security issues were interesting, especially the report on TPMSs and their vulnurabilities. I had never considered that something so basic and ubiquitous could be used for any sort of purpose. Obviously the researchers were trying to highlight that all future wireless signals in cars could be just as vulnerable if changes aren't made, but even the things they thought of that could be done with just this information! Tracking people, issuing fake tire alerts to make someone stop their vehicle, I never would have thought of those. It made me very glad to know that some people are trying just as hard to protect everyone as other people are trying to steal from/extort the general populace. Separately, I thought the idea of test-driven development was a good idea as far as making sure code is tested thoroughly, but I also thought the author of the article was overzealous in showing its usefulness. And lastly, I thought the idea of the short-term memory limits was interesting but not terribly applicable to this class.





#### HW6: Chapter 2

_2.1:  Suggest the most appropriate generic sofware process model that might be used as a basis for managing the development of the following systems. Explain your answers according to the type of system being developed:_

> A system to control the antilock braking in a car

> A virtual reality system to support software maintainence

> A university accounting system that replaces an existing system

> An interactive travel planning system that helps users plan journeys with the lowest environmental impact

Ans: I think that the waterfall methodology would be best for the ABS system in a car, because ABS is a safety-critical system. The waterfall model requires a lot of formal planning and requirement validation before the system design begins, which is a desired quality when creating safety-critical software. For the second system, while I don't quite understand how a VR system could support software maintainence, what I know of VR and of software maintainence seems to best support incremental development; this would allow the core functionality of the system to be implemented from the start, and subsequent user input can address new/less important functionality. For the third system, since the new accounting software needs to replace the old system, I think that an integration/configuration mehtod would be best; that way, as long as the new system is compatible with the old system, then the old system doesn't have to be replaced all at once, it can instead be "phased-in" as each part of the software is finished. Finally, I think the last system should be designed using the incremental development model. While there is a core functionality that is defined ("journey with lowest environmental impact"), the word "interactive" to me seems vague, so probably, after using the system in its base version, users would change what they wanted "interactive" to mean, and so an incremental/agile development process would save the cost and expense of re-doing the system requirements and validation that would be needed if the formal waterfall methodology was used.





#### HW7: Chapter 5 and 6

_5.3: You have been asked to develop a system... planning large-scale events and parties.... Using an activity diagram, model the process context for such a system that shows the activities involved in planning... and the sysem elements that might be used at each stage._

Ans:
![5.3 diagram](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/5.3%20diagram.png)

_5.5: Develop a sequence diagram showing the interactions involved when a student registers for a course in a university._

Ans:
![5.5 diagram](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/5.5%20diagram.png)

_5.7: Based on your experience with a bank ATM, draw an activity diagram that models the data processing involved when a customer withdraws cash from the machine._

Ans:
![alt text5.7 diagram](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/5.7%20diagram.png)

_5.8: Draw a sequence diagram for the sae system \[as in 5.7\]. Explain why you might want to develop both activity and sequence diagrams when modeling the behavior of a system._

Ans:
It could be useful to create both activity diagrams and sequence diagrams since data-flow diagrams highlight the operations or activities, while sequence diagrams highlight objects in a system. Nonexperts tend to favor data-flow diagrams, whereas engineers tend to favor sequence diagrams.
![5.8 diagram](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/5.8%20diagram.png)

_6.4: Draw diagrams showing a conceptual view and a process view of the architectures of the following systems:_

> A ticket machine used by passengers at a railway station.

> A computer-controlled video conferencing system that allows video, audio, and computer data to be visible to several participants at the same time.

> A robot floor-cleaner that is intended to clean relatively clear spaces such as corridors. The cleaner must be able to sense walls and other obstructions.

Ans:

![Ticket machine](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/6.4%20diagram%20(a).png)

![Conferencing software](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/6.4%20diagram%20(b).png)

![Floor cleaner](https://github.com/jake-nash/CS-362__SE-blog/blob/gh-pages/6.4%20diagram%20(c).png)





#### HW8: Mythical Man-Month

In reading chapters 1-4 of [The Mythical Man-Month], I was most clearly struck by the author’s clarity and conciseness in expressing his ideas. I looked up the publication date several times because I couldn’t believe that it was as old as it was, and also as informative as it was. Surely, not everything he talked about is still terribly relevant (I’m sure companies have realized that throwing more people at a software project doesn’t finish the work faster, as it might in other engineering disciplines), but to me, as a novice in this area, I felt like I gained a lot of knowledge from a very short reading. I think that the (presumed) focus of our reading, the idea that more manpower ≠ less time, was pretty straightforward. At the time of his writing these essays, probably many managers didn’t understand this, especially if they had some experience in another engineering field. I thought that his advice seemed rather pertinent, and it seemed that much of his advice came from personal experience/mistakes, so it also rang true. Most fascinating to me was the idea of the “surgical team” organization of a programming team (and relatedly, his cathedral/architectural analogy in chapter 4). Largely, I thought this organizational idea was brilliant. Note that, before I say more, I don’t really know anything about this field, so all of this is my own opinion. That being said, the idea that everyone in the team should specialize into a specific aspect of the software creation seems very efficient and organized to me; it’s like a miniaturization of the way most all of life (but especially professions) have specialized  in order to maximize efficiency. I would really like to learn (and I plan to look up) whether this has been implemented before, and if so how well it worked. However, if I had to say something against this organizational structure, I would ask why it hasn’t been widely adopted. I’ve never heard of this idea before; surely, if this idea was put forth in/before 1975, and this book is widely read, people would’ve tried this idea before, and if it had worked others would have copied them. But again, I’ve never heard of it, so probably people have tried it and it didn’t work very well. I would think that the hardest part would be finding a capable enough “surgeon”, and also finding other programmers who would be willing to merely assist him/her instead of also contributing code. Lastly, to relate back to his idea of designing a building, I think that there should be one person (or a very small few people), the architect, who at the end of the day gets the final say how things should go. It relates back to the idea of the surgical team, in that there is a very clear hierarchy of command, and all issues are resolved by the same person. In this way, the architect can keep a tight hold on the conceptual integrity of the project, which was mentioned repeatedly mentioned as being important to the overall success of the software. 





#### HW9: Chapter 8 and reflections on testing

