I've been running this script on Heroku for 10 days without any app/account suspensions. Also, no one has told me about their app/account getting suspended from using this version of the script. 

**Note: This method requires a GitHub account**

1. Fork this repo (or clone it and re-push to a GitHub account under your name): 

https://github.com/nathan78906/steam-salien-cheat (**It's best to make the repo private as well**)

2. Add the 2 following files to the repo
- File Name "Procfile"
    - Contents: `worker: python saliens.py`
- File Name "requirements.txt"
    - Contents: `requests`
3. Input the token/steamid into `saliens.py` (Instructions on Repo's README)
4. Create a Heroku account and a new app
5. Go to the deploy tab (on the new app)
6. In `Deployment Method` make sure to link your GitHub account with your Heroku account

![](https://i.imgur.com/a2o02W8.png)

7. Connect to the repository holding all of the files (including the files created in step 2)

![](https://i.imgur.com/AbUnIlO.png)

8. Deploy the app to Heroku 

![](https://i.imgur.com/XwHkm54.png)

9. Go to the overview tab
10. Turn on the worker under `Dyno Formation` (Click `Configure Dynos`, then click the pen on the right hand side)

![](https://i.imgur.com/8VNuWnZ.png)

11. To view logs click `More` then `View logs`

![](https://i.imgur.com/FzzEl2e.png)

**If you get stuck anywhere, googling (and using the terminology I used here) should help a lot.**