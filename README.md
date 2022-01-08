# FTP-to-AmazonS3

This module provides the functionality of uploading files to s3 from a FTP server. An SFTP connection is created with the FTP server and all the files present in the specified directory are uploaded to the specified s3 bucket. Following are the key features of this module:

Creates a secure ssh connection with FTP server.

Handles multipart upload to s3 automatically, if file size is greater than 100MB (can be configured).

Automatically handles retires in case of failed uploads during multipart upload.

Partitions the data in s3 based on current year,month,day,hour.

Ensures which file has been processed or needs to be processed.
