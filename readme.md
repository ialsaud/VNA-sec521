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
* after the machine has appeared running (pass: user)


* open a terminal and git clone this reposotory. 
* open folder explorer to `/home/user/Experiments`
* if there is a file called `version-number-attack` remove it (or back it up)
* copy from this repo `version-number-attack-XXX-mal-motes` into the `/home/user/Experiments` 
* rename the newly copied folder into `version-number-attack`

## Running the simulation
* open the rpl attack framework program, from the icon in desktop. Icon with name `RPL Attacks Framework`


* type `cooja version-number-attack` 
* now the cooja simulation with our set up will be spun up. 

## Important directories and config files.
* File for the experiement configuration:
  * `/home/user/Experiments/<attack-name>.json`
  * (guidance)[https://rpl-attacks.readthedocs.io/en/latest/campaigns/].
  * in this file you will be able to adjust the type of network topology, number of motes, ..etc.
* Folder where rpl attack framework saves experiment, simulation config, and simulation data:
  * `/home/user/Experiments/<attack-name>/`
  * in this folder you will find simulation data such as relationships and pcaps.
* File where building blocks (for malicious motes) are stored and created:
  * `home/user/templates/building-blocks.json`
  * (guidance)[https://rpl-attacks.readthedocs.io/en/latest/building-blocks/]
  * in this file you add new types of attack motes to be simulated. 
