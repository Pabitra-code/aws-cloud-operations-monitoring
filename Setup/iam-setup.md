# IAM Setup
# IAM User Setup

## Objective
The objective of this step was to create a secure AWS access mechanism by using an IAM user instead of the root account. This follows AWS security best practices and helps in controlled access management.

## Steps Performed
- Created a dedicated IAM user for cloud operations tasks
- Enabled AWS Management Console access for the IAM user
- Attached only required permissions for the project
- Avoided using the root account for daily operations

## Permissions Assigned
The following AWS managed policies were attached:
- AmazonEC2FullAccess
- CloudWatchFullAccess

These permissions were sufficient to launch and manage EC2 instances and to view monitoring metrics for this project.

## Security Considerations
- Root account was used only for initial account setup
- IAM user was used for all operational activities
- Least required permissions were followed to reduce security risk

## Outcome
A secure IAM user was successfully created and used to perform all further AWS operations in this project.
