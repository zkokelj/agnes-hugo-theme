# Agnes
<p>
	<a href="https://app.netlify.com/sites/sponge-bob/deploys">
		<img alt="Netlify Status" src="https://api.netlify.com/api/v1/badges/934b7c29-32b9-4ed5-92e7-79cfba9a27b7/deploy-status">
	</a>
	<a href="https://github.com/dchucks/agnes-hugo-theme/raw/master/LICENSE">
		<img src="https://img.shields.io/badge/license-MIT-green">
	</a>
	<a href="https://app.fossa.com/projects/git%2Bgithub.com%2Fdchucks%2Fagnes-hugo-theme?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2Fdchucks%2Fagnes-hugo-theme.svg?type=shield"/></a>
</p>

Agnes is a Landing Page theme ported from the free HTML template created by [Cruip](https://onepagelove.com/go/cruip). The design is lovely and features an intro screenshot preview area, product/service feature list and ends with three-tier pricing table.

# Getting started
We are assuming that you have already installed Hugo on your computer (follow the Quick start guide](https://gohugo.io/getting-started/quick-start/) if not).

## Create your Hugo website
```
hugo new site my_website
cd my_website
```
Now, there are two ways to add the theme to your Hugo website. 

### Method 1: Without involving Git
* Download the Agnes theme as a Zip file from https://github.com/dchucks/agnes-hugo-theme/archive/refs/heads/main.zip
* Create a sub-folder "Agnes" under the "Themes" folder.
```
cd themes
mkdir Agnes
```
* Unzip the zip file and copy all the files and folders (from the folder where the README.md file resides) to the Agnes folder.
* Now test if the theme is working, as follows, and your site should be running at http://localhost:1313/
```
cd Agnes/exampleSite/*
hugo server --themesDir ../..
```

### Method 2: With Git
* Clone the theme repository
```
git clone https://github.com/dchucks/agnes-hugo-theme.git Agnes
```
* Copy the example site 
```
cp -r Agnes/* my_website/themes
```
* Navigate to your website, and initialize an empty Git repository in the directory.
```
cd my_website
git init
```
* Add Agnes theme as a submodule and update the site configuration file for the current theme.
```
git submodule add -f https://github.com/dchucks/agnes-hugo-theme.git ./themes/Agnes
echo "theme = 'Agnes'" >> hugo.toml
```
* Start the dev server, your site should be running at http://localhost:1313/
```
hugo server
```

## Example config.toml
An example site Config file can be found under the theme's `exampleSite` folder. Just update the content in the file relevent to your website and you should be done.

## Contributing
If you want to contribute to Agnes to add a feature or improve the code, please open an [issue](https://github.com/dchucks/agnes-hugo-theme/issues) or make a [pull request](https://github.com/dchucks/agnes-hugo-theme/pulls).

## :stars: Show your support
Please give a :star: if this project helped you!

[![buy me a coffee](.github/bmc-button.png)](https://ko-fi.com/debashish)

#### :scroll: License
MIT © [Debashish Chakrabarty](https://www.debashish.com)