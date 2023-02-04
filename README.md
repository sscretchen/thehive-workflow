# TheHive Workflow

Using TheHive to show multiple workflows with the platform

### Open Tasks

- [ ] Visio flowchart for *Playbook* implementation

---

### The Workflow

💡 There are two ways I use with TheHive

1. Manual input for building cases
2. Using established playbooks

---

### Manual Execution
> An on the fly approach to building cases

#### STEP 1

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/213080165-ea6aa1e6-3fcd-4f4f-a83f-8c681dd2ef7d.PNG" style="width:auto" height="auto">
</p>
The main panel view for the user. I use this area to track any cases assigned or created myself. I will have more information to show as I build out a simulated case.

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/215211798-87e01701-8a8e-47b9-83d9-87bbd63e8855.PNG" style="width:auto" height="auto">
</p>

To get things started, click on `+ New Case` at the top. From here, the details of the case will be outlined. A few key points:

- TLP (Traffic Light Protocol) - This functions as an Access Control for sharing information. Depending on the sensitivity of the incident, you may need restrict who can share incident details.
- PAP (Permissible Actions Protocol) - Indicates how to use IoCs while investigating. This involves taking a passive or active response on the IoC.
- Tags - This is a minor detail but I think it can act as metadata for future analysis. I would just be weary of adding too many tags or this field becomes moot.

I will add tasks later in the process. The important part is capturing the case details as quickly as possible. Once that is done, hit `+ Create Case`

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/215212639-f1f64f36-64cc-4379-92b6-4178acdc6985.PNG" style="width:auto" height="auto">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/215214191-bca5007b-234b-438d-8b70-ee0ebd947c89.PNG" style="width:auto" height="auto">
</p>

Case view. The next step is to add tasks releated to this incident.

***

#### STEP 2

When adding tasks, I want this to be based on established procedures from an incident plan or playbook. In this demonstration I will focus on the triage & collection of artifacts. Once in the main Case view, click on the Tasks tab and start `+ Add Task` activities.

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/215215469-76855f32-e3fa-4fd4-a3ce-0cd9ed44348a.PNG" style="width:auto" height="auto">
</p>

Once the task is assigned, the user can now start their response. First step would be to click the ▶️ button so the response time can be recorded.

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/213080171-d9c5f845-af98-4667-8ffd-e05632a4713f.PNG" style="width:auto" height="auto">
</p>

***

#### STEP 3

The scope of performing incident response is beyond the simple documentation here but I have included a sample log that a user can put in their assigned case such as identifying affected workstations. The important thing to remember with Incident Response is there are established guidlines that can be followed. guidelines such as the four NIST Incident Response Steps:

1. :blue_book: Preparation
2. :mag: Detection and Analysis
3. :gun: Containment, Eradication and Recovery
4. :adhesive_bandage: Post-Incident Activity

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/213081956-999da5af-d83d-4463-bd5c-e7905cd5b25e.PNG" style="width:auto" height="auto">
</p>

---

### Playbook Execution
> Critical incidents may call for a more thorough approach. This demonstration will use established playbooks and map any identified TTPs to the MITRE ATT&CK framework. This will be done by creating Case Templates

#### STEP 1

<p>
  This <a href="https://github.com/austinsonger/Incident-Playbook/">GitHub project</a> is a good source for existing playbooks because it hosts a series of catalogs that cover multiple areas of Incident Response.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/216750456-992df46c-3b32-481e-88b2-1babf4f41fea.PNG" style="width:auto" height="auto">
</p>

Admin rights are needed to create case templates

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/216750618-2d44bda0-2066-4a96-9969-a2c59f591ece.png" style="width:auto" height="auto">
</p>

Case tempalte view. Here I will begin to outline the Case Details. I will use similar options from the manual demonstration for consistency. That MISP template will come into play later. That is an OSINT Threat Intelligence platform.

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/216750947-0cf6ca57-07df-4b77-a6be-759cc5fc4ae3.PNG" style="width:auto" height="auto">
</p>

Similar to the manual case, I will add details such as the severity and permissions. This template covers the MITRE technique `T1486` 💡 <a href="https://attack.mitre.org/techniques/T1486/">Technique Details</a>

<p align="center">
  <img src="https://user-images.githubusercontent.com/54426511/216752314-0f3358ed-455b-46bd-8821-444717796d4f.png" style="width:auto" height="auto">
  <img src="https://user-images.githubusercontent.com/54426511/216752100-69baf612-6973-4c25-ba82-1b86969559cd.png" style="width:auto" height="auto">  
</p>

First task is in, but a playbook isn't doing much without actionable items. So I will break this down further with a focus on the investigative tasks of response. The Task Group has also been isolated. You may be responsible for other areas such as Remidiation, or Eradication, but you cant do any of that if you dont know what your looking for 🕵️

*The main tasks of this template:*

1. Determine the type of ransomware
2. Determine the scope
3. Assess the impact to prioritize resources
4. Find the infection vector

---to be continued---
