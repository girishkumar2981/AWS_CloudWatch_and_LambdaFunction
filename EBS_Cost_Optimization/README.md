# AWS_Cost_Management

Identification of Stale EBS Snapshots

In this instance, we'll generate a Lambda function tasked with recognizing EBS snapshots that are not currently linked to any active EC2 instance. It will then proceed to remove these snapshots in order to reduce storage expenses.

The Lambda function retrieves all EBS snapshots owned by the account and gathers a list of active EC2 instances, including both running and stopped ones. It then examines each snapshot to determine if its associated volume is not linked to any active instance. If it identifies a snapshot that is no longer relevant, it proceeds to delete it, thereby optimizing storage expenses.

output:

<img width="768" alt="image" src="https://github.com/girishkumar2981/AWS_Cost_Management/assets/61040201/396924d5-db09-4b46-b5b4-71d35ea915a5">

Following policies need to be assigned to the role.

<img width="333" alt="image" src="https://github.com/girishkumar2981/AWS_Cost_Management/assets/61040201/6ac6e81f-cc9b-4774-9998-f0a3054b69d2">
