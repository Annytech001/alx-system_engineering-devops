
A postmortem is a systematic review or analysis conducted after a project, event, or process has concluded, especially if it didn't go as planned or if there were notable successes and failures. The purpose of a postmortem is to assess what worked well, what didn't, and what lessons can be learned for future endeavors.

In various contexts, such as software development, project management, or business operations, postmortems help teams reflect on their performance, identify areas for improvement, and implement changes to enhance future outcomes. They typically involve gathering feedback from team members, stakeholders, and relevant data sources, and then synthesizing this information to draw conclusions and actionable insights. The ultimate goal is to foster continuous improvement and avoid repeating mistakes

![Incident mangament  2 Medium](https://github.com/Annytech001/alx-system_engineering-devops/assets/117596977/ea8648b0-12da-40a3-a2e2-43c85b50286a)


Summary 
On 3rd December 2023 at 6:30pm  our OLT terminal  experienced an unexpected outage that lasted approximately 8hours. This outage resulted in a whole city downtime, including dedicated links.  This postmortem aims to analyze the incident, identify the root cause, and propose corrective and preventative measures to mitigate similar incidents in the future.

Timeline:
6:30pm: we observed some logs indicating downtime on our monitoring system.
6:35pm: Users reported inability to access the internet 
6:37pm: On-call engineers were alerted and initiated an investigation.
7:40pm Initial Troubleshoot indicated there was a lost of signal 
9:30pm Further investigation revealed a Fiber cable cut 
9:35pm Engineers deployed to rerun cable 
11:35pm Slippers  were deployed to restore the signal.
1:30pm  Signal was restored and the internet was back.
Root Cause:
The root cause of the internet outage was identified as loss of Signal(LOS) as a result of Fiber cut.  During routine maintenance conducted earlier, Fiber cable was rerun ( 12 core ) and spliced.

Resolution:
To restore service, engineers rerun the damaged cable and splice back for signal to flow 

Corrective Measures:
Use another route for the cable to avoid damage.		
Control procedures with appropriate approval mechanisms.
Enhance documentation related to signal level ensuring the get a good signal 1db.
Schedule regular checks of the  system to identify and rectify any discrepancies proactively.
Preventative Measures:
Implement automated monitoring and alerting systems to detect anomalies in the signal
Establish redundant failover mechanisms to mitigate the impact of similar incidents in the future.
Conduct regular training sessions for operations and maintenance teams to reinforce best practices and ensure awareness of potential risks.
Develop a comprehensive incident response plan with clear escalation procedures and roles/responsibilities defined for all team members.
By implementing these corrective and preventative measures, we aim to enhance the resilience and reliability of our signal level, minimising the risk of future outages and ensuring uninterrupted service for our users.

