# Robo Advisor
This project uses Amazon Web Services (AWS) to create a bot that customers can use to get investment portfolio recommendations for retirement. 



## Technologies
Click on the links below for documentation on each of the technologies used. This project uses the following libraries and dependencies:
+ [**Anaconda**](https://docs.anaconda.com/): an open source package and environment management system.
+ [**JupyterLab**](https://jupyterlab.readthedocs.io/en/stable/): an extensive environment using web-based user interface designed for data analysis. 
+ [**Pandas**](https://pandas.pydata.org/docs/getting_started/index.html): (included in Anaconda) a Python package data analysis toolkit.
+ [**Numpy**](https://numpy.org/doc/stable/) for scientific computing such as mathematical, basic statistical operations, and much more. 
+ [**scikitlearn**](https://scikit-learn.org/stable/install.html) an open source machine learning library that supports supervised and unsupervised learning. It also provides various tools for model fitting, data preprocessing, model selection, model evaluation, and many other utilities. 
+ [**matplotlib inline**](https://pandas.pydata.org/pandas-docs/version/0.13.1/install.html): library to create static, animated, and interactive visualizations in JupyterLab.


## Installation Guide
Sign up for AWS Free Tier account. 
1. To start using AWS, you need to create an account. Although doing this is free, you need to provide a valid credit card that allows Amazon to charge for any service usage beyond the limits of the free tier. The details for each free offer are constantly updated, so it’s a good idea to check the latest terms on the [AWS Free Tier ](https://aws.amazon.com/free/free-tier/) site.

 **Create an Administrator User**

To create an IAM user, open the AWS Management Console (Links to an external site.) by using your root user, and then complete the following steps:

1. In the search box, type “iam,” and then click “IAM” in the list of results that display.
2. In the left navigation pane, click Users. In the “IAM users” pane on the right side, click the “Add user” button.
3. On the “Add user” page that appears, set the user details as follows:
    + In the “User name” box, type “administrator.”

    + In the “Access type” area, select the “Programmatic access” and “AWS Management Console access” checkboxes.

    + In the “Console password” area, select the “Custom password” option, and then in the box, type your password.

    + In the “Require password reset” area, clear the “User must create a new password at next sign-in” checkbox.
4. Click the “Next: Permissions” button to continue. To set permissions, click “Add user to group, and then click the Create group button.
5. In the “Create group” dialog box that appears, in the “Group name” box, type “administrators".
6. Click “Filter policies,” and then on the drop-down menu that appears, select the “AWS managed - job function” checkbox.
7. In the policy list, select the checkbox for the AdministratorAccess policy name, and then click the “Create group” button. 
8. The “Create group” dialog box closes. Back on the “Add user” page, in the “Add user to group” area, select the checkbox for your new administrators group. If necessary, click the Refresh button to display the group in the list.
9. Click the "Next: Tags" button to continue.
10. On the “Next: Tags” page, leave the defaults, and then click the “Next: Review” button to continue.
11. Review your choices, which the page displays. When you’re ready to proceed, click the **Create user** button.
12. Once the user is created, a Success message appears. Click the “Download .csv” button to download the user's credentials, and keep those credentials in a safe location.
