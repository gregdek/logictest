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

Download NaanProphet/git-logic-init (see that repo for details)
`curl -s -L -OO \
https://github.com/NaanProphet/git-logic-init/releases/latest/download/init{.sh,.sh.sha256} \
&& shasum -a256 -c init.sh.sha256`

Run the init script against the local repo
`sh init.sh`
