# BPDI
**Business Process Design and Intelligence:** Knowledge summary and project exercises

Tools used in this course:

<a href="https://woped.dhbw-karlsruhe.de/" target="_blank" rel="noopener noreferrer"><img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171988368-ade3b279-bef9-4fcc-b5c3-7e994de20440.png" alt="" width="128" height="128"></a>
<a href="https://yawlfoundation.github.io/" target="_blank" rel="noopener noreferrer"><img loading="lazy" class="alignnone wp-image-644" src="https://user-images.githubusercontent.com/60782937/171988405-2e66f1f5-1d0d-4911-a91b-d5fed0af3bf5.png" alt="" width="128" height="128"></a>
<a href="https://academic.signavio.com/" target="_blank" rel="noopener noreferrer"><img loading="lazy" class="alignnone wp-image-642" src="http://amin.blogs.dsv.su.se/files/2020/12/signavio.png" alt="" width="129" height="128" srcset="https://user-images.githubusercontent.com/60782937/171988413-e411e58e-e21e-4ffa-9144-9bc02d1e0792.png" sizes="(max-width: 129px) 100vw, 129px"></a>
<a href="https://www.promtools.org/" target="_blank" rel="noopener noreferrer"><img loading="lazy" class="alignnone wp-image-641" src="https://user-images.githubusercontent.com/60782937/171988431-258396fe-d8d0-4ac7-971d-964de796bb06.png" alt="" width="129" height="128"></a>

**Overview:**

Business Process Management Systems (BPMS) are information systems aim to support the business processes in organizations. Business processes describe the organization of work into work tasks, the distribution of work task into different resources and the provision of necessary information for the performance of the individual tasks. In other words, these systems aim to support the administration of work in organizations, and they are configured by process models which are usually graphical。

The course contains the following three elements: Modeling; Analysis; and Enactment.

**Modelling：** Modelling refers to the activity of analyzing a domain (description) from a particular point of view and structuring the outcome in a process model。
There are two sorts of analysis in Business Process Management area, i.e. a-priori and a-posteriori. The focus will initially be on the control-flow perspective, but gradually even the data and resource perspectives will be introduced.

**Analysis:** A-priori analyses refer to the investigation of a business process using a process model. Some techniques enable such analysis like simulation techniques. A-posteriori analyses refer to the investigation of a business process based on data which is generated as a result of enacting the business process. Some techniques enable such analysis - known as process mining techniques. Both types of analyses may lead to process redesign.

**Enactment:** Enactment refers to implementing, configuring, executing, monitoring and adjusting business processes based on defined process model. The enactment can be performed with the help of BPMS. Workflow Management Systems are a sort of BPMS that supports enactment of process models. 

In this course, I have first learnt the basic concepts of Business Process Management, BPM Models and Lifecycle, as well as workflow patterns. Then I learn a business process modelling notation (called Petri nets) that can be used to design executable process models. It has formal definition for syntax and semantics. Thirdly, I use resource patterns to manage business processes using more advanced notation called Yet Another Workflow Language (YAWL). YAWL models can be configured to be enacted and We will see the architecture of a workflow management system. Afterwards, we use a new business process modelling language called Business Process Model and Notation (BPMN) to model our business cases. This notation is widely used in industry to model business processes. Finally, we take a look at how processes can be discovered through process mining automatically and different aspects of process mining like conformance checking and enhancement. We will do it following these steps:

Module 1. Foundations(Workflow Patterns)

Module 2. Petri nets

Module 3. Business Process Enactment (YAWL)

Module 4: Business Process Model and Notation (BPMN)

Module 5. Process Mining


**Module 1. Foundations(Workflow Patterns)**

1. Value Exchange and Business Functions:   ------  2. Business Process Direction:   ------3. Types of Business Process Modeling Languages

<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171991457-6a95ce57-88a8-4472-a0b2-8bf0870190ae.png" alt="" width="200" height="400">               <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171991618-4761b5aa-67f9-426a-b32f-bfb05f054294.png" alt="" width="500" height="380">     <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171991854-d1482da3-5521-401e-b6cd-5ccf276292eb.png" alt="" width="220" height="400">


4. Business Process Modeling Lifecycle:

<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171991833-8b5a9ff7-4ffa-4313-ab6d-9adaf77a57ee.png" alt="" width="800" height="400"> 

5. Aspects in evaluating Business Process: 

   i. Expressiveness: workflow patterns (control, data, resource).
  
   ii. Understandability: comprehension (can use colors, annotations, etc.).
  
   iii. Complexity: Enable comparing models & Improving models.

 
 6. Control-flow Patterns
 
    *Sequence   --- *parallel Split   --- *Synchronoization   --- *Exclusive Choice  ---  *Simple Merge   
    
