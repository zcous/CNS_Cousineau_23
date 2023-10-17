# CNS HW6 - 1/c Zoe Cousineau 19Oct 2023

## Splunk Course - Intro to Splunk

  The Introduction to Splunk gives the learner a overview of what Splunk is and how they could use it for their company or organization. The Splunk enterprise has three roles: Admin, Power, and User. The Admin can install apps, adjust data, and create knowledge objects. The Power role is one step down, being able to create and share knowledge objects and perform real time seraches. The lowest privledge is the users, who can only see their own knowledge objects. The home interface allows you to find documentation, and use the splunk tools. The interface is very easy to use, with a well designed GUI and easy to use menus and searching tools. The search tools is powerful for monitoring systems. You can search by terms, like failed searches to see who has been trying to gain access. If you know the IP of the attacker or name, you can also search by name or IP. When you search, you will be provided with extra information about the event with the time and date, showing the newest events first.  You can also use AND, OR, or asterics to widen or narrow searched based on what you hope to search. After you search, you can use commands to make charts and statistics, making this a helpful tool for organizations to see the data they are being presented. Commands are followed by functions, arguments, and clauses. These come after the search terms and a pipe. These are not case sensitive! Splunk will be slower the more data you have to retrieve, so filtering more might be helpful! Filtering early makes so that Splunk has to retrieve less events! Knowledge objects help you discover and analyze data. There is data interpretation, classification, enrichment, normalization, and models. If we want to save and share searches, we can generate a report. Additionlly, you can create dashboards, where you save multiple visualizations to. This way the team can see all the visualizations at a time to see the full picture on one page. You can share this with others easily! There are classic dshboards and dashboard studio. Dashboard studio is a more visually pleasing version of dashboard, allowing you to customize how each visualization looks. Overall, Splunk is a great tool to monitor a network and show less tech savy people what is going on with visualizations. 

Here's my cool certificate!
  ![Certificate](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW6/CousineauCertificate.pdf)

## Windows Event ID - 4608
  I decided to black list the Windows event ID 4608 because this event indicates that Windows is starting up. I would not deem this even necessary when looking into a system for possible attacks because it does not indicate that any sort of attack is going on. This would also declutter the events I would be looking at, making it easier to find the possible malicious actors in the system. 

  My inputs.conf file in my SplunkUniversalForwarder/etc/system/local folder, as pictured below:

![inputs.conf file](![image](https://github.com/zcous/CNS_Cousineau_23/assets/90362066/0d3e2f4e-d42a-4763-955e-cb57381144cd)

## Take Aways
  Overall this was a great Homework, I enjoyed getting to pick what I wanted to learn and what I wanted to block with my team. This the modd for this week, since it was super busy with two big papers, big capstone work, and leaving for two days for a glee trip!!

![today be like](https://github.com/zcous/CNS_Cousineau_23/blob/main/HW6/meme.png)

  


