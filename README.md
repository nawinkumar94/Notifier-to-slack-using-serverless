# Notifier-to-slack-using-serverless
Sending notification to slack users based on the cloud watch events using serverless lambda, SNS and auto scaling policy
Notifon has the following features
    ---> Send notification to slack using serverless. when the cloud watch events happens by
         auto scaling groups or lambda functions.

#Commands for serverless application

  # create a serverless application
    --> serverless create --template aws-python3 --name notifon-notifier
    --> serverless create -t "Name of template" -n "Name of the lamba function"
  # To deploy application
    --> sls deploy
  # Invoke a function('startProcessingVideo'-->name of function)
    --> sls invoke -f post_to_slack
  # To check logs('startProcessingVideo'-->name of function)
    --> sls logs -f post_to_slack -t