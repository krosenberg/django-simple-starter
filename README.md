Django Simple Starter Project
===
This is a starting template for those who wish to start a Django project very quickly without (barely) any configuration. You may optionally use virtualenv to create a virtual environment, and you can also initialize a development database (but you don't have to if you don't want to!).

The project contains a single app called **main** and there is a static files directory all ready do go inside the **main** directory.

---

Quick Instructions
---

**To get started right away (assuming you have Python 2.6+ and Django 1.6 installed), just run the command `python manage.py runserver`, and you should be up and running at [http://localhost:8000](http://localhost:8000)!**

---

Detailed Instructions
---

###1. Create a virtual environment (optional)
***(This step is optional, but make sure you have Python 2.6+ and Django 1.6 installed on your system if you're not going to use a virtual environment);***

1. Make sure you have virtualenv installed.
	- You can check if virtualenv is installed by running the command `virtualenv --version` in a terminal window.
	- If you need to install virtual env, run the command `pip install virtualenv`.
2. `cd` into this directory (django-simple-starter).
3. Run `virtualenv dss-env`.
	- You change dss-env to whatever you want to name your virtual environment.
	- To use python3 with your virtual environment, instead run `virtualenv -p python3 dss-env`
- Activate the virtual environment with the command `source dss-env/bin/activate`.
- Once the virtual environment is activated, install Django with the command `pip install -r requirements.txt`.
- If you need to deactivate the virtual environment, run `deactivate`.

###2. Initialize a database (optional)
***(This step is not required if you don't want use authorization, models, or any other database-related functions.)***

1. In the **django-simple-starter** directory (the one with manage.py), run `python manage.py syncdb`
2. When it offers to create a superuser, choose `Y` and enter a username, email address (optional), and password.


###3. Start the server
1. In the **django-simple-starter** directory, run `python manage.py` runserver
2. Once running you'll be able to visit [http://localhost:8000](http://localhost:8000) in your browser. You should see a green "Hello, world" message if everything is working correctly.


---
####*Hey Bower users!*
There is a **.bowercc** config that will put any Bower-installed libs into the **static/libs** directory if you run a bower install command from the **static**.

---

For more information about Django 1.6, check out [https://docs.djangoproject.com/en/1.6/intro/tutorial01/#creating-models](https://docs.djangoproject.com/en/1.6/intro/tutorial01/#creating-models).