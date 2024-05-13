# make sure node pakage is installed 
npm install
npm start
# to package the application 

npm pack     # you can change the name and the version of the artefact in package.json file

# to run application from the package ( *.tgz)
wget <Url of package> <br>
tar -xzf your-package-name.tgz <br>
cd your-package-name <br>
npm install <br>
npm start <br>



