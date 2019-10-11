# AWS Lambda Python boto3 moving files between S3 (archive)

This script will copy all files that are older than one month from my_bucket_name to my_arch_bucket_name (this variables 
are editable). 
The retention for files is 30 days and it can be changed by the datetime.timedelta(days=30) method's parameter.
After the copying process the files in old bucket will be deleted. 
Please be advised, that the archived files WILL HAVE NEW MODIFIED DATE parameter. 
It will print out the list of names of files TO MOVE and will return list of files to stay (younger than 30 days).
