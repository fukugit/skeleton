# skeleton
The Skeleton is an extremely simple theme for Hugo.  

![image](./images/screenshot.png)

## Demo
You can see the demo page [here](https://fukugit.github.io/skeleton/).  

## Introduction
This theme is composed of tiny resources. CSS line is just within 500 lines. The colors of definition in CSS are just four colors.  
That extreme simplicity allows you to customize by yourself, like changing colors and expanding some buttons, links, fonts, and tables in layout.  

Even though this theme is straightforward, it has essential features that you might want at least. You can find it below.  

### Features:
- Responsive design
- Main & secondary menus
- Widgetized sidebar

## Installation
### Preparation
Before starting, please be sure that you've already prepared the following.  
1. Installed Hugo.
1. Create a new website with the Hugo command, which is ```hugo new site XXXX```. 
1. It is necessary to turn the new site into a git project by executing ```git init``` command.  

After that, you are ready to install Skelton. Go ahead.

#### Note:
If you don't want to create a new site as in the above step 2, You have two ways of executing this theme. See the below.  

1. You can download the [hugoBasicExample](https://github.com/gohugoio/hugoBasicExample) to run Hugo with Skeleton.  
1. You can run this theme in [exampleSite](./exampleSite). 

### Install Skelton
```
mkdir themes ## If already existing, you can skip this command.
cd themes
git submodule add https://github.com/fukugit/skeleton.git
```

#### Note:
If you don't have a themes directory, you can create it manually as ```mkdir``` command.  

### Setting of config file
Next, open 'config. toml' in the base of the Hugo site and set like below.  
```
theme = "skeleton"
```

Installation got done!  
To run your Hugo with Skeleton, you can execute the following command.  
```
hugo server
```

## Update
If this project is updated while using it in your Hugo blog, you can run the below command to update the latest version.  
### Update Skeleton
```
git submodule update --recursive
```

## Uninstallation
If you want to uninstall Skeleton, you can remove it following the below commands.
### Uninstall Skeleton
```
## Move your current directory before executing the below commands.
git submodule deinit -f themes/skeleton
git rm -f themes/skeleton
rm -rf .git/modules/themes/skeleton
```

## GitHub Actions
The [demo page](https://fukugit.github.io/skeleton/) in this page got deployed using GitHub Actions. You can see the GitHub Actions setting file [here](./.github/workflows/github-pages.yml). The following is the setting of GitHub Actions and GitHub Pages on GitHub.  
1. Creat directory that is ```.github/workflows```. If already existing, skip it.  
1. Copy [github-pages.yml](./.github/workflows/github-pages.yml) into the ```.github/workflows``` directory.  
1. Set GitHub page like the below.  
![image](./images/GitHupPage.png)
1. To build the page with the above GitHub Actions, push something at the main branch.  
