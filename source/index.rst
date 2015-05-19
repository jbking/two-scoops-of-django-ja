.. Two Scoops of Django ja documentation master file, created by
   sphinx-quickstart on Tue May 19 16:54:08 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Two Scoops of Django ja's documentation!
===================================================

Contents:

* Dedication v
* About the Dedication . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . vi
* Authors’ Notes xxvii
* A Few Words From Daniel Roy Greenfeld . . . . . . . . . . . . . . . . . . . . . . . . . xxvii
* A Few Words From Audrey Roy Greenfeld . . . . . . . . . . . . . . . . . . . . . . . . xxviii
* Introduction xxix
* A Word About Our Recommendations . . . . . . . . . . . . . . . . . . . . . . . . . . xxix
* Why Two Scoops of Django? . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxx
* Before You Begin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxi
* This book is intended for Django 1.8 and Python 2.7.x/3.3.3+ . . . . . . . . . . . . xxxi
* Each Chapter Stands On Its Own . . . . . . . . . . . . . . . . . . . . . . . . . . xxxi
* Conventions Used in This Book . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxii
* Core Concepts . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxiii
* Keep It Simple, Stupid . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxiii
* Fat Models, Helper Modules, Thin Views, Stupid Templates . . . . . . . . . . . . xxxiv
* Start With Django By Default . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxiv
* Be Familiar with Django’s Design Philosophies . . . . . . . . . . . . . . . . . . . xxxiv
* The Twelve Factor App . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxv
* Our Writing Concepts . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxv
* Provide the Best Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxv
* Stand on the Shoulders of Giants . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxv
* Listen to Our Readers and Reviewers . . . . . . . . . . . . . . . . . . . . . . . . xxxvi
* Publish Errata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . xxxvi
* 1 Coding Style 1
* 1.1 The Importance of Making Your Code Readable . . . . . . . . . . . . . . . . . . 1
* 1.2 PEP 8 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
* 1.2.1 The 79 Character Limit . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
* 1.3 The Word on Imports . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3
* 1.4 Use Explicit Relative Imports . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
* 1.5 Avoid Using Import * . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
* 1.6 Consider the Django Coding Style Guidelines . . . . . . . . . . . . . . . . . . . 9
* 1.7 Choose JS, HTML, and CSS Style Guides . . . . . . . . . . . . . . . . . . . . . 9
* 1.7.1 JavaScript Style Guides . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
* 1.7.2 HTML and CSS Style Guides . . . . . . . . . . . . . . . . . . . . . . . 10
* 1.8 Never Code to the IDE (Or Text Editor) . . . . . . . . . . . . . . . . . . . . . . 10
* 1.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
* 2 The Optimal Django Environment Setup 13
* 2.1 Use the Same Database Engine Everywhere . . . . . . . . . . . . . . . . . . . . 13
* 2.1.1 Fixtures Are Not a Magic Solution . . . . . . . . . . . . . . . . . . . . . 13
* 2.1.2 You Can’t Examine an Exact Copy of Production Data Locally . . . . . . 14
* 2.1.3 Different Databases Have Different Field Types/Constraints . . . . . . . 14
* 2.2 Use Pip and Virtualenv . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
* 2.3 Install Django and Other Dependencies via Pip . . . . . . . . . . . . . . . . . . 17
* 2.4 Use a Version Control System . . . . . . . . . . . . . . . . . . . . . . . . . . . . 18
* 2.5 Optional: Identical Environments . . . . . . . . . . . . . . . . . . . . . . . . . . 18
* 2.5.1 Vagrant and VirtualBox . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
* 2.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 20
* 3 How to Lay Out Django Projects 21
* 3.1 Django 1.8’s Default Project Layout . . . . . . . . . . . . . . . . . . . . . . . . . 21
* 3.2 Our Preferred Project Layout . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22
* 3.2.1 Top Level: Repository Root . . . . . . . . . . . . . . . . . . . . . . . . . 23
* 3.2.2 Third Level: Configuration Root . . . . . . . . . . . . . . . . . . . . . . 23
* 3.3 Sample Project Layout . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 24
* 3.4 What About the Virtualenv? . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27
* 3.5 Using a Cookiecutter Template to Generate Our Layout . . . . . . . . . . . . . . 28
* 3.6 Other Alternatives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 29
* 3.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 29
* 4 Fundamentals of Django App Design 31
* 4.1 The Golden Rule of Django App Design . . . . . . . . . . . . . . . . . . . . . . 32
* 4.1.1 A Practical Example of Apps in a Project . . . . . . . . . . . . . . . . . . 33
* 4.2 What to Name Your Django Apps . . . . . . . . . . . . . . . . . . . . . . . . . 34
* 4.3 When in Doubt, Keep Apps Small . . . . . . . . . . . . . . . . . . . . . . . . . 35
* 4.4 What Modules Belong in an App? . . . . . . . . . . . . . . . . . . . . . . . . . 35
* 4.4.1 Common App Modules . . . . . . . . . . . . . . . . . . . . . . . . . . . 35
* 4.4.2 Uncommon App Modules . . . . . . . . . . . . . . . . . . . . . . . . . 36
* 4.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 38
* 5 Settings and Requirements Files 39
* 5.1 Avoid Non-Versioned Local Settings . . . . . . . . . . . . . . . . . . . . . . . . 40
* 5.2 Using Multiple Settings Files . . . . . . . . . . . . . . . . . . . . . . . . . . . . 41
* 5.2.1 A Development Settings Example . . . . . . . . . . . . . . . . . . . . . 44
* 5.2.2 Multiple Development Settings . . . . . . . . . . . . . . . . . . . . . . . 45
* 5.3 Separate Configuration From Code . . . . . . . . . . . . . . . . . . . . . . . . . 46
* 5.3.1 A Caution Before Using Environment Variables for Secrets . . . . . . . . 47
* 5.3.2 How to Set Environment Variables Locally . . . . . . . . . . . . . . . . 47
* 5.3.3 How to Set Environment Variables in Production . . . . . . . . . . . . . 49
* 5.3.4 Handling Missing Secret Key Exceptions . . . . . . . . . . . . . . . . . 50
* 5.4 When You Can’t Use Environment Variables . . . . . . . . . . . . . . . . . . . . 52
* 5.4.1 Using JSON Files . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52
* 5.4.2 Using Config, YAML, and XML File Formats . . . . . . . . . . . . . . 53
* 5.5 Using Multiple Requirements Files . . . . . . . . . . . . . . . . . . . . . . . . . 53
* 5.5.1 Installing From Multiple Requirements Files . . . . . . . . . . . . . . . . 55
* 5.5.2 Using Multiple Requirements Files With Platforms as a Service (PaaS) . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 55
* 5.6 Handling File Paths in Settings . . . . . . . . . . . . . . . . . . . . . . . . . . . 56
* 5.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 58
* 6 Model Best Practices 61
* 6.1 Basics . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 62
* 6.1.1 Break Up Apps With Too Many Models . . . . . . . . . . . . . . . . . . 62
* 6.1.2 Be Careful With Model Inheritance . . . . . . . . . . . . . . . . . . . . 62
* 6.1.3 Model Inheritance in Practice: The TimeStampedModel . . . . . . . . . 64
* 6.1.4 Database Migrations . . . . . . . . . . . . . . . . . . . . . . . . . . . . 65
* 6.2 Django Model Design . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 67
* 6.2.1 Start Normalized . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 67
* 6.2.2 Cache Before Denormalizing . . . . . . . . . . . . . . . . . . . . . . . . 67
* 6.2.3 Denormalize Only if Absolutely Needed . . . . . . . . . . . . . . . . . . 67
* 6.2.4 When to Use Null and Blank . . . . . . . . . . . . . . . . . . . . . . . . 68
* 6.2.5 When to Use BinaryField . . . . . . . . . . . . . . . . . . . . . . . . . . 70
* 6.2.6 Try to Avoid Using Generic Relations . . . . . . . . . . . . . . . . . . . 71
* 6.2.7 PostgreSQL-Specific Fields: When to Use Null and Blank . . . . . . . . 72
* 6.3 The Model meta API . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 73
* 6.4 Model Managers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 73
* 6.5 Understanding Fat Models . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 75
* 6.5.1 Model Behaviors a.k.a Mixins . . . . . . . . . . . . . . . . . . . . . . . 76
* 6.5.2 Stateless Helper Functions . . . . . . . . . . . . . . . . . . . . . . . . . 77
* 6.5.3 Model Behaviors vs Helper Functions . . . . . . . . . . . . . . . . . . . 77
* 6.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 77
* 7 Queries and the Database Layer 79
* 7.1 Use get object or 404() for Single Objects . . . . . . . . . . . . . . . . . . . . . 79
* 7.2 Be Careful With Queries That Might Throw Exceptions . . . . . . . . . . . . . . 80
* 7.2.1 ObjectDoesNotExist vs. DoesNotExist . . . . . . . . . . . . . . . . . . 80
* 7.2.2 When You Just Want One Object but Get Three Back . . . . . . . . . . 81
* 7.3 Use Lazy Evaluation to Make Queries Legible . . . . . . . . . . . . . . . . . . . 81
* 7.4 Lean on Advanced Query Tools . . . . . . . . . . . . . . . . . . . . . . . . . . . 82
* 7.4.1 Query Expressions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 83
* 7.4.2 Database Functions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 84
* 7.5 Don’t Drop Down to Raw SQL Until It’s Necessary . . . . . . . . . . . . . . . . 85
* 7.6 Add Indexes as Needed . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 86
* 7.7 Transactions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 87
* 7.7.1 Wrapping Each HTTP Request in a Transaction . . . . . . . . . . . . . 87
* 7.7.2 Explicit Transaction Declaration . . . . . . . . . . . . . . . . . . . . . . 90
* 7.7.3 django.http.StreamingHttpResponse and Transactions . . . . . . . . . . 91
* 7.7.4 Transactions in MySQL . . . . . . . . . . . . . . . . . . . . . . . . . . 92
* 7.7.5 Django ORM Transaction Resources . . . . . . . . . . . . . . . . . . . . 92
* 7.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 92
* 8 Function- and Class-Based Views 93
* 8.1 When to Use FBVs or CBVs . . . . . . . . . . . . . . . . . . . . . . . . . . . . 93
* 8.2 Keep View Logic Out of URLConfs . . . . . . . . . . . . . . . . . . . . . . . . 95
* 8.3 Stick to Loose Coupling in URLConfs . . . . . . . . . . . . . . . . . . . . . . . 96
* 8.3.1 What if We Aren’t Using CBVs? . . . . . . . . . . . . . . . . . . . . . . 99
* 8.4 Use URL Namespaces . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99
* 8.4.1 Makes for Shorter, More Obvious and Don’t Repeat Yourself URL Names 100
* 8.4.2 Increases Interoperability With Third-Party Libraries . . . . . . . . . . . 101
* 8.4.3 Easier Searches, Upgrades, and Refactors . . . . . . . . . . . . . . . . . 102
* 8.4.4 Allows for More App and Template Reverse Tricks . . . . . . . . . . . . 102
* 8.5 Don’t Reference Views as Strings in URLConfs . . . . . . . . . . . . . . . . . . 102
* 8.6 Try to Keep Business Logic Out of Views . . . . . . . . . . . . . . . . . . . . . 103
* 8.7 Django Views Are Functions . . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
* 8.7.1 The Simplest Views . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
* 8.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 105
* 9 Best Practices for Function-Based Views 107
* 9.1 Advantages of FBVs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 107
* 9.2 Passing the HttpRequest Object . . . . . . . . . . . . . . . . . . . . . . . . . . 108
* 9.3 Decorators Are Sweet . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 111
* 9.3.1 Be Conservative With Decorators . . . . . . . . . . . . . . . . . . . . . 113
* 9.3.2 Additional Resources on Decorators . . . . . . . . . . . . . . . . . . . . 114
* 9.4 Passing the HttpResponse Object . . . . . . . . . . . . . . . . . . . . . . . . . . 114
* 9.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 114
* 10 Best Practices for Class-Based Views 115
* 10.1 Guidelines When Working With CBVs . . . . . . . . . . . . . . . . . . . . . . 116
* 10.2 Using Mixins With CBVs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 116
* 10.3 Which Django GCBV Should Be Used for What Task? . . . . . . . . . . . . . . 118
* 10.4 General Tips for Django CBVs . . . . . . . . . . . . . . . . . . . . . . . . . . . 119
* 10.4.1 Constraining Django CBV/GCBV Access to Authenticated Users . . . . 120
* 10.4.2 Performing Custom Actions on Views With Valid Forms . . . . . . . . . 120
* 10.4.3 Performing Custom Actions on Views With Invalid Forms . . . . . . . . 121
* 10.4.4 Using the View Object . . . . . . . . . . . . . . . . . . . . . . . . . . . 122
* 10.5 How GCBVs and Forms Fit Together . . . . . . . . . . . . . . . . . . . . . . . 124
* 10.5.1 Views + ModelForm Example . . . . . . . . . . . . . . . . . . . . . . . 125
* 10.5.2 Views + Form Example . . . . . . . . . . . . . . . . . . . . . . . . . . . 129
* 10.6 Using Just django.views.generic.View . . . . . . . . . . . . . . . . . . . . . . . . 131
* 10.7 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133
* 10.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134
* 11 Form Fundamentals 135
* 11.1 Validate All Incoming Data With Django Forms . . . . . . . . . . . . . . . . . . 135
* 11.2 Use the POST Method in HTML Forms . . . . . . . . . . . . . . . . . . . . . 138
* 11.3 Always Use CSRF Protection With HTTP Forms That Modify Data . . . . . . . 138
* 11.3.1 Posting Data via AJAX . . . . . . . . . . . . . . . . . . . . . . . . . . . 139
* 11.4 Understand How to Add Django Form Instance Attributes . . . . . . . . . . . . 139
* 11.5 Know How Form Validation Works . . . . . . . . . . . . . . . . . . . . . . . . . 141
* 11.5.1 ModelForm Data Is Saved to the Form, Then the Model Instance . . . . 142
* 11.6 Fields Without Pre-Made Widgets . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 11.7 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 11.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 12 Common Patterns for Forms 145
* 12.1 Pattern 1: Simple ModelForm With Default Validators . . . . . . . . . . . . . . 146
* 12.2 Pattern 2: Custom Form Field Validators in ModelForms . . . . . . . . . . . . . 147
* 12.3 Pattern 3: Overriding the Clean Stage of Validation . . . . . . . . . . . . . . . . 152
* 12.4 Pattern 4: Hacking Form Fields (2 CBVs, 2 Forms, 1 Model) . . . . . . . . . . . 155
* 12.5 Pattern 5: Reusable Search Mixin View . . . . . . . . . . . . . . . . . . . . . . . 159
* 12.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161
* 13 Templates: Best Practices 163
* 13.1 Keep Templates Mostly in templates/ . . . . . . . . . . . . . . . . . . . . . . 163
* 13.2 Template Architecture Patterns . . . . . . . . . . . . . . . . . . . . . . . . . . . 164
* 13.2.1 2-Tier Template Architecture Example . . . . . . . . . . . . . . . . . . . 164
* 13.2.2 3-Tier Template Architecture Example . . . . . . . . . . . . . . . . . . . 165
* 13.2.3 Flat Is Better Than Nested . . . . . . . . . . . . . . . . . . . . . . . . . 166
* 13.3 Limit Processing in Templates . . . . . . . . . . . . . . . . . . . . . . . . . . . 167
* 13.3.1 Gotcha 1: Aggregation in Templates . . . . . . . . . . . . . . . . . . . . 169
* 13.3.2 Gotcha 2: Filtering With Conditionals in Templates . . . . . . . . . . . 171
* 13.3.3 Gotcha 3: Complex Implied Queries in Templates . . . . . . . . . . . . . 173
* 13.3.4 Gotcha 4: Hidden CPU Load in Templates . . . . . . . . . . . . . . . . 174
* 13.3.5 Gotcha 5: Hidden REST API Calls in Templates . . . . . . . . . . . . . 175
* 13.4 Don’t Bother Making Your Generated HTML Pretty . . . . . . . . . . . . . . . 175
* 10.7 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133
* 10.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134
* 11 Form Fundamentals 135
* 11.1 Validate All Incoming Data With Django Forms . . . . . . . . . . . . . . . . . . 135
* 11.2 Use the POST Method in HTML Forms . . . . . . . . . . . . . . . . . . . . . 138
* 11.3 Always Use CSRF Protection With HTTP Forms That Modify Data . . . . . . . 138
* 11.3.1 Posting Data via AJAX . . . . . . . . . . . . . . . . . . . . . . . . . . . 139
* 11.4 Understand How to Add Django Form Instance Attributes . . . . . . . . . . . . 139
* 11.5 Know How Form Validation Works . . . . . . . . . . . . . . . . . . . . . . . . . 141
* 11.5.1 ModelForm Data Is Saved to the Form, Then the Model Instance . . . . 142
* 11.6 Fields Without Pre-Made Widgets . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 11.7 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 11.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
* 12 Common Patterns for Forms 145
* 12.1 Pattern 1: Simple ModelForm With Default Validators . . . . . . . . . . . . . . 146
* 12.2 Pattern 2: Custom Form Field Validators in ModelForms . . . . . . . . . . . . . 147
* 12.3 Pattern 3: Overriding the Clean Stage of Validation . . . . . . . . . . . . . . . . 152
* 12.4 Pattern 4: Hacking Form Fields (2 CBVs, 2 Forms, 1 Model) . . . . . . . . . . . 155
* 12.5 Pattern 5: Reusable Search Mixin View . . . . . . . . . . . . . . . . . . . . . . . 159
* 12.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161
* 13 Templates: Best Practices 163
* 13.1 Keep Templates Mostly in templates/ . . . . . . . . . . . . . . . . . . . . . . 163
* 13.2 Template Architecture Patterns . . . . . . . . . . . . . . . . . . . . . . . . . . . 164
* 13.2.1 2-Tier Template Architecture Example . . . . . . . . . . . . . . . . . . . 164
* 13.2.2 3-Tier Template Architecture Example . . . . . . . . . . . . . . . . . . . 165
* 13.2.3 Flat Is Better Than Nested . . . . . . . . . . . . . . . . . . . . . . . . . 166
* 13.3 Limit Processing in Templates . . . . . . . . . . . . . . . . . . . . . . . . . . . 167
* 13.3.1 Gotcha 1: Aggregation in Templates . . . . . . . . . . . . . . . . . . . . 169
* 13.3.2 Gotcha 2: Filtering With Conditionals in Templates . . . . . . . . . . . 171
* 13.3.3 Gotcha 3: Complex Implied Queries in Templates . . . . . . . . . . . . . 173
* 13.3.4 Gotcha 4: Hidden CPU Load in Templates . . . . . . . . . . . . . . . . 174
* 13.3.5 Gotcha 5: Hidden REST API Calls in Templates . . . . . . . . . . . . . 175
* 13.4 Don’t Bother Making Your Generated HTML Pretty . . . . . . . . . . . . . . . 175
* 15.3.2 Using Template Tags in Jinja2 Templates . . . . . . . . . . . . . . . . . 196
* 15.3.3 Using Django-Style Template Filters in Jinja2 Templates . . . . . . . . . 196
* 15.3.4 Context Processors Aren’t Called by Jinja2 Templates . . . . . . . . . . . 198
* 15.3.5 The Jinja2 Environment Object Should Be Considered Static . . . . . . . 200
* 15.4 Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 201
* 15.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 201
* 16 Building REST APIs 203
* 16.1 Fundamentals of Basic REST API Design . . . . . . . . . . . . . . . . . . . . . 204
* 16.2 Implementing a Simple JSON API . . . . . . . . . . . . . . . . . . . . . . . . . 206
* 16.3 REST API Architecture . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 208
* 16.3.1 Code for an App Should Remain in the App . . . . . . . . . . . . . . . . 209
* 16.3.2 Code for Project Should Be Neatly Organized . . . . . . . . . . . . . . . 209
* 16.3.3 Try to Keep Business Logic Out of API Views . . . . . . . . . . . . . . 209
* 16.3.4 Grouping API URLs . . . . . . . . . . . . . . . . . . . . . . . . . . . . 210
* 16.3.5 Test Your API . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 212
* 16.3.6 Version Your API . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 212
* 16.4 Service-Oriented Architecture . . . . . . . . . . . . . . . . . . . . . . . . . . . 212
* 16.5 Shutting Down an External API . . . . . . . . . . . . . . . . . . . . . . . . . . 213
* 16.5.1 Step #1: Notify Users of Pending Shut Down . . . . . . . . . . . . . . . 213
* 16.5.2 Step #2: Replace API With 410 Error View . . . . . . . . . . . . . . . . 214
* 16.6 Evaluating REST Frameworks . . . . . . . . . . . . . . . . . . . . . . . . . . . 214
* 16.6.1 Django Rest Framework Is the Defacto Package . . . . . . . . . . . . . . 215
* 16.6.2 How Much Boilerplate Do You Want to Write? . . . . . . . . . . . . . . 215
* 16.6.3 Are Remote Procedure Calls Easy to Implement? . . . . . . . . . . . . . 215
* 16.6.4 CBVs or FBVs? . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 216
* 16.7 Rate Limiting Your API . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 216
* 16.7.1 Unfettered API Access is Dangerous . . . . . . . . . . . . . . . . . . . . 216
* 16.7.2 Rest Frameworks Must Come with Rate Limiting . . . . . . . . . . . . . 217
* 16.7.3 Rate Limit Can Be A Business Plan . . . . . . . . . . . . . . . . . . . . 217
* 16.8 Advertising Your REST API . . . . . . . . . . . . . . . . . . . . . . . . . . . . 217
* 16.8.1 Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218
* 16.8.2 Provide Client SDKs . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218
* 16.9 Additional Reading . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218
* 16.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218
* 17 Consuming REST APIs 221
* 17.1 Learn How to Debug the Client . . . . . . . . . . . . . . . . . . . . . . . . . . 222
* 17.2 Consider Using JavaScript-Powered Static Asset Preprocessors . . . . . . . . . . 223
* 17.3 Making Content Indexable by Search Engines . . . . . . . . . . . . . . . . . . . 223
* 17.3.1 Read the Search Engine Documentation . . . . . . . . . . . . . . . . . . 223
* 17.3.2 Hand-Craft the sitemap.xml . . . . . . . . . . . . . . . . . . . . . . . . 224
* 17.3.3 Use a Service to Make Your Site Crawlable . . . . . . . . . . . . . . . . 225
* 17.4 Real-Time Woes a.k.a. Latency . . . . . . . . . . . . . . . . . . . . . . . . . . . 225
* 17.4.1 Solution: Mask the Latency With Animations . . . . . . . . . . . . . . . 225
* 17.4.2 Solution: Fake Successful Transactions . . . . . . . . . . . . . . . . . . . 226
* 17.4.3 Solution: Geographically Based Servers . . . . . . . . . . . . . . . . . . 226
* 17.4.4 Solution: Restrict Users Geographically . . . . . . . . . . . . . . . . . . 226
* 17.5 Avoid the Anti-Patterns . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 226
* 17.5.1 Building Single Page Apps When Multi-Page Apps Suffice . . . . . . . . 227
* 17.5.2 Not Writing Tests . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 227
* 17.5.3 Not Understanding JavaScript Memory Management . . . . . . . . . . . 227
* 17.5.4 Storing Data in the DOM When It’s Not jQuery . . . . . . . . . . . . . 227
* 17.6 AJAX and the CSRF Token . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 228
* 17.6.1 JQuery and the CSRF Token . . . . . . . . . . . . . . . . . . . . . . . . 228
* 17.6.2 Backbone.js and the CSRF Token . . . . . . . . . . . . . . . . . . . . . 230
* 17.6.3 AngularJS and the CSRF Token . . . . . . . . . . . . . . . . . . . . . . 230
* 17.7 Improving JavaScript Skills . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 231
* 17.7.1 Assessing Skill Levels . . . . . . . . . . . . . . . . . . . . . . . . . . . . 231
* 17.7.2 Learn More JavaScript! . . . . . . . . . . . . . . . . . . . . . . . . . . . 231
* 17.8 Follow JavaScript Coding Standards . . . . . . . . . . . . . . . . . . . . . . . . 231
* 17.9 Useful Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 231
* 17.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 232
* 18 Tradeoffs of Replacing Core Components 233
* 18.1 The Temptation to Build FrankenDjango . . . . . . . . . . . . . . . . . . . . . . 234
* 18.2 Non-Relational Databases vs. Relational Databases . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 235
* 18.2.1 Not All Non-Relational Databases Are ACID Compliant . . . . . . . . . 235
* 18.2.2 Don’t Use Non-Relational Databases for Relational Tasks . . . . . . . . . 236
* 18.2.3 Ignore the Hype and Do Your Own Research . . . . . . . . . . . . . . . 236
* 18.2.4 How We Use Non-Relational Databases With Django . . . . . . . . . . 237
* 18.3 What About Replacing the Django Template Language? . . . . . . . . . . . . . 237
* 18.4 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 237
* 19 Working With the Django Admin 239
* 19.1 It’s Not for End Users . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 240
* 19.2 Admin Customization vs. New Views . . . . . . . . . . . . . . . . . . . . . . . 240
* 19.3 Viewing String Representations of Objects . . . . . . . . . . . . . . . . . . . . . 240
* 19.4 Adding Callables to ModelAdmin Classes . . . . . . . . . . . . . . . . . . . . . 244
* 19.5 Don’t Use list editable in Multiuser Environments . . . . . . . . . . . . . . . . . 245
* 19.6 Django’s Admin Documentation Generator . . . . . . . . . . . . . . . . . . . . 246
* 19.7 Securing the Django Admin and Django Admin Docs . . . . . . . . . . . . . . . 247
* 19.8 Using Custom Skins With the Django Admin . . . . . . . . . . . . . . . . . . . 247
* 19.8.1 Evaluation Point: Documentation is Everything . . . . . . . . . . . . . . 248
* 19.8.2 Write Tests for Any Admin Extensions You Create . . . . . . . . . . . . 248
* 19.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 249
* 20 Dealing With the User Model 251
* 20.1 Use Django’s Tools for Finding the User Model . . . . . . . . . . . . . . . . . . 251
* 20.1.1 Use settings.AUTH USER MODEL for Foreign Keys to User . . . . . 252
* 20.1.2 Don’t Use get user model() for Foreign Keys to User . . . . . . . . . . . 252
* 20.2 Migrating Pre-1.5 User Models to 1.5+’s Custom User Models . . . . . . . . . . 253
* 20.3 Custom User Fields for Django 1.8 Projects . . . . . . . . . . . . . . . . . . . . 253
* 20.3.1 Option 1: Subclass AbstractUser . . . . . . . . . . . . . . . . . . . . . . 254
* 20.3.2 Option 2: Subclass AbstractBaseUser . . . . . . . . . . . . . . . . . . . . 255
* 20.3.3 Option 3: Linking Back From a Related Model . . . . . . . . . . . . . . 255
* 20.4 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 257
* 21 Django’s Secret Sauce: Third-Party Packages 259
* 21.1 Examples of Third-Party Packages . . . . . . . . . . . . . . . . . . . . . . . . . 260
* 21.2 Know About the Python Package Index . . . . . . . . . . . . . . . . . . . . . . 260
* 21.3 Know About DjangoPackages.com . . . . . . . . . . . . . . . . . . . . . . . . . 261
* 21.4 Know Your Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 261
* 21.5 Tools for Installing and Managing Packages . . . . . . . . . . . . . . . . . . . . 261
* 21.6 Package Requirements . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 262
* 21.7 Wiring Up Django Packages: The Basics . . . . . . . . . . . . . . . . . . . . . . 262
* 21.7.1 Step 1: Read the Documentation for the Package . . . . . . . . . . . . . 262
* 21.7.2 Step 2: Add Package and Version Number to Your Requirements . . . . . 262
* 21.7.3 Step 3: Install the Requirements Into Your Virtualenv . . . . . . . . . . . 263
* 21.7.4 Step 4: Follow the Package’s Installation Instructions Exactly . . . . . . . 264
* 21.8 Troubleshooting Third-Party Packages . . . . . . . . . . . . . . . . . . . . . . . 264
* 21.9 Releasing Your Own Django Packages . . . . . . . . . . . . . . . . . . . . . . . 264
* 21.10 What Makes a Good Django Package? . . . . . . . . . . . . . . . . . . . . . . . 265
* 21.10.1 Purpose . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 265
* 21.10.2 Scope . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 266
* 21.10.3 Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 266
* 21.10.4 Tests . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 266
* 21.10.5 Templates . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 266
* 21.10.6 Activity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 267
* 21.10.7 Community . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 267
* 21.10.8 Modularity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 267
* 21.10.9 Availability on PyPI . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 267
* 21.10.10 Uses the Broadest Requirements Specifiers Possible . . . . . . . . . . . . 268
* 21.10.11 Proper Version Numbers . . . . . . . . . . . . . . . . . . . . . . . . . . 269
* 21.10.12 Name . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 270
* 21.10.13 License . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 271
* 21.10.14 Clarity of Code . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 271
* 21.10.15 Use URL Namespaces . . . . . . . . . . . . . . . . . . . . . . . . . . . 271
* 21.11 Creating Your Own Packages the Easy Way . . . . . . . . . . . . . . . . . . . . 272
* 21.12 Maintaining Your Open Source Package . . . . . . . . . . . . . . . . . . . . . . 272
* 21.12.1 Give Credit for Pull Requests . . . . . . . . . . . . . . . . . . . . . . . . 273
* 21.12.2 Handling Bad Pull Requests . . . . . . . . . . . . . . . . . . . . . . . . 273
* 21.12.3 Do Formal PyPI Releases . . . . . . . . . . . . . . . . . . . . . . . . . . 274
* 21.12.4 Create and Deploy Wheels to PyPI . . . . . . . . . . . . . . . . . . . . 275
* 21.12.5 Upgrade the Package to New Versions of Django . . . . . . . . . . . . . 276
* 21.12.6 Follow Good Security Practices . . . . . . . . . . . . . . . . . . . . . . . 276
* 21.12.7 Provide Sample Base Templates . . . . . . . . . . . . . . . . . . . . . . 277
* 21.12.8 Give the Package Away . . . . . . . . . . . . . . . . . . . . . . . . . . . 277
* 21.13 Additional Reading . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 277
* 21.14 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 278
* 22 Testing Stinks and Is a Waste of Money! 279
* 22.1 Testing Saves Money, Jobs, and Lives . . . . . . . . . . . . . . . . . . . . . . . . 279
* 22.2 How to Structure Tests . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 280
* 22.3 How to Write Unit Tests . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 281
* 22.3.1 Each Test Method Tests One Thing . . . . . . . . . . . . . . . . . . . . 281
* 22.3.2 For Views, When Possible Use the Request Factory . . . . . . . . . . . . 284
* 22.3.3 Don’t Write Tests That Have to Be Tested . . . . . . . . . . . . . . . . . 285
* 22.3.4 Don’t Repeat Yourself Doesn’t Apply to Writing Tests . . . . . . . . . . . 285
* 22.3.5 Don’t Rely on Fixtures . . . . . . . . . . . . . . . . . . . . . . . . . . . 286
* 22.3.6 Things That Should Be Tested . . . . . . . . . . . . . . . . . . . . . . . 286
* 22.3.7 Test for Failure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 287
* 22.3.8 Use Mock to Keep Unit Tests From Touching the World . . . . . . . . . 288
* 22.3.9 Use Fancier Assertion Methods . . . . . . . . . . . . . . . . . . . . . . . 290
* 22.3.10 Document the Purpose of Each Test . . . . . . . . . . . . . . . . . . . . 291
* 22.4 What About Integration Tests? . . . . . . . . . . . . . . . . . . . . . . . . . . . 291
* 22.5 Continuous Integration . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 292
* 22.6 Who Cares? We Don’t Have Time for Tests! . . . . . . . . . . . . . . . . . . . . 292
* 22.7 The Game of Test Coverage . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 293
* 22.8 Setting Up the Test Coverage Game . . . . . . . . . . . . . . . . . . . . . . . . 293
* 22.8.1 Step 1: Start Writing Tests . . . . . . . . . . . . . . . . . . . . . . . . . 293
* 22.8.2 Step 2: Run Tests and Generate Coverage Report . . . . . . . . . . . . . 294
* 22.8.3 Step 3: Generate the Report! . . . . . . . . . . . . . . . . . . . . . . . . 294
* 22.9 Playing the Game of Test Coverage . . . . . . . . . . . . . . . . . . . . . . . . . 295
* 22.10 Alternatives to unittest . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 295
* 22.11 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 296
* 23 Documentation: Be Obsessed 297
* 23.1 Use reStructuredText for Python Docs . . . . . . . . . . . . . . . . . . . . . . . 297
* 23.2 Use Sphinx to Generate Documentation From reStructuredText . . . . . . . . . . 299
* 23.3 What Docs Should Django Projects Contain? . . . . . . . . . . . . . . . . . . . 299
* 23.4 Additional Documentation Resources . . . . . . . . . . . . . . . . . . . . . . . . 301
* 23.5 The Markdown Alternative . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 301
* 23.5.1 README.md to README.rst: Using Pandoc for Packages Uploaded to PyPI . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 302
* 23.5.2 Markdown Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . 302
* 23.6 Wikis and Other Documentation Methods . . . . . . . . . . . . . . . . . . . . . 303
* 23.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 303
* 24 Finding and Reducing Bottlenecks 305
* 24.1 Should You Even Care? . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 305
* 24.2 Speed Up Query-Heavy Pages . . . . . . . . . . . . . . . . . . . . . . . . . . . 305
* 24.2.1 Find Excessive Queries With Django Debug Toolbar . . . . . . . . . . . 305
* 24.2.2 Reduce the Number of Queries . . . . . . . . . . . . . . . . . . . . . . . 306
* 24.2.3 Speed Up Common Queries . . . . . . . . . . . . . . . . . . . . . . . . 307
* 24.2.4 Switch ATOMIC REQUESTS to False . . . . . . . . . . . . . . . . . . 308
* 24.3 Get the Most Out of Your Database . . . . . . . . . . . . . . . . . . . . . . . . 308
* 24.3.1 Know What Doesn’t Belong in the Database . . . . . . . . . . . . . . . . 308
* 24.3.2 Getting the Most Out of PostgreSQL . . . . . . . . . . . . . . . . . . . 309
* 24.3.3 Getting the Most Out of MySQL . . . . . . . . . . . . . . . . . . . . . 309
* 24.4 Cache Queries With Memcached or Redis . . . . . . . . . . . . . . . . . . . . . 310
* 24.5 Identify Specific Places to Cache . . . . . . . . . . . . . . . . . . . . . . . . . . 310
* 24.6 Consider Third-Party Caching Packages . . . . . . . . . . . . . . . . . . . . . . 310
* 24.7 Compression and Minification of HTML, CSS, and JavaScript . . . . . . . . . . 311
* 24.8 Use Upstream Caching or a Content Delivery Network . . . . . . . . . . . . . . 312
* 24.9 Other Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 312
* 24.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 314
* 25 Asynchronous Task Queues 315
* 25.1 Do We Need a Task Queue? . . . . . . . . . . . . . . . . . . . . . . . . . . . . 316
* 25.2 Choosing Task Queue Software . . . . . . . . . . . . . . . . . . . . . . . . . . . 317
* 25.3 Best Practices for Task Queues . . . . . . . . . . . . . . . . . . . . . . . . . . . 318
* 25.3.1 Treat Tasks Like Views . . . . . . . . . . . . . . . . . . . . . . . . . . . 318
* 25.3.2 Tasks Aren’t Free . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 318
* 25.3.3 Only Pass JSON-Serializable Values to Task Functions . . . . . . . . . . 319
* 25.3.4 Learn How to Monitor Tasks and Workers . . . . . . . . . . . . . . . . 319
* 25.3.5 Logging! . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 319
* 25.3.6 Monitor the Backlog . . . . . . . . . . . . . . . . . . . . . . . . . . . . 320
* 25.3.7 Periodically Clear Out Dead Tasks . . . . . . . . . . . . . . . . . . . . . 320
* 25.3.8 Ignore Results We Don’t Need . . . . . . . . . . . . . . . . . . . . . . . 320
* 25.3.9 Use the Queue’s Error Handling . . . . . . . . . . . . . . . . . . . . . . 320
* 25.3.10 All Tasks Should Accept Kwargs . . . . . . . . . . . . . . . . . . . . . . 321
* 25.3.11 Learn the Features of Your Task Queue Software . . . . . . . . . . . . . 321
* 25.4 Resources for Task Queues . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 321
* 25.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 322
* 26 Security Best Practices 323
* 26.1 Harden Your Servers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 323
* 26.2 Know Django’s Security Features . . . . . . . . . . . . . . . . . . . . . . . . . . 323
* 26.3 Turn Off DEBUG Mode in Production . . . . . . . . . . . . . . . . . . . . . . 324
* 26.4 Keep Your Secret Keys Secret . . . . . . . . . . . . . . . . . . . . . . . . . . . . 324
* 26.5 HTTPS Everywhere . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 324
* 26.5.1 Use Secure Cookies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 326
* 26.5.2 Use HTTP Strict Transport Security (HSTS) . . . . . . . . . . . . . . . 326
* 26.5.3 HTTPS Configuration Tools . . . . . . . . . . . . . . . . . . . . . . . . 328
* 26.6 Use Allowed Hosts Validation . . . . . . . . . . . . . . . . . . . . . . . . . . . . 328
* 26.7 Always Use CSRF Protection With HTTP Forms That Modify Data . . . . . . . 328
* 26.8 Prevent Against Cross-Site Scripting (XSS) Attacks . . . . . . . . . . . . . . . . 328
* 26.8.1 Use Django Templates Over mark safe . . . . . . . . . . . . . . . . . . . 329
* 26.8.2 Don’t Allow Users to Set Individual HTML Tag Attributes . . . . . . . . 329
* 26.8.3 Use JSON Encoding for Data Consumed by JavaScript . . . . . . . . . . 329
* 26.8.4 Additional Reading . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 329
* 26.9 Defend Against Python Code Injection Attacks . . . . . . . . . . . . . . . . . . 329
* 26.9.1 Python Built-Ins That Execute Code . . . . . . . . . . . . . . . . . . . . 330
* 26.9.2 Python Standard Library Modules That Can Execute Code . . . . . . . . 330
* 26.9.3 Third-Party Libraries That Can Execute Code . . . . . . . . . . . . . . . 330
* 26.9.4 Be Careful With Cookie-Based Sessions . . . . . . . . . . . . . . . . . . 331
* 26.10 Validate All Incoming Data With Django Forms . . . . . . . . . . . . . . . . . . 332
* 26.11 Disable the Autocomplete on Payment Fields . . . . . . . . . . . . . . . . . . . 332
* 26.12 Handle User-Uploaded Files Carefully . . . . . . . . . . . . . . . . . . . . . . . 333
* 26.12.1 When a CDN Is Not an Option . . . . . . . . . . . . . . . . . . . . . . 333
* 26.12.2 Django and User-Uploaded Files . . . . . . . . . . . . . . . . . . . . . . 334
* 26.13 Don’t Use ModelForms.Meta.exclude . . . . . . . . . . . . . . . . . . . . . . . . 334
* 26.13.1 Mass Assignment Vulnerabilities . . . . . . . . . . . . . . . . . . . . . . 337
* 26.14 Don’t Use ModelForms.Meta.fields = " all " . . . . . . . . . . . . . . . 337
* 26.15 Beware of SQL Injection Attacks . . . . . . . . . . . . . . . . . . . . . . . . . . 337
* 26.16 Never Store Credit Card Data . . . . . . . . . . . . . . . . . . . . . . . . . . . . 338
* 26.17 Secure the Django Admin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 338
* 26.17.1 Change the Default Admin URL . . . . . . . . . . . . . . . . . . . . . . 339
* 26.17.2 Use django-admin-honeypot . . . . . . . . . . . . . . . . . . . . . . . . 339
* 26.17.3 Only Allow Admin Access via HTTPS . . . . . . . . . . . . . . . . . . 339
* 26.17.4 Limit Admin Access Based on IP . . . . . . . . . . . . . . . . . . . . . 340
* 26.17.5 Use the allow tags Attribute With Caution . . . . . . . . . . . . . . . . 340
* 26.18 Secure the Admin Docs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 340
* 26.19 Monitor Your Sites . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 340
* 26.20 Keep Your Dependencies Up-to-Date . . . . . . . . . . . . . . . . . . . . . . . 341
* 26.21 Prevent Clickjacking . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 341
* 26.22 Guard Against XML Bombing With defusedxml . . . . . . . . . . . . . . . . . 341
* 26.23 Explore Two-Factor Authentication . . . . . . . . . . . . . . . . . . . . . . . . 342
* 26.24 Embrace SecurityMiddleware . . . . . . . . . . . . . . . . . . . . . . . . . . . . 343
* 26.25 Force the Use of Strong Passwords . . . . . . . . . . . . . . . . . . . . . . . . . 343
* 26.26 Give Your Site a Security Checkup . . . . . . . . . . . . . . . . . . . . . . . . . 343
* 26.27 Put Up a Vulnerability Reporting Page . . . . . . . . . . . . . . . . . . . . . . . 344
* 26.28 Stop Using django.utils.html.remove tag . . . . . . . . . . . . . . . . . . . . . . 344
* 26.29 Have a Plan Ready for When Things Go Wrong . . . . . . . . . . . . . . . . . . 344
* 26.29.1 Shut Everything Down or Put It in Read-Only Mode . . . . . . . . . . . 345
* 26.29.2 Put Up a Static HTML Page . . . . . . . . . . . . . . . . . . . . . . . . 345
* 26.29.3 Back Everything Up . . . . . . . . . . . . . . . . . . . . . . . . . . . . 345
* 26.29.4 Email security@djangoproject.com, Even if It’s Your Fault . . . . . . . . 346
* 26.29.5 Start Looking Into the Problem . . . . . . . . . . . . . . . . . . . . . . 346
* 26.30 Keep Up-to-Date on General Security Practices . . . . . . . . . . . . . . . . . . 347
* 26.31 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 348
* 27 Logging: What’s It For, Anyway? 349
* 27.1 Application Logs vs. Other Logs . . . . . . . . . . . . . . . . . . . . . . . . . . 349
* 27.2 Why Bother With Logging? . . . . . . . . . . . . . . . . . . . . . . . . . . . . 350
* 27.3 When to Use Each Log Level . . . . . . . . . . . . . . . . . . . . . . . . . . . . 350
* 27.3.1 Log Catastrophes With CRITICAL . . . . . . . . . . . . . . . . . . . . 351
* 27.3.2 Log Production Errors With ERROR . . . . . . . . . . . . . . . . . . . 351
* 27.3.3 Log Lower-Priority Problems With WARNING . . . . . . . . . . . . . 352
* 27.3.4 Log Useful State Information With INFO . . . . . . . . . . . . . . . . . 353
* 27.3.5 Log Debug-Related Messages to DEBUG . . . . . . . . . . . . . . . . . 353
* 27.4 Log Tracebacks When Catching Exceptions . . . . . . . . . . . . . . . . . . . . 355
* 27.5 One Logger Per Module That Uses Logging . . . . . . . . . . . . . . . . . . . . 356
* 27.6 Log Locally to Rotating Files . . . . . . . . . . . . . . . . . . . . . . . . . . . . 356
* 27.7 Other Logging Tips . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 357
* 27.8 Necessary Reading Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 357
* 27.9 Useful Third-Party Tools . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 358
* 27.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 358
* 28 Signals: Use Cases and Avoidance Techniques 359
* 28.1 When to Use and Avoid Signals . . . . . . . . . . . . . . . . . . . . . . . . . . 359
* 28.2 Signal Avoidance Techniques . . . . . . . . . . . . . . . . . . . . . . . . . . . . 360
* 28.2.1 Using Custom Model Manager Methods Instead of Signals . . . . . . . . 360
* 28.2.2 Validate Your Model Elsewhere . . . . . . . . . . . . . . . . . . . . . . . 363
* 28.2.3 Override Your Model’s Save or Delete Method Instead . . . . . . . . . . 363
* 28.2.4 Use a Helper Function Instead of Signals . . ... ..  .. ..  .  ... . . . . . 364
* 28.3 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 364
* 29 What About Those Random Utilities? 365
* 29.1 Create a Core App for Your Utilities . . . . . . . . . . . . . . . . . . . . . . . . 365
* 29.2 Django’s Own Swiss Army Knife . . . . . . . . . . . . . . . . . . . . . . . . . . 366
* 29.2.1 django.contrib.humanize . . . . . . . . . . . . . . . . . . . . . . . . . . 367
* 29.2.2 django.utils.decorators.method decorator(decorator) . . . . . . . . . . . . 367
* 29.2.3 django.utils.decorators.decorator from middleware(middleware) . . . . . 367
* 29.2.4 django.utils.encoding.force text(value) . . . . . . . . . . . . . . . . . . . 368
* 29.2.5 django.utils.functional.cached property . . . . . . . . . . . . . . . . . . . 368
* 29.2.6 django.utils.html.format html(format str, *args, **kwargs) . . . . . . . . . 369
* 29.2.7 django.utils.html.remove tags(value, tags) . . . . . . . . . . . . . . . . . 369
* 29.2.8 django.utils.html.strip tags(value) . . . . . . . . . . . . . . . . . . . . . . 369
* 29.2.9 django.utils.six . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 369
* 29.2.10 django.utils.text.slugify(value) . . . . . . . . . . . . . . . . . . . . . . . . 370
* 29.2.11 django.utils.timezone . . . . . . . . . . . . . . . . . . . . . . . . . . . . 371
* 29.2.12 django.utils.translation . . . . . . . . . . . . . . . . . . . . . . . . . . . 372
* 29.3 Exceptions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 372
* 29.3.1 django.core.exceptions.ImproperlyConfigured . . . . . . . . . . . . . . . 372
* 29.3.2 django.core.exceptions.ObjectDoesNotExist . . . . . . . . . . . . . . . . 372
* 29.3.3 django.core.exceptions.PermissionDenied . . . . . . . . . . . . . . . . . 373
* 29.4 Serializers and Deserializers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 374
* 29.4.1 django.core.serializers.json.DjangoJSONEncoder . . . . . . . . . . . . . 377
* 29.4.2 django.core.serializers.pyyaml . . . . . . . . . . . . . . . . . . . . . . . . 377
* 29.4.3 django.core.serializers.xml serializer . . . . . . . . . . . . . . . . . . . . 378
* 29.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 378
* 30 Deployment: Platforms as a Service 379
* 30.1 Evaluating a PaaS . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 380
* 30.1.1 Compliance . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 380
* 30.1.2 Pricing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 381
* 30.1.3 Uptime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 381
* 30.1.4 Staffing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 382
* 30.1.5 Scaling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 382
* 30.1.6 Documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 383
* 30.1.7 Performance Degradation . . . . . . . . . . . . . . . . . . . . . . . . . . 383
* 30.1.8 Geography . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 384
* 30.1.9 Company Stability . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 384
* 30.2 Best Practices for Deploying to PaaS . . . . . . . . . . . . . . . . . . . . . . . . 384
* 30.2.1 Aim for Identical Environments . . . . . . . . . . . . . . . . . . . . . . 384
* 30.2.2 Automate All the Things! . . . . . . . . . . . . . . . . . . . . . . . . . . 385
* 30.2.3 Maintain a Staging Instance . . . . . . . . . . . . . . . . . . . . . . . . 385
* 30.2.4 Prepare for Disaster With Backups and Rollbacks . . . . . . . . . . . . . 385
* 30.2.5 Keep External Backups . . . . . . . . . . . . . . . . . . . . . . . . . . . 386
* 30.3 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 386
* 31 Deploying Django Projects 387
* 31.1 Single-Server for Small Projects . . . . . . . . . . . . . . . . . . . . . . . . . . . 387
* 31.1.1 Should You Bother? . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 387
* 31.1.2 Example: Quick Ubuntu + Gunicorn Setup . . . . . . . . . . . . . . . . 388
* 31.2 Multi-Server for Medium to Large Projects . . . . . . . . . . . . . . . . . . . . 389
* 31.2.1 Advanced Multi-Server Setup . . . . . . . . . . . . . . . . . . . . . . . 392
* 31.3 WSGI Application Servers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 393
* 31.4 Performance and Tuning: uWSGI and Gunicorn . . . . . . . . . . . . . . . . . . 394
* 31.5 Stability and Ease of Setup: Gunicorn and Apache . . . . . . . . . . . . . . . . . 395
* 31.6 Common Apache Gotchas . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 395
* 31.6.1 Apache and Environment Variables . . . . . . . . . . . . . . . . . . . . . 395
* 31.6.2 Apache and Virtualenv . . . . . . . . . . . . . . . . . . . . . . . . . . . 396
* 31.7 Automated, Repeatable Deployments . . . . . . . . . . . . . . . . . . . . . . . . 396
* 31.7.1 A Rapidly Changing World . . . . . . . . . . . . . . . . . . . . . . . . . 398
* 31.8 Which Automation Tool Should Be Used? . . . . . . . . . . . . . . . . . . . . . 399
* 31.8.1 Too Much Corporate Fluff . . . . . . . . . . . . . . . . . . . . . . . . . 399
* 31.8.2 Do Your Own Research . . . . . . . . . . . . . . . . . . . . . . . . . . . 399
* 31.9 Current Infrastructure Automation Tools . . . . . . . . . . . . . . . . . . . . . . 400
* 31.10 Other Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 402
* 31.11 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 403
* 32 Continuous Integration 405
* 32.1 Principles of Continuous Integration . . . . . . . . . . . . . . . . . . . . . . . . 406
* 32.1.1 Write Lots of Tests! . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 406
* 32.1.2 Keeping the Build Fast . . . . . . . . . . . . . . . . . . . . . . . . . . . 406
* 32.2 Tools for Continuously Integrating Your Project . . . . . . . . . . . . . . . . . . 407
* 32.2.1 Tox . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 407
* 32.2.2 Jenkins . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 408
* 32.3 Continuous Integration as a Service . . . . . . . . . . . . . . . . . . . . . . . . . 408
* 32.3.1 Code Coverage as a Service . . . . . . . . . . . . . . . . . . . . . . . . . 409
* 32.4 Additional Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 409
* 32.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 409
* 33 The Art of Debugging 411
* 33.1 Debugging in Development . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 411
* 33.1.1 Use django-debug-toolbar . . . . . . . . . . . . . . . . . . . . . . . . . 411
* 33.1.2 That Annoying CBV Error . . . . . . . . . . . . . . . . . . . . . . . . . 411
* 33.1.3 Master the Python Debugger . . . . . . . . . . . . . . . . . . . . . . . . 413
* 33.1.4 Remember the Essentials for Form File Uploads . . . . . . . . . . . . . . 413
* 33.1.5 Lean on the Text Editor or IDE . . . . . . . . . . . . . . . . . . . . . . 416
* 33.2 Debugging Production Systems . . . . . . . . . . . . . . . . . . . . . . . . . . . 416
* 33.2.1 Read the Logs the Easy Way . . . . . . . . . . . . . . . . . . . . . . . . 416
* 33.2.2 Mirroring Production . . . . . . . . . . . . . . . . . . . . . . . . . . . . 417
* 33.2.3 UserBasedExceptionMiddleware . . . . . . . . . . . . . . . . . . . . . . 417
* 33.2.4 That Troublesome settings.ALLOWED HOSTS Error . . . . . . . . . . . 418
* 33.3 Feature Flags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 419
* 33.3.1 Feature Flag Packages . . . . . . . . . . . . . . . . . . . . . . . . . . . . 420
* 33.3.2 Unit Testing Code Affected by Feature Flags . . . . . . . . . . . . . . . 420
* 33.4 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 420
* 34 Where and How to Ask Django Questions 421
* 34.1 What to Do When You’re Stuck . . . . . . . . . . . . . . . . . . . . . . . . . . 421
* 34.2 How to Ask Great Django Questions in IRC . . . . . . . . . . . . . . . . . . . 421
* 34.3 Feed Your Brain . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 422
* 34.4 Insider Tip: Be Active in the Community . . . . . . . . . . . . . . . . . . . . . 422
* 34.4.1 9 Easy Ways to Participate . . . . . . . . . . . . . . . . . . . . . . . . . 423
* 34.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 424
* 35 Closing Thoughts 425
* Appendix A: Packages Mentioned In This Book 427
* Appendix B: Troubleshooting Installation 435
* Identifying the Issue . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 435
* Our Recommended Solutions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 436
* Check Your Virtualenv Installation . . . . . . . . . . . . . . . . . . . . . . . . . . 436
* Check If Your Virtualenv Has Django 1.8 Installed . . . . . . . . . . . . . . . . . 437
* Check For Other Problems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 437
* Appendix C: Additional Resources 439
* Beginner Python Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 439
* Beginner Django Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 439
* More Advanced Django Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 441
* Useful Python Material . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 442
* JavaScript Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 443
* Appendix D: Internationalization and Localization 445
* Start Early . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 445
* Wrap Content Strings with Translation Functions . . . . . . . . . . . . . . . . . . . . . 446
* Don’t Interpolate Words in Sentences . . . . . . . . . . . . . . . . . . . . . . . . . . . 447
* Browser Page Layout . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 450
* Appendix E: Settings Alternatives 453
* Twelve Factor-Style Settings . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 453
* Appendix F: Working with Python 3 455
* Most Critical Packages Work with Python 3 . . . . . . . . . . . . . . . . . . . . . . . . 455
* Use Python 3.3.3 or Later . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 457
* Working With Python 2 and 3 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 457
* Resources . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 458
* Appendix G: Security Settings Reference 459
* SESSION SERIALIZER . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 460
* Acknowledgments 461
* List of Figures 466
* List of Tables 469
* Index 471


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

