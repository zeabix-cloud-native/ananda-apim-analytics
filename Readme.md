### Monitor and built-in API Analytics
Use the Azure portal to review analytics data at a glance for your API Management instance.
1. In the [Azure portal](https://portal.azure.com/), navigate to your API Management instance.
2. n the left-hand menu, under Monitoring, select Analytics.
![Analytics](./assets/monitoring-menu-analytics.png)

3. Select a time range for data, or enter a custom time range.
4. Select a report category for analytics data, such as Timeline, Geography, and so on.
5. Optionally, filter the report by one or more additional categories.

### Application Insight
Create a connection between Application Insights and API Management
1. Navigate to your Azure API Management service instance in the Azure portal.
2. Select Application Insights from the menu on the left
3. Select + Add.
![Appication Insignt](./assets/apim-app-insights-logger-1.png)
4. Select the Application Insights instance you created earlier and provide a short description.
5. To enable availability monitoring of your API Management instance in Application Insights, select the Add availability monitor checkbox.
    * This setting regularly validates whether the API Management gateway endpoint is responding.
    * Results appear in the Availability pane of the Application Insights instance.
6. Select Create.
7. heck that the new Application Insights logger with an instrumentation key now appears in the list.
![APIM Application Insight](./assets/apim-app-insignt-logger-2.png)

### Enable Application Insights logging for your API
1. Navigate to your Azure API Management service instance in the Azure portal.
2. Select APIs from the menu on the left.
3. Click on your API, in this case Demo Conference API. If configured, select a version.
4. Go to the Settings tab from the top bar.
5. Scroll down to the Diagnostics Logs section.
![APIM Application Insight](./assets/apim-app-insights-api-3.png)
6. Check the Enable box.
7. Select your attached logger in the Destination dropdown.
8. Input 100 as Sampling (%) and select the Always log errors checkbox.
9. Leave the rest of the settings as is.
10. Select Save.
