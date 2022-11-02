# Docs for using Beaker 

## Installation 
### Requirements 
- Rust: https://www.rust-lang.org/tools/install
- Cargo: https://doc.rust-lang.org/cargo/getting-started/installation.html

You need to install Rust and Cargo first in order to continue the following steps 

### Install Local Osmosis 
**_NOTE:_** Referrence: https://docs.osmosis.zone/cosmwasm/local/localosmosis

You can either implement the Osmosis tool kit using the automatic setup provided by Osmosis:
```
bash <(curl -sL https://get.osmosis.zone/run)
``` 

Or you can download the LocalOsmosis from the Github repo and speed up Blocktime for faster testing experience
```
https://github.com/osmosis-labs/LocalOsmosis
``` 

**_NOTE:_** I suggest you should try using automatic setup providede by Osmosis first. By doing this, we have full tool kits provided by Osmosis, including Local Osmosis, osmosisd CLI. And it even downloads all the prerequisites for you i suppposed 


## Beaker

**_NOTE:_** Referrence:  https://docs.osmosis.zone/beaker/#execute-contract-messages

### Install 
To install beaker
```
$cargo install -f beaker # `-f` flag for up-to-date version
```

### Setup 
- Create new workspace: 
```
beaker new counter-dapp
``` 
A command line prompt will show up and ask you to choose between mininal or counter-example template. If you choose the minimal, an empty work space structure will be provided and you need to add the contract in the following steps. If you choose the couter-example, an workspace with a counter-example contract + frontend will be generated. You can directly test beaker with this prebuild smartcontract

Workspace structure will look like this
```
.
├── frontend
├── contracts
├── Cargo.toml
├── Beaker.toml
├── .gitignore
└── .beaker
```

The contracts will be located in the contracts folder. If you choose the 