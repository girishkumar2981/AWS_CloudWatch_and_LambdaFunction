# AWS_Cost_Management

Identification of Stale EBS Snapshots

In this instance, we'll generate a Lambda function tasked with recognizing EBS snapshots that are not currently linked to any active EC2 instance. It will then proceed to remove these snapshots in order to reduce storage expenses.

The Lambda function retrieves all EBS snapshots owned by the account and gathers a list of active EC2 instances, including both running and stopped ones. It then examines each snapshot to determine if its associated volume is not linked to any active instance. If it identifies a snapshot that is no longer relevant, it proceeds to delete it, thereby optimizing storage expenses.
