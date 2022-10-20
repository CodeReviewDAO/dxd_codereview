Grant Proposal | [341 - Casper Ruby SDK](https://portal.devxdao.com/public-proposals/341)
------------ | -------------
Milestone | 3
Milestone Title | Final
OP | sgulmez
Reviewer | Chad (elmabahma@gmail.com)

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- Ruby version of CLType primitives
- Ruby version for Casper domain-specific objects
- Serialization of Casper domain-specific objects
- ED25519/SECP256K1 key pairs  Wrappers
- PutDeploy RPC call implemented
- Refactoring Ruby SDK calls to return Casper domain-specific objects

**Acceptance criteria:**

- Ruby version of CLType primitives
- Ruby version for Casper domain-specific objects
- Serialization of Casper domain-specific objects
- ED25519/SECP256K1 key pairs  Wrappers implemented
- PutDeploy call implemented and tested
- SDK calls will return Casper domain-specific objects
- SDK published as a Ruby Gem


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/saitgulmez/casper-ruby-sdk | fa31569

# Install & Usage Testing Procedure and Findings

Following the instructions in the README file of https://github.com/saitgulmez/casper-ruby-sdk, the reviewer was
able to  : 

* Install Ruby on Rails on an Ubuntu20.04 cloud server

* Install all  Ruby dependencies (gems) required by the  Ruby SDK

```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ bundle install
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
Using concurrent-ruby 1.1.10
Using unf_ext 0.0.8.2
Using netrc 0.11.0
Using blake2b 0.10.0
Using blankslate 3.1.3
Using bundler 2.3.24
Using casper_network 1.1.2 from source at `.`
Using chilkat 9.5.0.91 (x86_64-linux)
Using diff-lcs 1.5.0
Using i18n 1.12.0
Using unf 0.1.4
Using ipaddress 0.8.3
Using domain_name 0.5.20190701
Using multi_json 1.15.0
Using http-cookie 1.0.5
Using mime-types-data 3.2022.0105
Using rspec-support 3.11.1
Using mime-types 3.4.1
Using timeout 0.2.0
Using resolv 0.2.1
Using rspec-expectations 3.11.1
Using rspec-mocks 3.11.1
Using blake2 0.5.0
Using tzinfo 2.0.5
Using ed25519 1.3.0
Using http-accept 1.7.0
Using rack 3.0.0
Using rspec-core 3.11.0
Using rest-client 2.1.0
Using stringio 3.0.2
Using minitest 5.16.3
Using jimson 0.13.0
Using psych 4.0.6
Using activesupport 7.0.4
Using rspec 3.11.0
Using rdoc 6.4.0
Bundle complete! 13 Gemfile dependencies, 36 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
```

* Install and build casper_network1.1.2 gem from repository

```bash

abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ gem build casper_network.gemspec
  Successfully built RubyGem
  Name: casper_network
  Version: 1.1.2
  File: casper_network-1.1.2.gem
```

```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ gem install casper_network-1.1.2.gem
Successfully installed casper_network-1.1.2
1 gem installed
```

```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ gem build casper_network.gemspec
  Successfully built RubyGem
  Name: casper_network
  Version: 1.1.2
  File: casper_network-1.1.2.gem
````


* Install testing tools 

```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ gem install rspec
Successfully installed rspec-3.11.0
1 gem installed

```

## Overall Impression of usage testing
The documentation provides clear and sufficient instructions to build and install the Ruby sdk bundle.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS 
Project functionality meets/exceeds acceptance criteria and operates without error | PASS


# Code 

The reviewer was able to verify that all the CLType primitives are implemented in the project. The project also contains most 
of the [Casper domain objects and entities (Deploy, Block, Era, Validator etc...)](https://docs.casperlabs.io/dapp-dev-guide/sdkspec/types_chain/) implemented in Ruby. 
The reviewer  was also able to verify the presence of byte [Serialization](https://docs.casperlabs.io/design/serialization-standard/) functions for all [CLType](https://docs.casperlabs.io/dapp-dev-guide/sdkspec/types_cl/) primitives and Casper domain 
objects (related to sending a deploy to the network: Deploy, Block, DeployExecutable etc...).

# Unit / Automated Testing
The project has very good test coverage with more than 238 unit tests covering positive tests and exceptional cases.
The OP has since the last milestone added logging functionality to unit tests. 
We can understand the course of these tests when they are launched.
The reviewer was also able to check the presence of many negative path tests across the project.

The tests run successfully, without errors and produce the following output:

[Ruby SDK- M3-Tests](tests.md)

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS 

# Documentation

### Code Documentation
A commendable effort has been made to document the project code following the remarks made on this point. In the review of milestone 2. 
The code is now overall well documented now and almost all critical functions designed for milestone 3 have acceptable code-level documentation.

Requirement | Finding
------------ | -------------
Code Documented | PASS 


### Project Documentation

The reviewer has observed that the project has a very acceptable level of documentation. The documentation is sufficient to understand the SDK project.
There are also code examples that simplify the understanding of critical functions of the SDK.

Requirement | Finding
------------ | -------------
Usage Documented | PASS 


## Overall Conclusion on Documentation

In the reviewer's opinion, the project and usage documentation are sufficient.

# Open Source Practices

## Licenses

The Project is released under the Apache-2.0 License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and Issues are enabled on the repository. The project contains a CONTRIBUTING and a SECURITY policy. 

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS 

# Coding Standards

Source code is well-written. General best coding practices are used throughout.
Some leftover comments can be cleaned up as a suggestion.

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub and all 238 unit tests pass.

# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria. 
The SDK is well-documented and has a very good level of tests. 
In the reviewer's opinion, this submission should pass.

# Recommendation

Recommendation | PASS 
------------ | -------------
