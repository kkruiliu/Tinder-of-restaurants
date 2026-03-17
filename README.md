# Tinder-of-restaurants
User Instruction for running 
Tinder of Restaurants

0. Before you run: (important) 
Alternative way to deploy: 
Instead of directly open the files we submitted, you can clone the whole project through our main repository:

https://github.com/kkruiliu/Tinder-of-restaurants

     b.SSL
There’s a high chance you might run into a SSL verification problem: (something like this) 

urllib.error.URLError: <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1028)>
IF you are using a  macOS (perfered), simply run the following command line in terminal to avoid such problem: 

/Applications/Python\ 3.13/Install\ Certificates.command

IF you are using Windows, please use: 

pip install --upgrade requests
python -m pip install --upgrade certifi

IF you are using any Linux OS, please do not use it. (never test it in any Linux environment) 




1. Required Libraries
requests
selenium
webdriver_manager
pandas
googlemaps
numpy
flask
matplotlib
random
kivy
os
If you're using an IDE like PyCharm, simply hover your cursor over the red wavy line under the code and click on "Install xxx." 
Alternatively, you can install these libraries using pip by running the following command:


pip install requests selenium webdriver_manager pandas googlemaps numpy flask matplotlib random kivy os



2. File Structure
Ensure the files are structured as follows:

3. API Key Configuration
All API keys (Google Maps, Zipcode) are already included in the scripts. 
However, the Zipcode API has a rate limit of 10 requests per hour and is only called when you select "Distance" on this page. If you exceed this limit, please select "Review" instead.



4. Running the Program
The program is best run in the following environments: Spyder, VS Code, or PyCharm.
Run Opening_Page.py to start Tinder of Restaurants! 

UNFORTUNATELY, I couldn’t find any way as CMake to build Python code so that you don’t have to look for which file to run with, but you can use the following command line to run: 


   pip install pyinstaller
   pyinstaller --onefile Opening_Page.py


5. Resolution
Since this app is made for mobile devices, the different size of a monitor of testers might have a different experience, for example the size of (500, 1200) is good for Mac screens, however it looks a bit off on a 2k desktop monitor. So please feel free to adjust the window size: 
In Opening_Page.py, search for (ctrl +F ): 

       Window.size = (500 ,1280)

