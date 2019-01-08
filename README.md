# Umbraco v8 Beta Site

I set up this repo so I can play with Umbraco v8 without having to install the alpha/beta nuget package each time or without having to fork the temp8 branch of the UmbracoCms source code.

Feel free to fork it if you want to use it.

When you want to go back to the beginning you can just revert the changes.

The login details for the backoffice are:

Username: admin@admin.com
Password: 1234567890

If you are interested in the steps I took to get this repo ready, here they are. You won't need to do this though if you just fork the repo.

To set this site up, all I did was the following:

- Create the repo in GitHub
- Clone the repo
- Create a new .NET Framework 4.7.2 Web Project inside the project folder locally
- Install the NuGet package for the alpha/beta of Umbraco v8
```
Install-Package UmbracoCms -Pre -Source https://www.myget.org/F/umbracocore/api/v3/index.json
```
- Build the solution
- Run without Debugging (Ctrl + F5)
- Run through the Umbraco Install screen
- Create a doc type with a template and call it Home
- Allow this doc type to be created at the root
- Create the home page at the root of the content tree
- add a load of files and folders to the gitignore
- commit and push the changes
