# IIS Playground
## _Configure the windows server for web application._


This readme walkthrough the installation and configueration of IIS manager, deploy the web application on localhost in port 5100

#### What we going to do? 
 - Add IIS manager.
- Create application pool.
- Create web application.
- Copy web application file.
- Open the website in the browser.

## Add IIS manager
Go to search on your windows server and type ***Ture Windows features on or off***
- Choose the IIS manager and press add.
- Install and open the program.

## Create application pool
On the left side right-click on the Application pool and choose Add Application pool
- Insert the ***Name***
- Chosse ***No managed code***
- Choose ***Integrated***
- Make sure Start application ***marked***
- Press ***OK***

You now have Applicayion pool.

## Create web application
On the left side right-click on the ***Site*** and choose ***Add website...***

- Select the ***Application pool***
- Select ***Name***
- Add the ***physical path***
- Choose ***port*** *in our case 5100*
- Press ***OK***

## Copy web application file
Go to Visual Studio, right-click on the project name and select ***Publish*** 
In your local machine go to your source folder. usely at:
**source &#8594; project_name &#8594; bin &#8594; Release &#8594; net5.0 &#8594; publish**

- Copy all the files in the folder.
- Go to the  IIS manager &#8594; your-website and stop the server &#8594; on the rghit side there is a **STOP** button
- Rghit-click on the website name and choose explore
- Paste the file in the **inetpub &#8594; wwwroot &#8594; you-web-name** 
- If the file can't copies, paste it tempoary in folder at your desktop
- Go to the  IIS manager &#8594; your-website and start the server &#8594; on the rghit side there is a **START** button


## install dotnet
download the [dotnet](https://discord.com/channels/879626924975067176/879626926766059541/892565843748220938) software and install it on your server

## Open the website in the browser

Finely, go to your browser and type the address http://localhost:5100
