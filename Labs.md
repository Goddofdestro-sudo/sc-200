**Creating Defender for Admin ROle**
1. Go to Permission Tab on Defender portal.
   
   <img width="270" height="258" alt="image" src="https://github.com/user-attachments/assets/bab404b1-7b4e-47dd-bb50-d1872160e085" />
3. Select Custom role
<img width="783" height="397" alt="image" src="https://github.com/user-attachments/assets/742e6ced-d70b-4b5d-9f80-c89cc51127b0" />
3.Fill in the Basic.
<img width="675" height="385" alt="image" src="https://github.com/user-attachments/assets/13250d0d-e3e4-4fac-ad0f-9cd72d660aa5" />
4. Under permission, select each permission group and configure as neeed.
   <img width="604" height="600" alt="image" src="https://github.com/user-attachments/assets/75582e25-9f0a-4ff4-b382-00ec6e2f8f18" />
  <img width="578" height="475" alt="image" src="https://github.com/user-attachments/assets/0dd442cd-8b50-4e00-b8f3-49fd34fa5325" />
  <img width="615" height="778" alt="image" src="https://github.com/user-attachments/assets/83fbdefb-345f-4a10-81fe-f5efdab83c06" />
  5. Now create and Assignment, select the scope and assign it to the dedicated users.
<img width="621" height="560" alt="image" src="https://github.com/user-attachments/assets/9ba6fe31-bcfc-438a-b99d-988f2a50854e" />


-** Now when we are onboarding a device to Defender for Endpoint.**
- EIther you can onboard using script for few devices.
- Settings>Endpoint>Onboaridng>script
  <img width="775" height="1585" alt="image" src="https://github.com/user-attachments/assets/833b2eaf-5048-40b3-819a-35842ecf5b31" />
  But if we are onboarding a large devices as in a corporate scene where the device are mostly managed by Intune, then.
  1. Firstly we need to create a sync between Intune and DEF
  2. Security>Settings>Endpoint>AdvanceFeature> Turn on Microsoft Intune Connection.
     
  <img width="798" height="1214" alt="image" src="https://github.com/user-attachments/assets/07df834f-da3f-473c-b0bd-6e1d7e57a7a7" />
Now, on Intune navigate to Intune> Endpoint security and configure the settings. Also, we can create a sepreate on boarding policy
Endpoint for security> Endpoint Detection and Response
<img width="769" height="1474" alt="image" src="https://github.com/user-attachments/assets/0cc463a1-a6f9-4941-b3ec-3a9967f002a2" />



     




