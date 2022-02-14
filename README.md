# okta-customized-login-assets

#### Serving assets locally
- Create a folder with the file you want to serve publicly
- Install ngrok https://ngrok.com/
```
$ unzip ngrok-stable-darwin-amd64.zip
$ sudo mv ngrok /usr/local/bin
$ exit
$ ngrok authtoken <generated-token> # sourced from https://dashboard.ngrok.com/
```
- cd to your new folder, run python3 -m http.server to serve it locally
```
$ cd ~/dev/okta-customized-login-assets
$ python3 -m http.server # let this run in the background
```
- run ngrok http 8000 (change the port as necessary to match the output of python)
- See thing hosted on the internet e.g http://a3a3-24-244-29-187.ngrok.io/public/assets/css/styles.css
