# Welcome to the first exercise
As you can see, there's a lot here in this project. For reference, this is
a repository that can launch a website, using your computer as a server. It
isn't public nor deployment-ready, but it gives you a look into what website
technologies can look like. The README.md instructions are a good overview
for the project, but we're only dealing with a small portion of the repository,
adding a few images, so here are instructions specific on what you need to do.

We're going to step through a few steps that will launch our website.

# Launching our website
1. Make sure you can access python and pip
```
python --version
python -m pip --version
```
Python is your Python interpreter; you should have this installed. Pip is
Python's module installer, and can pull from Python repositories to expand
its library. We'll need a few dependencies to launch this website.

2. Install virtualenv
```
python -m pip install virtualenv
```
This repository has a few dependencies that could interfere with our version of
Python. Rather than playing with multiple versions, we will make use of virtual
environments, which create an isolated area where you can safely work.

3. Create a virtual environment
```
python -m virtualenv env
```
This command uses Python to create a virtual environment called "env."

4. Run the virtual environment
```
source env/bin/activate
```
OR
```
source env/Scripts/activate
```
Inside your env folder, there's a folder with scripts/binaries, and there's
one called "activate." This starts the virtual environment and should show
a `(env)` at the end of the command line. Whenever you want to run the site,
you'll need to to turn on the virtual environment.

5. Get the dependencies
```
pip install -r requirements.txt
```
With our environment open, we can now install our dependencies using pip. As
long as your virtual environment is running, nothing should go wrong.

6. Launch the website
```
python app.py
```
After this command, open your browser and go to localhost:5000 to see your
website template! (Just enter "localhost:5000" in your url address bar.)

7. Turning off the website (Crtl+C)
```
deactivate
```
Use Crtl+C to kill the process, and enter deactivate to turn off your virtual
environment. Congratulations, you created your first web application. Whenever
you want to run it again, remember to activate your virtual environment and
run app.py.

# The Exercise:
You'll notice that main page is pretty barren, so let's add some photos.

Go to static/img, and replace the images with whatever you want (keep it
appropriate). Remember to name them correctly, otherwise you'll need to edit
the html (located in static/templates/pages/placeholder.home.html). When you're
done, commit your changes, run the website, and submit a photo of your website to
the discussion. You can keep editing the website if you're inclined.