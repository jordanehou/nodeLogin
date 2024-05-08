# make sure node pakage is installed 
npm install
npm start
# to package the application 

npm pack     # you can change the name and the version of the artefact in package.json file

# to run application from the package ( *.tgz)
wget <Url of package>
tar -xzf your-package-name.tgz
cd your-package-name
npm install
npm start



