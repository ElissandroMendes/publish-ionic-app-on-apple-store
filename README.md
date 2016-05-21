# publish-ionic-app-on-apple-store
How to publish an ionic APP on Apple store 
* Step 1->  configure your ionic app means add the unique package name in config.xml file 
* Step 2-> Add ios platform to ionic project app using below command
          * # $  Ionic platform add ios
* Step 3-> now build your ionic project using the below command 
* # $ ionic build ios –release
* Step 4-> Login Xcode with developer.apple.com account
* Step 5-> Login developer.apple.com account on web site
* Step 6- > now 1st we need to create certificate for app profile so open keychain access from MAC system , then from the keychain access-> at top menu certificate Assistant-> Request a certificate from a certificate authority.
1 window fill open fill the developer info then save the certificate file
* Step 7-> now open the web developer.apple.com click on + button in certificate creation page, -> in Production select -> Apple store and Ad Hoc then continue , now choose certificate file that is generated in step 6 now continue for next step and download certificate .
* Step 8 -> aging open keychain access to install the certificate , drag the downloaded certificate to keychain access->login 
* Step 9->open web now
* Step 10 -> now we need to create App ID in developer account, provide name and buindle ID(com.parken.urban)  now ->continue->submit->done
* Step 11-> now create Provisioning Profile in developer account,click on distribution and select App store -> continue now select the app id that is created in step 10 , give profile name and Generate   now click on download and done.
* Step 12 -> now double click on Provisioning Profile file that is downloaded in step 11 to add the profile into the iphone library,
* Step 13 -> open the project in Xcode and select the project , now select the under project, project name , now click on info and add Distribution under in configuration section with Relase,Debug.
* Step 14 -> Now select project under Target now select Build setting section and in the code signing section set the certificate name in code signing identity and  provision profile name. and now do the same Build setting under project code signing and provision profile ,
Now project is ready to Archive, So now go to at top and under Product-> Archive to archive the project , it will take couple of second , and now App is ready to Publish on Apple store . before publishing the app use the step 15.
* Step 15 -> now go to the web developer.apple.com and open itune and now create new app and complete all the details for the app information .

# Thank You
