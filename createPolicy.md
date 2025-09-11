## Create an Incident creation policy

To create a policy that will create an incident based on the classification, go to the **Automations** page, click **Create policy**

![Policy](images/Policy01.png)

Choose **Promote alerts to an incident**

![Policy](images/Policy02.png)

Fill in a name

![Policy](images/Policy03.png)

Set increasing event count as the reason to generate an incident.

![Policy](images/PolicyTrigger.png)

Set the alert condition to create an Incident. Click **Add alert condition** and choose "Basic".

Then, click **Add basic condition** and choose "Alert property" condition to check for the alert `classification` field. Use "SMAX test event" as value.

![Policy](images/Policy04.png)

In **Create an incident** section, click the **Open a ticket** selector and pick your SMAX integration.

![Policy](images/Policy05.png)

Scroll back up and hit **Create policy** button at the top-right corner.

To trigger an incident, [generate a test alert](./createAlert.md).

