# Apex GMT Offset

This Custom Setting and Schedulable Apex class allows users to set and retireve the GMT Offset per user or for a master user.

Install the package:

<br/>

<a href="https://githubsfdeploy.herokuapp.com?owner=tiaanswart&repo=ApexGMTOffset&ref=master">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

<br/>

Then run the scheduled job at 2AM every day by executing the below code in the Developer Console:

`System.schedule('GMT Offset Scheduled Job', GMTOffsetScheduler.CRON_EXP, new GMTOffsetScheduler());`

The schedulable job will run and update the Org Default Custom Setting Rec with Time Zone offset.