# Optimizing operations using AI: A Roster Automation Solution for SMEs #
<br>
<br>

## Introduction ##
Small and medium enterprises, SMEs, are the base of most economies around the world. According to the Central Statistics Office (2020), in Ireland, SMEs represent 99.8% of all companies and employ 68.4% of the workforce. The hospitality industry has been slow to adopt new technologies, according to Market Scale (2022). In a previous project, we focused on improving communication and information-sharing within the company connecting staff through Kanban boards and instant messages. Building on top of our previous project we would add a new feature to automatically create employee shifts. 
This feature, embedded in our previous software, would help to smooth day-to-day operations, resulting in a save in management manhours, reduce errors, grant a tool for managers to further improve resource allocation and additionally, ensure a fair and equitable scheduling practices what would lead to employee engagement and retention. Later development of the project could include the use of machine learning to choose between teams and help to identify blind spots in training and skill gaps.

## Project Concept ##
Scheduling staff shifts consumes time and resources for managers, often resulting in errors, and miscommunications. These methods make it difficult to adapt to an increasingly dynamic job market. When we consider staff needs, such as work availability and preferences, contractual and legal issues, and skill sets staffing has proven a challenging task.
Managers normally use physical methods such as paper-based systems or spreadsheets to determine the best roster. Despite the existence of staff management applications in the market, these apps are still in the early stages and the adoption rates are slow.
Treating it as a Constraint Satisfaction Problem, our approach would enable users to define both, soft and hard constraints. A CSP can be defined as a set of solutions that complies with a set of constraints regarding a defined domain. This solution provides SMEs some flexibility to get better solutions regarding their specific needs. The challenge of the software is to create a solution able to fit a wide range of possible business cases, from a retail shop where most of the staff knows all the business to a hotel where every member of the staff has different positions. We would address this by creating a series of constraints based on user inputs about the business. 
Later stages of the project could include the analysis of the data to identify skill gaps and offer a service of human resources consultancy through gig-work.

## Business Analysis ##
Porter’s Five Forces analysis
The five forces is a framework for understanding the competitive forces at work in an industry and how the economic value is divided between industry actors. (Harvard, n.d.)
The threat of new entrants into the market is relatively high. The software is relatively simple to create and does not require highly skilled software developers and people with management skills. 
The bargaining power of buyers, primarily SMEs in the hospitality industry, is low. Buyers have the option to choose from various providers. However, most companies do not offer rostering automation services but an integrated human resources platform to manage a multiplicity of aspects.
The bargaining power of suppliers is low. As a software company, we do not depend on complex supply chains, so we should consider as suppliers the staff needed to develop the product. As we established before this stage of the project where we would address roster automation does not require highly skilled developers.
The threat of substitute products is relatively low, mostly due to the nature of the service. While manual rostering methods, such as spreadsheets or paper-based systems, may work as substitutes to a certain extent, they are limited in functionality and efficiency. 
Existing industry rivalry is high, and numerous companies are competing in the market. Competitors include established software vendors, workforce management firms, and startups. We would address this threat with a business model that includes a tier where the customer pays a lower price enough to maintain the infrastructure and get a solid base of users to later advance to other services. Software development is a constantly evolving and changing market but most of our leverage would come from a solid user base and the insides that would give us.
After doing The Five Forces Analysis we believe the project is feasible due to low implementation and operational costs. It is possible to develop and extend the project to cover multiple functionalities for the hospitality sector and to achieve this in stages while getting customer feedback. Future improvements could be modules to help in discovering skill gaps what would help training teams and HR, or modules to implement gig-work and bill the customers a percentage of the salary of those workers.

## MoSCoW Analysis ##
MoSCoW is a prioritization technique for helping to understand and manage priorities in development projects (Agile Business Consortium Limited, 2024). By focusing on must-have features such as automated shift scheduling, employee availability, compliance with labour laws, and a user-friendly interface, the system can deliver most of the value to the customers in the hospitality sector while leaving some room for future improvements.
1. Must-Have:
- It must have the capability to automate the process of generating employee shift schedules based on hard and soft constraints.
- It must provide features to manage and update employee availability.
- It must comply with labour laws and regulations regarding working hours.
- It must have an intuitive and user-friendly interface to help the adoption from managers and employees.
2. Should-Have:
- It should allow users to define and customize soft and hard constraints, such as maximum working hours, minimum rest periods, and skill requirements, to tailor the planning to specific business needs.
- It should provide real-time updates and notifications to staff regarding schedule changes.
3. Could-Have:
- It could have a mobile app to better enhance user experience, though the first stage of the project would be a web app.
- It could include user feedback as a rating system from each employee to collect some extra data for future development.
4. Won’t-Have:
- In this phase the project does not include clock-in/out systems to track employee performance.
- Other Human Resources features as payslips control are out of the scope of the project due to the sensitivity of the data management.
- The model for roster creation will not have any predictive feature due to the complexity of forecasting sales, and the complexity of managing sales data in a software environment.
- The development of custom employee training is not part of the project due to time constraints.
- It will not integrate machine learning algorithms to analyse historical scheduling data and skills to provide recommendations for rostering.

## Technology Overview ##
Our previous piece of software was made using React.Js for the frontend, C# and .NET core 6 for the backend, and Microsoft SQL as the database management system. The decision to utilize Microsoft technologies was to lower potential compatibility issues and the intention of deploying the whole system using Azure cloud service. This choice was driven by the preference for exploiting Microsoft's tools and services, including access to complete and well-written documentation.
For this feature, we opt for Python as the preferred backend technology due to its extensive repository of open-source libraries and strong community support. Python's ecosystem is beneficial for data applications, with specialized libraries tailored for constraint satisfaction problems available. While the feature could be implemented using C#, the absence of CSP libraries would take the development of a custom solution. However, given the constraints of time and expertise. The biggest challenge of this solution would be to integrate both systems, we would approach the issue by using containerization.
The decision to keep React.js for frontend development instead of plain JavaScript is due to its component-based architecture, which allows for code modularity and reusability. Additionally, the availability of component libraries, such as Material UI, contributes to speeding up development by offering pre-built components. Furthermore, React.js's adaptability enables seamless migration to React Native for mobile application development, ensuring platform consistency across web and mobile environments.

## Legal and Ethical Issues ##
Ensuring legal and ethical compliance is paramount in the design and implementation of rostering automation systems. One must navigate complex data privacy regulations, such as GDPR to protect employee data from unauthorized access and breaches. Additionally, adherence to labour laws is essential to ensure appropriate scheduling decisions to ensure fair treatment of all employees and minimize bias.
Furthermore, transparency and accountability mechanisms should be established to provide employees with insights into how scheduling decisions are made, fostering trust and confidence in the system. By prioritizing legal and ethical considerations, organizations can create rostering automation systems that not only enhance operational efficiency but also uphold the rights and well-being of their workforce.

## Data Collection ##
To acquire the data necessary for the rostering system, a multifaceted approach will be adopted, integrating employee registration and onboarding processes with the existing HR system. During registration, employees will be prompted to provide essential details, including personal information and contact details safeguarding employee privacy rights. In a future stage of the system, it is possible to collect data such as skills, experience, and performance of the staff, and to use that data to further improve the rostering and to get extra insides or recommendations for business.
However, it is imperative to adhere to the principle of data minimization, collecting only the necessary personal data required. Further data is necessary to create the rosters such as work preferences, availability, and minimum and maximum working hours in the contract.
