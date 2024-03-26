# Pythonanywhere-Hosting-Steps

- Create a beginner account here: https://www.pythonanywhere.com/pricing/ ![Dashboard](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/1.JPG) 
- Go to pythonanywhere Dashboard, there head over to New Console on the bottom left.
- Click on `bash`.  ![Bash](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/2.JPG) 
- A console will open. ![Console](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/3.JPG) 
- Make sure you are in the home directory `(/home/YOUR_USERNAME)` using `pwd` command in the console.
- Go into your project on Github and get the project url that you want to host.
- Clone git project in home directory `git clone PROJECT_URL`.
- Make Python venv using command `mkvirtualenv --python=/urs/bin/python3.10 VENV_NAME` for a specific version in my case it is 3.10 python version.
- It will create and activate Venv in console, you can now simply install your project dependencies `pip install Django`.
- Go to Dashboard and click on `Open Web tab` in the Web apps column. ![Web apps](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/4.JPG) 
- Create a new web app here click on `Add a new web app`. ![Create Web app](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/5.JPG) 
- You can upgrade the domain name, in my case, I have used the free version.
- Then select your Web Framework, in my case, I am doing it manually, and click on `Manual configuration`.
- Select your Python version, in my case it is Python 3.10.
- Click next (Manual configuration).
- Here you go Web app is setup correctly.
- Head over to that web app, scroll down, and enter the virtual environment name, in my case it is venv. ![Venv](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/6.JPG)
- Now enter path for Static files in Static fies section. ![Static Files](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/7.JPG)
- Now alter wsgi configuration file for that click on `WSGI configuration file` in the code section. ![WSGI config](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/8.JPG) 
- Uncomment line# 74-89 and except these lines delete everything else. 
- Set the project path, get it from the console using `pwd` command, and add YOUR_PROJECT_NAME.settings. ![Path](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/9.JPG)
- Add the domain in `ALLOWED_HOSTs` in `settings.py`. ![Host](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/10.JPG)
- Reload the app and there you go, your project is hosted successfully! ![Reload](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/11.JPG)
  ![Reload](https://github.com/noorulnisa2k/Pythonanywhere-Hosting-Steps/blob/main/12.JPG)
- Reference link for hosting https://www.youtube.com/watch?v=xtnUwvjOThg
- Reference link for static files https://www.youtube.com/watch?v=uCKZr9wddNw
