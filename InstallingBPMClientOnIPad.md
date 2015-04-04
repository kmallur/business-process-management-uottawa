#Steps to install the BPM client and have access on the iPad
##### Back to the [Table of Contents](Table_Of_Contents.md) #####
# BPM on the iPad (using the University of Ottawa  IBM BPM server) #

## Steps ##

  1. In the App Store, purchase(it's free) the IBM Business Process Manager app.
  1. Install the app on your iPad.
  1. We now need to connect the iPad to the VPN. Download the iPad mobile VPN configuration from http://www.uottawa.ca/support/en/software/vpn-client.
  1. I was not able to download it directly from my iPad so I sent it by email to myself(from a desktop) and opened the file from the email on my iPad. Automatically, it should prompt you to "Install Profile". It will warn you that it is an Unverified Profile. Click "Install Now."
  1. A prompt to enter your iPad's Passcode will appear if you have one. Enter it if you do.
  1. Enter your information for the VPN network at the university as it will prompt you.
  1. Click "Done".
  1. Go to Settings -> General -> VPN.
  1. Choose the VPN configuration you installed and turn the VPN on whenever you want to use the IBM BPM app. When you turn the VPN on, it will prompt you for your VPN password and tell you you are connected once you click OK (if the connection is successful).
  1. Go to the IBM BPM app.
  1. Add a "Business Process Manager" account.
    * Host: http://oslerbpm.site.uottawa.ca
    * Port: 9080
    * Account Name: `NameYouWantToGiveToYourAccount`
    * User Name: `UserNameOfTheAccountYouWantToUse`(ex: `DemoPhysician`)
    * Password: `PasswordOfTheAccountYouWantToUse` (ex: password)
  1. Click Add and you should now have access.

**Note:** It is possible to add multiple accounts on the same iPad.


