# Welcome to MLSA Blazor Outlook Calendar!
It's a Calendar and events application that is synced and integrated with Microsoft Outlook Calendar using Microsoft Graph API.
## Objectives
- View all events on your calendar
- Add events to my calender
- View a summary of events per day

## How to make this app works

 - Clone this repository locally to your machine.
 - Make sure you have the latest version of .NET Core 3.1, you can find it [here](https://dotnet.microsoft.com/download) 
 - Sign in to your Microsoft Azure account or create a new free account.
 - Go to your Azure Active Directory then AppRegistrations 
 - Click on create a new registration
 - Call the app what ever you want 
 - Set the account type to Multi-Tenant (Microsoft Personal Accoutns)
 - In the  *Redirect URI*  section: Choose Single Page Application and set the URI to https://locahost:5001/authentication/login-callback
 - Click Register
 - Copy the Application Id that appears in the overview section and paste it within the *AppSettings.json* file in the wwwroot folder inside the BlazorCalendar project.
 - Back to your Azure application go to the *Authentication* page from the left side menu within your app.
 - Go to *Implicit grant* section and check *Access Token and ID Tokens* and save the changes 
 - Go to API Permissions page from the left side menu.
 - Add Permissions then Microsoft Graph and Add *Calendars.ReadWrite* permission.
 - Go back to your project folder and open the cmd then the run the command dotnet run. 
 And ready to go.


