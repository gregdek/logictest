# logictest
Test a workflow for using GitHub to manage Logic X projects

## TODO

- [x] Find that script that dude wrote on the internet to do this (https://github.com/NaanProphet/git-logic-init)
- [x] Set up NaanProphet locally
- [ ] Commit a project that's just midi and update to see what happens
- [ ] Commit a project that has audio files and update to see what happens

## HOWTO

Clone the test repo:
`git clone git@github.com:gregdek/logictest.git`

Go into the test repo directory:
`cd logictest`

Download NaanProphet/git-logic-init (see that repo for details):
`curl -s -L -OO \
https://github.com/NaanProphet/git-logic-init/releases/latest/download/init{.sh,.sh.sha256} \
&& shasum -a256 -c init.sh.sha256`

Run the init script against the local repo:
`sh init.sh`

NOTE: installation also tests for presence of git lfs and other key
dependencies. 

## PROJECT01 DETAILS

Project01 is a test project with 4 tracks of sequencer only data. No audio tracks have been recorded for it. The initial save options:

* "Organize my project as a:
 * Folder
* "Copy the following files intp your project:" --> 
 * Audio files 
 * Sampler audio
 * Alchemy audio data
 * Ultrabeat audio data

Tag 01.001: first commit to Project01 with the basic 4 tracks of sequencer data

Tag 01.002: new 5th track added, "wurlitzer pattern 3"

Tag 01.003: just a simple close/reopen, then save with "no changes".

Tag 01.004: added a 6th track, this one a basic vocal speaking track

Tag 01.005: added a new track, "wurlitzer pattern 4"