<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992800-8cdd50c8-95c2-4ffb-aca9-c4a2f7487d9b.png" alt="" width="150" height="50"> ---<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992738-c96c25d7-31ab-4295-b481-477b0f876b9c.png" alt="" width="180" height="50">--- <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992747-60b19fc6-23b7-4694-87f6-0faa66cb19f9.png" alt="" width="180" height="50"> ---<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992757-0e668d4c-2df9-49d5-89e5-3439a08bfa26.png" alt="" width="180" height="50">--- <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992774-f0d93e14-dc61-4f60-a1c5-78db97895bc4.png" alt="" width="180" height="50"> 
    
    *Multi-choice   ---   *Asatructured Synchronoizing Merge  ---  * Multi Merge   ---  * Deferred Choice  ---  *Milestone
    
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992960-a0596301-2d14-4576-9dd7-537520e371c1.png" alt="" width="150" height="50"> ---<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171992977-b1ff5707-f327-4432-b35b-8c6a8c27890b.png" alt="" width="200" height="50">--- <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993002-015b3538-5be1-4bc8-b84c-693cc5760056.png" alt="" width="200" height="50"> ---<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993015-a0c59d00-f136-4669-8cc0-cc9706943587.png" alt="" width="150" height="50">---
<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993317-dda4cbc6-342d-4d10-9dc4-781abf346884.png" alt="" width="180" height="50">

    * Cancel Task  ---  *Cancel Case  --- * Cancel Region  ---- * Arbitrary Cycles  ---* Structured Loop
    
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993550-74ba0f09-371b-4ddc-bf77-a5017f88e888.png" alt="" width="150" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993602-22751e92-7912-4bde-a3ae-518e6819e992.png" alt="" width="150" height="50">--- 
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993625-675d73e2-55ec-48ea-bd61-51fa51c5b8ae.png" alt="" width="180" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993654-97507e14-3071-48a7-9cc6-962d31229709.png" alt="" width="150" height="50">---
<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993669-68845b95-0635-44a7-817a-5eb6f7a3cc60.png" alt="" width="150" height="50">

   *Implicit Terminal   ------ *Explicit Terminal  ------ *Transient Trigger  ------*Persistant Trigger
   
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993843-4fcee20c-9957-4c32-89b7-86f3c5b2c194.png" alt="" width="150" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993858-aa60da6d-2dcd-40e2-a705-4796c0682dbe.png" alt="" width="150" height="50">--- 
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993951-30f2f215-090b-4f92-9348-d1257c2bd424.png" alt="" width="150" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171994005-9da9825a-7995-483a-8453-65277336508f.png" alt="" width="150" height="50">---

7. Measure the complexity
   * NOA: number of activities

   * NOAC: Number of activities and control-flow elements in a process (– Well structured model) include gateways but exclude events

   * NOAIS: Number of activities, joins, and splits in a process (– Non-structured model), include all gateways but exclude events

   * MCC: = edges -nodes + 2 , nodes include events, boundaries,etc.


**Module 2: Petri Nets**

1. Syntax and Semantics

  1.1  Elements:  places (state of system)  <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/172011819-852b2d7d-105c-47c7-b082-6a4f7c8beff6.png" alt="" width="50" height="50">
  transitions (actions / tasks)   <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/172011847-2415e12d-4784-46c0-8396-79df4981f13a.png" alt="" width="50" height="50">
   arcs/ flows (connections)  <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/172011943-ab72451b-8697-457c-90e5-ecf5bbfdbe82.png" alt="" width="100" height="50">

 1.2 Rules:
 
     1.2.1. can connect transactions to places and vice versa. Neither places to places nor transactions to transactions.
     
     1.2.2  Tokens: indicate if a state if fulfilled; represented by dots; places may hold zero or more tokens.
     
     1.2.3  Enablement: a transition is enabled if each of its input place contains at least one token.
     
     1.2.4  Firing: An enabled transition can fire(occur); when it fires, it consumes a token from each input place and produces a token for each output place.
     
 1.3 Remarks:
 
     1.3.1 Firing is atomic.
     
     1.3.2  Multiple transitions may be enabled, but only one fires at a time.
     
     1.3.3 The number of tokens may vary if there are transitions for which the number of input places is not equal to the number of output places.
     
     1.3.4  The state is represented by the disctribution of tokens over places (also referred to as marking)
     
2. Petri Nets - Workflow Patterns

    * Sequence  ---  *Parallelism  --- *Parallelism: AND-Split  ---- * Parallelism:AND-Join  ---* Deferred Choice
    
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993550-74ba0f09-371b-4ddc-bf77-a5017f88e888.png" alt="" width="150" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993602-22751e92-7912-4bde-a3ae-518e6819e992.png" alt="" width="150" height="50">--- 
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993625-675d73e2-55ec-48ea-bd61-51fa51c5b8ae.png" alt="" width="180" height="50"> ---
 <img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993654-97507e14-3071-48a7-9cc6-962d31229709.png" alt="" width="150" height="50">---
<img loading="lazy" class="alignnone wp-image-643" src="https://user-images.githubusercontent.com/60782937/171993669-68845b95-0635-44a7-817a-5eb6f7a3cc60.png" alt="" width="150" height="50">   
     
  








 


