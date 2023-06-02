# ML-AI--Finger-detection-container-scaleup
Machine learning AI model for Scale UP the docker Containers on ec2

**********************************************************************
To setUp this Project 

1. Launch 'EC2' instance on AWS 
   					--Set up configuation for Docker on Instace
-----------------------------------------------------------------------
2. Use 'Systems Manager AWS' service --> 
						to remote configure the system/Instace.

-----------------------------------------------------------------------
3. Set the 'IAM Role access' to --> (SSM to access the EC2)

-----------------------------------------------------------------------
4. Create lambda function --> 
				-- we use 'boto3' as a client tool to connect 'SSM' 
				-- SSM 'Runcommand' on the Lambda Function
				-- Set the IAM role access for 
							('Lamda function' to-- 'SSM')

----------------------------------------------------------------------
5. Create an 'Amazon API Gateway'
				-- RestAPI
				-- Create and API for the Lamda function to run 
					on when the -- URL is hit

-----------------------------------------------------------------------

6. Client User --> uses the 'Machine Learning model' code to ScaleUp 
					python Code 
						-- using HandTrackingModule and cv2 library
				 
