******************************************************************************************************************************
******************************************************************************************************************************
************************************************************Read ME***********************************************************
***********************************Developed By Mostafa Ahmed(moustapha.anwar@hotmail.com)************************************
******************************************************************************************************************************
******************************************************************************************************************************

To Enhance Oryx Editor: 

1- Install Oryx follow the steps in this URL (https://code.google.com/p/oryx-editor/wiki/SetupDevelopmentEnvironment)
2- To add new monitoring rules:
	1- Add the new rule into this file "oryx\editor\data\stencilsets\monitoringRules\monitoringRules.json".
	2- Add the Rule's SVG file into this folder "oryx\editor\data\stencilsets\monitoringRules\view".
	3- Generate new version of oryx.war file (as described in the URL), and deploy it.
3- To Enhance XML Generator plugin:
	1- edit "createXMLNodeAttributes" method in "oryx\editor\client\scripts\Plugins\XMLBuilder.js" to add more attributed to be shown in the generated XML.
	2- Generate new version of Oryx.war file (as described in the URL), and deploy it.
	
4- to Add a new stencil
	1- Follow the steps in this link (https://code.google.com/p/oryx-editor/wiki/HowToCreateStencilSet).
	
To Enhance CEP server:

1- Open the CEP Server project using Visual Studio 2012.
2- To define new EPL statement:
	1- Add the EPL statement definition in this class "CEP Server\EPLTemplates.cs"
	2- Edit the switch case in "TraverseRule" method in "CEP Server\Services\StatementManagerService.cs" class to include the new rule.
	
To Use Activiti Events Emitter plugin:

1- Download Activiti code from (https://github.com/Activiti/Activiti/releases/download/activiti-5.16.3/activiti-5.16.3.zip)
2- Open activiti-explorer.war using WinZip(this war file will be found in "activiti-5.16.3\wars")   
3- Import ActivitiCustomEventHandler project in Eclipse	
4- Export ActivitiCustomEventHandler project as a jar
5- Copy this jar to (activiti-explorer\WEB-INF\lib)
6- Deploy activiti-explorer.war using Tomcat and go to "http://localhost:8080/activiti-explorer/" to start Activiti.    
