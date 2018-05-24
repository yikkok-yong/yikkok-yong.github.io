---
layout: post
title:  "Ethereum Smart Contract - Part 2"
date:   2018-05-27 10:00:00 +0800
categories: ethereum smart-contract
author: John Yong
excerpt_separator: <!--Read More...-->
---

Write your first smart contract
<!--Read More...-->

### Requirements
<hr>
* NodeJS 5.0 or above installed - ([More Details](https://nodejs.org/en/download/))

#### 1. Installation
* Installing [**truffle**](http://truffleframework.com/)
> ```npm -g install truffle```


* Installing [**ganache**](http://truffleframework.com/ganache) (GUI)
> ```npm -g install ganache-cli```

#### 2. Create an empty project and initialize
* Create an empty directory, eg.
> ```mkdir SampleICO``` 
>> ```cd SampleICO```

* Initialize the directory
> ```truffle init```

* Generate packages.json
> ```npm init --yes```

#### 3. Installed packages for development
* OpenZeppelin, an open source smart contract library
> ```npm install openzeppelin-solidity --save```

* Installing packages for testing purpose
> ```npm install babel-polyfill babel-register --save-dev```
>> ```npm install babel-preset-env babel-preset-stage-2 babel-preset-stage-3 --save-dev```
>>> ```npm install chai chai-bignumber chais-as-promised```

##### 4. Linked Resources
* [Ethereum Smart Contract - Part 1]({% post_url 2018-03-11-smart-contract-part-1 %})