# Weblogic Auto Deploy Script
========================================

This project shows how to using Weblogic's WLST tool and python script to deploy project to Weblogic Server.

### How to use the script
  1. Please check your weblogic is started yet. If the weblogic is not started. Please go to  `Oracle_Home\user_projects\domains\(your domain)\bin` and double click `startWeblogic.cmd` or `startWeblogic.sh` if you are using linux platform.
  2. Then, when the weblogic is start up completely. Please go to `Oracle_Home\wlserver\server\bin` and fire up the `setWLSEnv.cmd` or `setWLSEnv.sh` if your are using linux platform.
  3. Then, please set up the user and sever url and the project path to the `weblogic_deploy.py`.
  4. Finally please run ` java weblogic.WLST (your weblogic_deploy.py path) `.

### Set up weblogic_deploy.py

| Variable | Value |
| ------ | ------ |
| username | Weblogic Server's usename. |
| password | Weblogic Server's password. |
| adminUrl | Weblogic Server's url e.g.`t3://localhost:7001`. |
| deploymentName | The name of the war or ear or jar. |
| deploymentFile | The path of the war or ear or jar. |
| deploymentTarget | Name of the server that you want to deploy on it. ** If you want deploy to multiple severs, please use a comma to separate it. e.g. 'server01,server02' ** |