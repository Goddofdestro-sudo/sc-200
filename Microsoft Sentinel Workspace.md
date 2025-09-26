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








