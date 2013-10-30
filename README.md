sample CloudFoundry installer on WindowsAzure using Chef

----

To download your publish settings file visit https://windows.azure.com/download/publishprofile.aspx

----

To prepare your vm

bundle exec knife solo prepare -i ~/.ssh/azure.pem azureuser@137.116.231.118

----

To provision server with config.json

bundle exec knife solo cook -i ~/.ssh/azure.pem azureuser@137.116.231.118 -N config