I've had a problem that the chromedriver doesnt execute a commands of capybara.

So, bellow the link that I check and function:

https://gist.github.com/ziadoz/3e8ab7e944d02fe872c3454d17af31a5


capybara_cucumber

My first project

how I solved my problem with chromedriver on ubuntu 16.04 https://christopher.su/2015/selenium-chromedriver-ubuntu/

Install ChromeDriver:1

sudo apt-get install unzip

wget -N http://chromedriver.storage.googleapis.com/2.26/chromedriver_linux64.zip unzip chromedriver_linux64.zip chmod +x chromedriver

sudo mv -f chromedriver /usr/local/share/chromedriver sudo ln -s /usr/local/share/chromedriver /usr/local/bin/chromedriver sudo ln -s /usr/local/share/chromedriver /usr/bin/chromedriver

######################################################################################################################

problem to install gem selenium-webdriver

solved with commands

sudo apt-get install libffi-dev

sudo gem install ffi

######################################################################################################################

commands to generations a execution report are:

cucumber --format html -o report.html or can be too cucumber --format html out=> report.html

#will generate a archive report.html on mainlyng folder of the project

Case you wanna to generate a report in other folder so you may write that

cucumber --format html -o folder/report.html #Ubuntu

cucumber --format html --out folder/report.html #windows

######################################################################################################################

I had to generate a nem archive .json that it´s necessary to interpretation of Jenkins for cucumber reports.

cucumber -f pretty -f json -o cucumber.json

######################################################################################################################
Same configurations for jenkins with chromedriver and firefox geckodriver

https://stgconsulting.com/running-automated-selenium-tests-from-jenkins-on-linux/

#######################################################################################################################
How I solved my problem with instalation Jenkins in Ubuntu 18.04
https://stackoverflow.com/questions/49937743/install-jenkins-in-ubuntu-18-04-lts-failed-failed-to-start-lsb-start-jenkins-a

########################################################################################################################
site prism page objetcs
http://shipit.resultadosdigitais.com.br/blog/como-estruturar-page-objects-utilizando-siteprism/

########################################################################################################################
https://tableless.com.br/tudo-que-voce-queria-saber-sobre-git-e-github-mas-tinha-vergonha-de-perguntar/
