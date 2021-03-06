## IBM Cloud Watson Personality Insights Lab
See what Watson has to say about you!

### Get Started with the lab by following the steps below

1. Create a Watson personality service in your own org and space in the IBM Cloud Dashboard 
	1. Go [Here](https://console.bluemix.net/catalog/services/personality-insights?env_id=ibm:yp:us-south) and edit **Service name** to `MyPersonalityInsights`, leave the rest as default and click **Create** in the bottom right corner.
1. Clone or [Download the zip](https://github.com/alohr51/Bluemix-Lab/archive/master.zip) file of this git repository.
1. Push your app to the IBM Cloud
	1. Download the [Cloud Foundry CLI](https://github.com/cloudfoundry/cli#downloads) to interact with the IBM Cloud from the command line
	1. Open your terminal and `cd` to the root of your local repository's directory (Where app.js is)
	1. Login to the US-South Region and the org and space you created the Watson service in using the below commands
		1. `cf api api.ng.bluemix.net`
		1. `cf login` (Use your Bluemix credentials)
			1. if `cf login` fails due to federation try using `cf login -sso` and use the link given to get a temp password
		1. cf will ask you to target an org and space. Select the org and space you created the watson service in
	1. `cf push`
	That is it! the manifest.yml file will take care of all the extra options. When your app is done the url will show in the logs
1. Your application is now up and running in the public cloud!
	1. Go to the IBM Cloud application URL and use the prefill buttons or write any text you want  and click `Ask Watson`!