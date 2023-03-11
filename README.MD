# devcontainer-hugo-extend-0.88.1

This README was written by Chat GPT, a language model developed by OpenAI. It provides a concise and informative overview of the devcontainer-hugo-extend-0.88.1 repository, including details on its purpose, requirements, and usage. The repository provides a devcontainer for Visual Studio Code to use the Hugo static site generator, with the Hugo extension pre-installed for a quick setup of the development environment.

## Purpose

The purpose of this repository is to provide a devcontainer for using the Hugo static site generator in Visual Studio Code. Hugo is a popular open-source static site generator that allows users to create fast and flexible websites. The devcontainer comes with the Hugo extension pre-installed, allowing for a quick setup of the development environment.

## Requirements

To use the devcontainer, users will need the following:

- Docker
- Visual Studio Code
- Remote - Containers extension

## Usage

### To use the devcontainer, follow these steps:

1. Clone this repository.
```
git clone https://github.com/ykinfo/devcontainer-hugo-extend-0.88.1.git
```

2. Open the folder of this repository in Visual Studio Code.
3. Click on the "><" icon in the bottom left and open the container remotely.
4. The development environment for using Hugo is now ready.

### to start hugo
#### Setup

1. Create a new directory for your site. For example, run the following command:
```
mkdir myblog
```

2. Change to the new directory, and build the site by running the following command:
```
cd myblog
hugo
```

#### Create Site

1. To create a new Hugo site, run the following command: 
```
hugo new site [site-name]
```

2. To create a new page, navigate to the site's directory and run the following command: 
```
cd [site-name]
hugo new [section-name]/[post-name].md
```

For example: 
```
hugo new post/hello-world.md
```

#### Run Server

To run the Hugo development server, use the following command: 
```
hugo server -D
```

#### When Using Theme

1. To install a theme, navigate to the site's directory and create a "themes" directory: 
```
cd [site-name]
mkdir themes
```

2. Add the theme as a Git submodule: 
```
git submodule add https://github.com/chipzoller/hugo-clarity.git themes/hugo-clarity
```

3. Edit the `config.toml` file in the root directory of your site and modify the values as needed. For example:
```
baseURL = "http://localhost:1313"
languageCode = "ja-jp"
title = "My New Hugo Site"

theme = "hugo-clarity"
```

## License

This repository is licensed under the MIT license. For more information, see the LICENSE file.

## Contact

If you have any questions or feedback about the repository or this README, please feel free to reach out to the repository owner.
