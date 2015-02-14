# face-web dev environment

A provisioning script for setting up a new dev environment for the dollarshaveclub.com client ember application.

This provisioning script is meant to be `curl`'d into a fresh dev environment ( e.g. a [Nitrous NodeJS Box]() TODO Add URI /TODO )


# Setup Remote Server

* Log in to Nitrous and create a new NodeJS box.
* Open the box's terminal

```sh
export github_user=austin-dsc
export repo_name=face-web-dev-environment

bash -c "$(curl -fsSL https://raw.github.com/$github_user/$repo_name/master/setup)"
```

## What Does It Do?

* Installs `ember-cli` and other dev dependencies TODO enumerate /TODO
* Clones the `face-web` app
* Starts the `face-web` in dev mode and monitors changes

Note : While `face-web` is in dev mode it uses the [Mock API]() TODO Apiary API /TODO

# Install Nitrous Desktop

```sh
brew cask install nitrous-desktop
```

* Launch Nitrous Desktop
* TODO Setup Local Env /TODO