# In Project:
- Create, update, delete & manage user profiles_api
- Authenticate with username and password
- Manage user profile feed items
- creating a workding local development runserver
- using django models to create a database
- enable and use Django admin
- Use Django dev server to run & test code
- Deploy app on aws (not done, only scripts)

# Profiles Rest API
Profile Rest API training course <br />
ModeHeader chrome extension for HTTP Requests : https://bewisse.com/modheader/help/ <br />
From Tutorial : https://github.com/LondonAppDev <br />
License: https://choosealicense.com/licenses/mit/ <br />
gitignore: https://www.gitignore.io/api/django,vagrant <br />
c1-ami-image (for aws): https://gist.github.com/LondonAppDev/d195610d79c9cca1769b6b5fece09067 <br / >

# Initilize vagrant
vagrant init ubuntu/bionic64 <br />
vagrant up <br />

# Virtual Environment creation
python -m {ENV_NAME} {PATH_WHERE_TO_CREATE_VIRTUAL_ENV} <br />
python -m venv ~/evn/ <br />
source ~/env/bin/activate
deactivate

# Creating Django Project
django-admin.py startproject profiles_project . <br />
python manage.py startapp profiles_api <br />

# start Project
- vagrant up
- vagrant ssh
- go to vagrant directory : cd /vagrant/
- activate virtual environement : source ~/env/bin/deactivate
- make migration file : python manage.py makemigrations
- apply changes to database : python manage.py migrate
- python manage.py runserver 0.0.0.0:8000


# Run script on GIT directly from terminal
- goto file, click raw, copy url
- curl -sL https://raw.githubusercontent.com/vikrantchaudharyy/profile_rest_api/master/deploy/setup.sh | sudo bash -
