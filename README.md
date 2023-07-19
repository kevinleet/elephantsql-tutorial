# ElephantSQL Tutorial

![banner](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/banner.jpg?raw=true)

## Introduction

In the digital age, where data is scattered everywhere, it's important for Django developers to know how to connect their projects to remote databases. In this tutorial, we'll walk you through the process of seamlessly linking Django, the awesome web framework, to a remote database. By using a remote database, you can take your Django projects beyond a single machine or local network. This brings a bunch of cool benefits like collaborating with teams spread across the globe, scaling your projects effortlessly, and beefing up your data security. With the power of remote databases at your fingertips, Django becomes even more powerful, enabling you to create robust and flexible applications that rock in today's data-driven world. So, let's dive in and make those remote connections like a pro!

## Creating A Remote PostgreSQL Database

To get started with creating a remote PostgreSQL database for your Django project, follow these simple steps:

1. Head over to ElephantSQL, a cloud-based PostgreSQL database provider, by visiting their website: https://www.elephantsql.com.

2. Once you're on the ElephantSQL website, look for the "Log In" button and then click on "Sign Up" at the bottom of the log in page. This will take you to the registration page.

![loginpage](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/login.png?raw=true)

3. Fill in the required information (your email address), to create your ElephantSQL account. Then check the inbox for that email address for the confirmation email from ElephantSQL.

4. After verifying your email address, you will be redirected back to ElephantSQL to finish creating your account. Follow the instructions provided to complete the registration process.

5. Once your account is set up and verified, you will be redirected to the ElephantSQL dashboard. This is where you'll be able to create and manage your remote PostgreSQL databases.

Congratulations! You've created your ElephantSQL account and are ready to move on to the next step of setting up your remote PostgreSQL database for your Django project.

## Creating a New PostgreSQL Instance

1. On the ElephantSQL dashboard, click on the "Create New Instance" button or the "+ New Instance" option. This will start the process of creating a new PostgreSQL instance.

![createinstance](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/createinstance.png?raw=true)

2. You will be prompted to choose a plan for your database. ElephantSQL offers various plans with different resource allocations, depending on your needs. For this tutorial, we will be using the free plan called 'Tiny Turtle'.

![selectplan](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/selectplan.png?raw=true)

3. Select the 'Tiny Turtle' plan and give your instance a name. The instance name can be anything you like, but make sure it's descriptive so that you can easily recognize it later.

4. You can also choose the region where your database will be hosted. Select the region that is geographically closest to your target audience or your own location for better performance.

![selectregion](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/selectregion.png?raw=true)

5. Click the "Create" or "Continue" button to initiate the instance creation process. ElephantSQL will now provision your database, which may take a few moments.

## Accessing Your ElephantSQL Instance Details

1. Once the instance is successfully created, you will be redirected to the instances list page. Here, you should see the newly created instance listed with the name you provided.

2. Click on the instance name to access its details. In this page, you'll find information about your PostgreSQL database, including the connection details required to connect to it from your Django application.

3. Look for the following essential details:

- Server: The URL that our Django application will connect to.
- User & Default Database: The username to log in to the PostgreSQL instance. The default database name.
- Password: The password associated with the username for authentication.

![instancedetails](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/instance.png?raw=true)

## Configuring Django to Connect to ElephantSQL

1. Open your Django project in your preferred code editor.

2. Locate the DATABASES settings in your Django project's settings.py file. It should look something like this:

![database_original](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/databases1.png?raw=true)

3. Replace the current settings with the ElephantSQL instance details you obtained earlier. It should look similar to this:

![database_new](https://github.com/kevinleet/elephantsql-tutorial/blob/main/images/databases2.png?raw=true)

4. Save the 'settings.py' file.
