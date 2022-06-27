# alfred-workflows

# Confluence Search Person
This workflow searches a person email from the person profile on Confluence. When found and used once the email is saved to a text file to be reused in the future. This allows to reduce amount of API calls sent to Confluence.

Release notes:
0.0.5
- moved to Python 3
- changed keywords for searching email from 'n' to 'ue'
- generalized workflow name, logos, variables names, descriptions
- renamed bundle it
- renamed folders and files in the workflow
0.0.4
- replaced unirest library with native http.client library
- confluence host is moved to environment variables
0.0.3
- Added possibility to search by cyrillic query
0.0.2
- Added possibility to search in NIX Confluence
0.0.1
- Search emails from the file with a list of users

# Tunnelblick VPN
This workflow allows connecting/disconnecting a Tunnelblick VPN profile. When typing 'vpn' keyword it will show a list of all profiles and their statuses (ON or OFF). When clicking Enter on a profile it will start connection (it it was OFF) or stop it (if it was ON).

If you start typing a vpn profile after 'vpn' keyword the provided list of profiles will be filtered out appropriately

When you set DEFAULT_PROFILE variable the profile will always be the first item in the list of profiles. This allows you to avoid extra clicking arrows down to chose one, whis would be inconvenient if your most used profile is somewhere down the list.

Do not forget to specify a path a folder where tunnelblickctl executable file is located. Without it the script will not know where to start tunnelblickctl command from.

The workflow requires:
- Tunnelblickctl to be preinstalled on you computer. Here is the repository where it can be taken: https://github.com/benwebber/tunnelblickctl
- Python 3
