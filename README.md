# Cost-Optimization-Jenkins-Logs
Upload Jenkins build logs to an Amazon S3 bucket for  Cost Optimization

# Script Overview
The script iterates through all jobs and their respective builds in a Jenkins instance.<br />
It identifies build logs created on the current date and uploads them to an Amazon S3 bucket.<br />
It checks for the presence of the AWS CLI to handle S3 uploads.<br />

Pre-Check: Verifies if AWS CLI is installed.<br />
Job Iteration: Loops through each Jenkins job directory.<br />
Build Iteration: Loops through each build directory for the job.<br />
Log Filtering: Checks if the build's log file exists and was modified today.<br />
Upload: Uploads valid log files to the S3 bucket and logs the result.<br />
