**Creating Log analytics workspace.**
Create a resource and provide the name for the LAW.
<img width="840" height="711" alt="image" src="https://github.com/user-attachments/assets/9a6d963e-abb6-4166-98b4-9b2f17cc13e4" />
<img width="745" height="555" alt="image" src="https://github.com/user-attachments/assets/70c75136-07ec-4e42-9954-e81db43b7ad3" />
Once LAW has been create, navigate to sentinel and add the LAW to the sentinel.
<img width="1060" height="1641" alt="image" src="https://github.com/user-attachments/assets/cc0ef01d-286c-4c7f-946d-87ee258323c1" />

**Configuring log retention**
- Navigate to settings>Table>select a log and click on the 3 dots.
<img width="1002" height="200" alt="image" src="https://github.com/user-attachments/assets/8dc96474-1805-4430-ab7f-b6fdab570c5b" />
- As needed you can configure your logs for real time analytics and archiving.
<img width="798" height="1047" alt="image" src="https://github.com/user-attachments/assets/5a3b2acd-bc91-4c28-84d7-883e0ba2e0b0" />

**Injesting DataSource to Sentinel**
In order to start injesting logs to your sentinel using various data connectos. You will need to connect your LAW to defender XDR.
Navigate to Defender and under Sentinel> Content Management>Content hub, select your workspace and connect it to the XDR.
<img width="1068" height="1046" alt="image" src="https://github.com/user-attachments/assets/140e0f53-327a-45bb-bfd6-a3a9d6420dcb" />
<img width="1018" height="315" alt="image" src="https://github.com/user-attachments/assets/462f1cb8-cd94-47f2-aecc-7ed981217793" />
<img width="888" height="327" alt="image" src="https://github.com/user-attachments/assets/b3e13e50-458a-4cfa-9340-e68d78c09b70" />
<img width="970" height="1651" alt="image" src="https://github.com/user-attachments/assets/735d6f7e-eb12-4dca-b766-72d161613bf5" />
Once the workspace has been connected to the XDR, navigate back to the sentinel in azure and under content hub, you can select the different Microsoft plus 3rd party connectors.
<img width="1046" height="1652" alt="image" src="https://github.com/user-attachments/assets/5717c249-76c4-4e59-8e57-4a6d8e305bf1" />

Select the connector and install,
<img width="1079" height="1607" alt="image" src="https://github.com/user-attachments/assets/4ee39522-afe5-4bc3-9a7e-593b476943ed" />

**Data Collection Rule**
Once the connectors are connected to the sentinel, you will need to create data collection rules to deteremine how data are collected from various sources like AMA, Fordwarded events, DFI,DFC etc.

<img width="1909" height="879" alt="image" src="https://github.com/user-attachments/assets/2ce6ed51-acac-41ac-bfda-24d51891866a" />

1. Creating a DCR. Navigate to Data connectors and open the data connector. Configure the DCR.
   <img width="1905" height="885" alt="image" src="https://github.com/user-attachments/assets/297f12e8-25da-4224-a161-84a3c9a0f56e"
   2. Select the resources and configure the type of collection.
   
     <img width="837" height="488" alt="image" src="https://github.com/user-attachments/assets/a6fd8ad6-f422-4a87-be6e-2fb04035ae30" />
     <img width="505" height="184" alt="image" src="https://github.com/user-attachments/assets/a4354e19-75fe-45ed-bb26-e8bdbd544380" />
     <img width="820" height="569" alt="image" src="https://github.com/user-attachments/assets/2bbdddba-2578-4228-8a21-24c7f3473149" />

**Creating a custom log tables to store ingest data.**
1.Navigate to LW and go to tables.
2. Create a customtbale based on DCR.
<img width="764" height="390" alt="image" src="https://github.com/user-attachments/assets/224912a6-4812-41e3-a2ed-a648ead4dd91" />
3. Before we can create a custom table, we will need to create a custom data collection endpoint.
Navigate to azure monitor and then, go to Data collection Endpoint
<img width="1087" height="893" alt="image" src="https://github.com/user-attachments/assets/05a7a600-c14a-4ad0-9986-cb80a823bd23" />
4. Once created, navigate back to table and create the custom table.
<img width="930" height="688" alt="image" src="https://github.com/user-attachments/assets/9aaad698-6f2e-48b8-979e-bab31a60f0bf" />
5. Download and upload a custom log.
<img width="1636" height="890" alt="image" src="https://github.com/user-attachments/assets/ceb65f27-06bf-4977-9d5e-305ebc1cf529" />
Once created you should be able to see the custom rule.
<img width="1919" height="888" alt="image" src="https://github.com/user-attachments/assets/4d07a7e4-8bee-435e-af85-f9757ee268c4" />









     

   














