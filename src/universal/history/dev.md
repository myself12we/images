# [universal](https://github.com/devcontainers/images/tree/main/src/universal)
This document describes the base contents of the Universal image. Note that this image also includes detection logic to dynamically install additional language / runtime versions based on your repository's contents. Dynamically installed content can be found in sub-folders under `/opt`.

**Image version:** dev

**Source release/branch:** [main](https://github.com/devcontainers/images/tree/main/src/universal)

**Digest:** sha256:150fde58684752c6d538941a71fc5e182648b9bd475898bc892e9e2ca4694acf

**Tags:**
```
mcr.microsoft.com/devcontainers/universal:dev-focal
mcr.microsoft.com/devcontainers/universal:dev-linux
mcr.microsoft.com/devcontainers/universal:dev
```
> *To keep up to date, we recommend using partial version numbers. Use the major version number to get all non-breaking changes (e.g. `0-`) or major and minor to only get fixes (e.g. `0.200-`).*

**Linux distribution:** Ubuntu 20.04.6 LTS (debian-like distro)

**Architectures:** linux/amd64

**Available (non-root) user:** codespace

### Contents
**Languages and runtimes**

| Language / runtime | Version | Path |
|--------------------|---------|------|
| [Node.js](https://nodejs.org/en/) | 18.16.0<br />19.9.0 | /usr/local/share/nvm/versions/node/&lt;version&gt; |
| [Python](https://www.python.org/) | 3.10.4<br />3.9.16 | /usr/local/python/&lt;version&gt; |
| [Java](https://adoptopenjdk.net/) | 11.0.18<br />17.0.6 | /usr/local/sdkman/candidates/java/&lt;version&gt; |
| [.NET](https://dotnet.microsoft.com/) | 6<br />0<br />4<br />0<br />8<br />7<br />0<br />2<br />0<br />3 | /usr/local/dotnet |
| [Ruby](https://www.ruby-lang.org/en/) | 3.0.6<br />3.1.4 | /usr/local/rvm/rubies/&lt;version&gt; |
| [PHP](https://xdebug.org/) | 8.1.14<br />8.2.1 | /usr/local/php/&lt;version&gt; |
| GCC | 9.4.0-1ubuntu1~20.04.1 | 
| Clang | 10.0.0-4ubuntu1 | 
| [Go](https://golang.org/dl) | 1.20.3 | /usr/local/go |
| [Jekyll](https://jekyllrb.com/) | 4.3.2 | 
| [Jupyter Lab](https://jupyter.org/) | 3.6.3 | /home/codespace/.local/bin/jupyter-lab |

**Tools installed using git**

| Tool | Commit | Path |
|------|--------|------|
| [Oh My Zsh!](https://github.com/ohmyzsh/ohmyzsh) | 91c7ed45a312a71b7d3b856228047ddcd51d4651 | /home/codespace/.oh-my-zsh |
| [nvm](https://github.com/nvm-sh/nvm.git) | 0ccd099bff8e384043883c4ae01b589794b13d72 | /usr/local/share/nvm |
| [nvs](https://github.com/jasongin/nvs) | 6c5a5983e2bccae5ac2b217b69210ecf3cd560f1 | /usr/local/nvs |
| [rbenv](https://github.com/rbenv/rbenv.git) | a632465cf4007d0a5b419ed5c5a7bd87349d7b14 | /usr/local/share/rbenv |
| [ruby-build](https://github.com/rbenv/ruby-build.git) | 48e927dad83b8b41e32bb718edc82a4a7081a903 | /usr/local/share/ruby-build |

**Pip / pipx installed tools and packages**

| Tool / package | Version |
|----------------|---------|
| numpy | 1.24.2 |
| pandas | 2.0.0 |
| scipy | 1.10.1 |
| matplotlib | 3.7.1 |
| seaborn | 0.12.2 |
| scikit-learn | 1.2.2 |
| torch | 2.0.0 |
| requests | 2.28.2 |
| plotly | 5.14.1 |
| jupyterlab-git | 0.41.0 |
| certifi | 2022.12.7 |
| setuptools | 67.7.0 |
| wheel | 0.40.0 |
| pylint | 2.17.2 |
| flake8 | 6.0.0 |
| autopep8 | 2.0.2 |
| black | 23.3.0 |
| yapf | 0.33.0 |
| mypy | 1.2.0 |
| pydocstyle | 6.3.0 |
| pycodestyle | 2.10.0 |
| bandit | 1.7.5 |
| virtualenv | 20.22.0 |
| pipx | 1.2.0 |

**Go tools and modules**

| Tool / module | Version |
|---------------|---------|
| golang.org/x/tools/gopls | 0.11.0 |
| honnef.co/go/tools | 0.3.3 |
| golang.org/x/lint | 0.0.0-20210508222113-6edffad5e616 |
| github.com/mgechev/revive | 1.3.1 |
| github.com/uudashr/gopkgs | 2.0.1+incompatible |
| github.com/ramya-rao-a/go-outline | 0.0.0-20210608161538-9736a4bde949 |
| github.com/go-delve/delve | 1.20.2 |
| github.com/golangci/golangci-lint | latest |

**Ruby gems and tools**

| Tool / gem | Version |
|------------|---------|
| rake | 13.0.6 |
| jekyll | 4.3.2 |

**Other tools and utilities**

| Tool | Version | Path |
|------|---------|------|
| [git](https://github.com/git/git) | 2.40.0 | 
| [Xdebug](https://xdebug.org/) | 3.2.1 | /usr/local/php/current |
| [Composer](https://getcomposer.org/) | 2.5.5 | /usr/local/php/current/bin |
| [kubectl](https://github.com/kubernetes/kubectl) | v1.27.1 | /usr/local/bin |
| [Helm](https://github.com/helm/helm) | 3.11.3 | /usr/local/bin |
| [Docker Compose](https://github.com/docker/compose) | 1.29.2 | /usr/local/bin |
| [rvm](https://github.com/rvm/rvm) | 1.29.12 | /usr/local/rvm |
| [GitHub CLI](https://github.com/cli/cli) | 2.27.0 | 
| [yarn](https://yarnpkg.com/) | 1.22.19 | /usr/bin |
| [Maven](https://maven.apache.org/) | 3.9.1 | /usr/local/sdkman/candidates/maven/current/bin |
| [Gradle](https://gradle.org/) | 8.1 | /usr/local/sdkman/candidates/gradle/current/bin |
| Docker (Moby) CLI &amp; Engine | 20.10.24+azure | 
| [conda](https://github.com/conda/conda) | 23.1.0 | /opt/conda/bin |

**Additional linux tools and packages**

| Tool / library | Version |
|----------------|---------|
| apt-transport-https | 2.0.9 |
| apt-utils | 2.0.9 |
| build-essential | 12.8ubuntu1.1 |
| ca-certificates | 20211016ubuntu0.20.04.1 |
| clang | 1:10.0-50~exp1 |
| cmake | 3.16.3-1ubuntu1.20.04.1 |
| cppcheck | 1.90-4build1 |
| curl | 7.68.0-1ubuntu2.18 |
| dialog | 1.3-20190808-1 |
| g++ | 4:9.3.0-1ubuntu2 |
| gcc | 4:9.3.0-1ubuntu2 |
| gdb | 9.2-0ubuntu1~20.04.1 |
| git | 1:2.25.1-1ubuntu3.10 |
| git-lfs (Git Large File Support) | 3.3.0 |
| gnupg2 | 2.2.19-3ubuntu2.2 |
| htop | 2.2.0-2build1 |
| iproute2 | 5.5.0-1ubuntu1 |
| iptables | 1.8.4-3ubuntu2 |
| jq | 1.6-1ubuntu0.20.04.1 |
| less | 551-1ubuntu0.1 |
| libatk-bridge2.0-0 | 2.34.2-0ubuntu2~20.04.1 |
| libatk1.0-0 | 2.35.1-1ubuntu2 |
| libc6 | 2.31-0ubuntu9.9 |
| libc6-dev | 2.31-0ubuntu9.9 |
| libcups2 | 2.3.1-9ubuntu1.2 |
| libgbm1 | 21.2.6-0ubuntu0.1~20.04.2 |
| libgcc1 | 1:10.3.0-1ubuntu1~20.04 |
| libgssapi-krb5-2 | 1.17-6ubuntu4.3 |
| libgtk-3-0 | 3.24.20-0ubuntu1.1 |
| libicu66 | 66.1-2ubuntu2.1 |
| libkrb5-3 | 1.17-6ubuntu4.3 |
| liblttng-ust0 | 2.11.0-1 |
| libnspr4 | 2:4.25-1 |
| libnss3 | 2:3.49.1-1ubuntu1.9 |
| libpango-1.0-0 | 1.44.7-2ubuntu4 |
| libpangocairo-1.0-0 | 1.44.7-2ubuntu4 |
| libsecret-1-dev | 0.20.4-0ubuntu1 |
| libssl1.1 | 1.1.1f-1ubuntu2.17 |
| libstdc++6 | 10.3.0-1ubuntu1~20.04 |
| libx11-6 | 2:1.6.9-2ubuntu1.2 |
| libx11-xcb1 | 2:1.6.9-2ubuntu1.2 |
| libxcomposite1 | 1:0.4.5-1 |
| libxdamage1 | 1:1.1.5-2 |
| libxfixes3 | 1:5.0.3-2 |
| lldb | 1:10.0-50~exp1 |
| llvm | 1:10.0-50~exp1 |
| locales | 2.31-0ubuntu9.9 |
| lsb-release | 11.1.0ubuntu2 |
| lsof | 4.93.2+dfsg-1ubuntu0.20.04.1 |
| make | 4.2.1-1.2 |
| man-db | 2.9.1-1 |
| manpages | 5.05-1 |
| manpages-dev | 5.05-1 |
| moby-cli (Docker CLI) | 20.10.24+azure-ubuntu20.04u1 |
| moby-engine (Docker Engine) | 20.10.24+azure-ubuntu20.04u1 |
| nano | 4.8-1ubuntu1 |
| ncdu | 1.14.1-1 |
| net-tools | 1.60+git20180626.aebd88e-1ubuntu1 |
| openssh-client | 1:8.2p1-4ubuntu0.5 |
| openssh-server | 1:8.2p1-4ubuntu0.5 |
| pigz | 2.4-1 |
| pkg-config | 0.29.1-0ubuntu4 |
| procps | 2:3.3.16-1ubuntu2.3 |
| psmisc | 23.3-1 |
| python3-dev | 3.8.2-0ubuntu2 |
| python3-minimal | 3.8.2-0ubuntu2 |
| rsync | 3.1.3-8ubuntu0.5 |
| sed | 4.7-1 |
| software-properties-common | 0.99.9.11 |
| strace | 5.5-3ubuntu1 |
| sudo | 1.8.31-1ubuntu1.5 |
| tar | 1.30+dfsg-7ubuntu0.20.04.3 |
| unzip | 6.0-25ubuntu1.1 |
| valgrind | 1:3.15.0-1ubuntu9.1 |
| vim | 2:8.1.2269-1ubuntu5.14 |
| vim-doc | 2:8.1.2269-1ubuntu5.14 |
| vim-tiny | 2:8.1.2269-1ubuntu5.14 |
| wget | 1.20.3-1ubuntu2 |
| xtail | 2.1-6 |
| zip | 3.0-11build1 |
| zlib1g | 1:1.2.11.dfsg-2ubuntu1.5 |
| zsh | 5.8-3ubuntu1.1 |

