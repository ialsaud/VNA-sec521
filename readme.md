# SEC521: Network Security
# Version Number Attack reproduction steps

  In this readme we will walk you through the steps of recreating report specific simulation. Most of the steps were 'implied' in this [link](https://rpl-attacks.readthedocs.io/en/latest/install/).


## Dependencies
* install virutalbox via [link](https://www.virtualbox.org/wiki/Downloads)
* install vagrant via [link](https://www.vagrantup.com/downloads)
* create a working directory, i.e. `/home/user/rpl-attack-vm/` and `cd` to it.
* run the following vagrant up command on cmd or terminal:
  * `vagrant init dhondta/rpl-attacks --box-version 1.0.0


## Setting up the required documents
* from the same working directory run `vagrant up`
  * this will download and run the rpl attack framework virtual machine. 
  * note: you might face some USB error, open virtualbox and disable USB adapter on the vm. 
* after the machine has appeared running, such as follow: (pass: user)


* open a terminal and git clone this reposotory. 
* open folder explorer to `/home/user/Experiments`
* if there is a file called `version-number-attack` remove it (or back it up)
* copy from this repo `version-number-attack-XXX-mal-motes` into the `/home/user/Experiments` 
* rename the newly copied folder into `version-number-attack`

## Running the simulation
* open the rpl attack framework program, from the icon in desktop. Icon such as follow:


* type `cooja version-number-attack` 
* now the cooja simulation with our set up will be spun up. 

