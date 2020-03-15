# Introduction

Leave Management - The goal is to create a leave managment system that process of handling leaves and absences due to sickness vacation or other reasons, increases employee satisfaction, provides transparency and eliminates unexplained or excessive absenteeism.

Here are some major problems:

1. Line managers were not able to manage leaves of every team members within boom.camp organization that cause to make informed decisions before approving leaves.

2. Boom.Camp employees updates leave content by sending multiple leave request. 

3. Untrackable employees leaves and uninformed decisions.


# Requirements:

## Database

* Database name `bc_leave_db`.

* Database custom tables should also have a table prefix `bc_`.

* Able to dump mysql database. 

* Custom queries should be a prepared statements.

## Pages


### Dashboard

1.) Home - The main landing page that tells about the Boom.Camp leave management it should have a button "Request Leave" that will redirects the employee to the request form page


### Employees Menu:
	
1.) Request Policy - The policy for requesting a leave.

2.) My Leave(s) - The page that displays leave information including Approved, Pending and Rejected within a year `current requested leaves should be editable`.

3.) My Leave Balance - The leave balances it includes leave taken the previous month, but do not include any leave taken during the current pay period.

4.) Request a Leave - Request form to be filled up by an employee.

```
Date filed: Date today 
Project Manager(s)/Supervisor: (Can select multiple managers or supervisors)
Type : (Leave without pay(absent) or Leave with pay(Vacation/Sick/Maternity etc.))
Reasons: (A valid leave reason)
Leave Balance: (If type is absent do not display leave balance, should also have an information that it will be deducted once leave request approved)
Duration: (Nos. of leave days)
Status: (Default is Pending)
From: (Leave from)
To: (Leave until)
```

### Line Manager(s) menu

1.) Request Policy

2.) Employee Leave(s) - Searchable by department and last name but sortable by leave status and department, line managers should have an option to update employees leave status to `Approved`, `Pending` or `Rejected`, every leave is `PRINTABLE` to be signed by line managers.

3.) My Leave(s)

4.) My Leave Balance 	

5.) Request a Leave


### HR personnel

1.) Update Policy - A form that updates the request policy.

2.) Leave Balance 

* Add leave types - Able to add new leave types to be used by the requester.

Example: 

```
Type: Leave with pay
Name: Maternity
Days: 60 days
Paid: Yes

Type: Leave without pay
Name: Absent
Days: 0 days
Paid: No
```

* Add leave balance - Able to add new leave balance for the next year(s) in a department(e.g 2021 - Software Development - 2021)

```
Department: Software Development
Year : 2021

Leave Type(s) :
 1.) Leave with pay 
     Sick: 5 days
     Vacation: 15 days
     
 2.) Leave without pay
     Absent : 0 days
```

* Update leave balances - Able to update leave balances of the employees (updates should be in every department)
		
3.) My leave balance 	

4.) Request Leave


## Url

Application urls should be readable format

## Plugins

Bomm.Camp leave management should be in a form of plugin called `bcleave` and can be installed to other wordpress projects.

## Security

Youre task is to determine what [security measures](https://secure.wphackedhelp.com/blog/wordpress-security-checklist-guide/) are needed to apply to ensure that application are not prone to hacking.

## Hosting

You will need to host this appliction and have live domain accessable in public.

## Admin Login

Should have a custom url and hidden to public.

## Screen sizes and Layout

You should create a responsive UI and have at least 3 different screen sizes.

# Finished

Submit the following to Google Classroom assignment related to this project.

* Link of repository.
* Link of your live domain.
* Link to `.zip` of your custom plugins.

