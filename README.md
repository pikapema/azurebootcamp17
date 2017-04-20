# azurebootcamp17
Instructions for serverless lab:

Steg 1: Skapa ett (gratis) twilio konto och lägg till ett nummer.
Steg 2: https://channel9.msdn.com/Blogs/Azure/Azure-Logic-Apps-Walkthrough-Webhook-Functions-and-an-SMS-Bot?ocid=player

Lite hjälp på vägen...det finns inte instruktioner på hur man skapar en Function i videon:
	1. Skapa en ny Function App
	2. Lägg till en ny Function ("HttpTrigger-JavaScript"). Tips! Namnet på din Function kommer att användas i det sista LogicApp steget.
	3. Klistra in koden (index.js) som du hittar här: https://github.com/logicappsio/AzureFunction-URLFormDecoder/blob/master/function.js
	4. Testkör din Function i Azure portalen med tex: "form": "Hello=world&foo=bar+foox&test=again"

Steg 3: Om du vill jobba vidare med Functions så rekommenderar jag att använda en Azure Functions Extension för VisualStudio. Denna är dock i preview tills detta fungerar helt i VS2017 och fungerar endast med C# för närvarande. Här får du möjlighet att:
	• Debugga med breakpoints
	• Sätta upp Continous Integration med tex. Git
Labba gärna med detta :)!

Steg 4: Om du vill göra ännu mer så lägg till möjligheten att skicka dina LogicApp loggar till EventHub för felhantering mm. Läs mer här: https://docs.microsoft.com/en-us/azure/logic-apps/logic-apps-scenario-error-and-exception-handling. Utnyttja det ni lärde er i en tidigare session med EventHub, StreamAnalytics och PowerBI för att tex. visualisera olika fel.

