# JUNHYUK CHOI's RESUME

## Install ruby

1. First, update the packages index and install the packages required for the ruby-build tool to build Ruby from source:

```shell
sudo apt-get remove ruby
sudo apt update
sudo apt install git curl libssl-dev libreadline-dev zlib1g-dev autoconf bison build-essential libyaml-dev libreadline-dev libncurses5-dev libffi-dev libgdbm-dev
```

2. Next, run the following curl command to install both rbenv and ruby-build:

```shell
curl -sL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-installer | bash - 3. Add \$HOME/.rbenv/bin to the system PATH.
```

If you are using Bash, run:

```shell
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "\$(rbenv init -)"' >> ~/.bashrc
source ~/.bashrc
```

If you are using Zsh run:

```shell
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "\$(rbenv init -)"' >> ~/.zshrc
source ~/.zshrc 4. Install the latest stable version of Ruby and set it as a default version with:
```

```shell
rbenv install 2.5.1
rbenv global 2.5.1
```

To list all available Ruby versions you can use: rbenv install -l

5. Verify that Ruby was properly installed by printing out the version number:

```shell
ruby -v

# ruby 2.5.1p57 (2018-03-29 revision 63029) [x86_64-linux]
```

## Running locally

1. cd [my-project]

2. bundle install

3. bundle exec jekyll serve --livereload

> option: --livereload
