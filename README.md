# Pythonanywhere-Hosting-Steps

- Create a beginner account here: https://www.pythonanywhere.com/pricing/ 
- Go to Dashboard.
- Go to pythonanywhere Dashboard,there head over to New Console on bottom let.
- Click on `bash`.
- A console will open.
- Make sure you are in hope directory using pwd command `(/home/YOUR_USERNAME)`.
- Go into you project on Github and get the project url that you want to host.
- Clone git project in home directory `git clone PROJECT_URL`.
- Make Python venv using command `mkvirtualenv --python=/urs/bin/python3.10 VENV_NAME` for specific version in my case it is 3.10 python version.
- It will create and activate Venv in console, you can now simply install your project dependencies `pip install django`.
- Go to Dashboard and click on `Open Web tab` in Web apps column
- Create a new web app here click on `Add a new web app`
- You can upgrade domain name, in my case i have used free version.
- Then select your Web Framework, in my case i am doing it manually, click on `Manual configuration`.
- Select your python version, in my case it is python 3.10
- Click next (Manual configuration).
- Here you go Web app is setup correctly.
