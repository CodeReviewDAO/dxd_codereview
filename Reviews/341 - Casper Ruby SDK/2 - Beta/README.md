Grant Proposal | [341 - Casper Ruby SDK](https://portal.devxdao.com/public-proposals/341)
------------ | -------------
Milestone | 2
Milestone Title | BETA
OP | sgulmez
Reviewer | M Chad ABAHMAN

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

- The following RPC methods will be fully implemented in the Ruby SDK:
  * info_get_deploy
  * info_get_status
  * chain_get_block_transfers
  * chain_get_block
  * chain_get_eraInfo_by_SwitchBlock
  * state_get_item
  * state_get_dictionary_item
  * state_get_balance
  * state_get_AuctionInfo

These methods will return JSON arrays.

- Unit tests will be implemented.
- The SDK will be fully documented

**Acceptance criteria:**

- Following methods of the SDK are fully functional and returning data when called:
  * info_get_deploy
  * info_get_status
  * chain_get_block_transfers
  * chain_get_block
  * chain_get_eraInfo_by_SwitchBlock
  * state_get_item
  * state_get_dictionary_item
  * state_get_balance
  * state_get_AuctionInfo

- All unit tests are available and passing.
- Documentation are available for all critical classes and methods.


## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/saitgulmez/casper-ruby-sdk/tree/milestone-2 | e950bcb

# Install & Usage Testing Procedure and Findings

Following the instructions in the README of https://github.com/saitgulmez/casper-ruby-sdk/tree/milestone-2, the reviewer was
able to  : 

* Install Ruby on Rails on a Ubuntu 20.04 cloud server (https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-ubuntu-20-04)

* Install all the required ruby dependencies (gems) required by the SDK

```console
[root@citools ~]#bundle install
Fetching gem metadata from https://rubygems.org/.........
Resolving dependencies...
Using minitest 5.15.0
Using blankslate 3.1.3
Using multi_json 1.15.0
Using casper_network 0.2.0 from source at `.`
Using diff-lcs 1.5.0
Using unf_ext 0.0.8
Using http-accept 1.7.0
Using ipaddress 0.8.3
Using rack 2.2.3
Using unf 0.1.4
Using mime-types-data 3.2022.0105
Using resolv 0.2.1
Using rspec-support 3.11.0
Using concurrent-ruby 1.1.9
Using rspec-core 3.11.0
Using rspec-expectations 3.11.0
Using rspec-mocks 3.11.0
Using domain_name 0.5.20190701
Using i18n 1.10.0
Using tzinfo 2.0.4
Using rspec 3.11.0
Using stringio 3.0.1
Using activesupport 7.0.2.2
Using http-cookie 1.0.4
Using netrc 0.11.0
Using psych 4.0.3
Using timeout 0.2.0
Using bundler 2.3.8
Using mime-types 3.4.1
Using rdoc 6.4.0
Using rest-client 2.1.0
Using jimson 0.13.0
Bundle complete! 9 Gemfile dependencies, 32 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
```

* Install and build casper_network0.2.0 gem from repository

``` console
[root@citools ~]#gem build casper_network.gemspec
  Successfully built RubyGem
  Name: casper_network
  Version: 0.2.0
  File: casper_network-0.2.0.gem
```

```console
[root@citools ~]#gem install casper_network-0.2.0.gem
Successfully installed casper_network-0.2.0
1 gem installed
```

```console
[root@citools ~]#gem build casper_network.gemspec
  Successfully built RubyGem
  Name: casper_network
  Version: 0.2.0
  File: casper_network-0.2.0.gem
````

## Overall Impression of usage testing
The documentation provides clear and sufficient instructions to build and install the ruby sdk bundle.
However, the documentation does not give details on the version of Ruby used to develop and test the SDK (the reviewer installed version 3.0.2 by default).
After building the project ,the reviewer was unable to run the code example provided in the repository main page (https://github.com/saitgulmez/casper-ruby-sdk/tree/milestone-2#usage-examples):

```console

ruby test.rb
/home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `initialize': Failed to open TCP connection to 5.161.68.4:7777 (Connection refused - connect(2) for "5.161.68.4" port 7777) (Errno::ECONNREFUSED)
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `open'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `block in connect'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:107:in `block in timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:117:in `timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:985:in `connect'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:970:in `do_start'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:959:in `start'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:727:in `transmit'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:163:in `execute'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:63:in `execute'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:52:in `send_single_request'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:29:in `process_call'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:178:in `method_missing'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/casper_network-0.2.0/lib/casper_network.rb:37:in `block in info_get_peers'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:107:in `block in timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `block in catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:123:in `timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/casper_network-0.2.0/lib/casper_network.rb:35:in `info_get_peers'
	from test.rb:9:in `<main>'
/home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `initialize': Connection refused - connect(2) for "5.161.68.4" port 7777 (Errno::ECONNREFUSED)
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `open'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:987:in `block in connect'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:107:in `block in timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:117:in `timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:985:in `connect'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:970:in `do_start'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/3.0.0/net/http.rb:959:in `start'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:727:in `transmit'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:163:in `execute'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/rest-client-2.1.0/lib/restclient/request.rb:63:in `execute'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:52:in `send_single_request'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:29:in `process_call'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/jimson-0.13.0/lib/jimson/client.rb:178:in `method_missing'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/casper_network-0.2.0/lib/casper_network.rb:37:in `block in info_get_peers'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:107:in `block in timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `block in catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:36:in `catch'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/timeout-0.2.0/lib/timeout.rb:123:in `timeout'
	from /home/user/.rbenv/versions/3.0.2/lib/ruby/gems/3.0.0/gems/casper_network-0.2.0/lib/casper_network.rb:35:in `info_get_peers'
	from test.rb:9:in `<main>'
```
The reviewer was then able to run the example after replacing the node address (5.161.68.4) used in the example . 

The reviewer recommands to correct the  code example for the next milestones.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS 
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has 57 tests. The reviewer checked that all the RPC calls have at least one positive path test.

````Java
...
 # **********************************************************************************************
  # Test state_get_dictionary_item(state_root_hash, item_key, uref)
  describe "#state_get_dictionary_item" do
    stored_value = client.state_get_dictionary_item("146b860f82359ced6e801cbad31015b5a9f9eb147ab2a449fd5cdb950e961ca8",
      "abc_name",
      "uref-30074a46a79b2d80cff437594d2422383f6c754de453b732448cc711b9f7e129-007")
    stored_value.deep_symbolize_keys!
    it "checks that CLValue should not be nil" do
      expect(stored_value[:CLValue]).to be_truthy
    end

    it "checks that cl_type should equal to String" do
      expect(stored_value[:CLValue][:cl_type]).to eql("String")
    end

    it "checks that CLValue parsed equals to \"abc_value\"" do
      expect(stored_value[:CLValue][:parsed]).to eql("abc_value")
    end
  end

````

However, the reviewer had  observed that the tests run without a logging utility that would allow to see the actual progress of the tests. 
The tests run successfully, without errors and produce the following output:

```console 
rspec  spec/testnet_spec.rb
.........................................................

Finished in 0.03654 seconds (files took 1.13 seconds to load)
57 examples, 0 failures
```

The reviewer was able to check the presence of some negative path tests:

```Java
...
 context "When info_get_deploy is called with an empty deploy hash parameter" do
      deploy = client.info_get_deploy("")
      it "passes,  ServerError: Invalid params " do
        err = "Server error -32602: Invalid params (Jimson::Client::Error::ServerError)"
        expect {raise StandardError, err}.
        to raise_error(err)
      end
    end
```
The reviewer encourages the OP to add more of these negative path tests.


Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS with Notes
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

The code is documented in a very minimalist way, only a few classes and functions are provided with code-level documentation.
Since the project is in its early stage and does not contain much code yet, the reviewer strongly recommends documenting the SDK code.

Requirement | Finding
------------ | -------------
Code Documented | PASS with notes

### Project Documentation
The project does not provide detailed SDK documentation. The sample code provided in the Readme does not work and needs to be changed.
The only documentation available is the one the user can generate with the commands provided in the README file.
The reviewer was able to generate and view this documentation on this link: https://htmlpreview.github.io/?https://raw.githubusercontent.com/saitgulmez/casper-ruby-sdk/milestone-2/doc/index. html
There is no step-by-step guide on how to write ruby code using the SDK.
It is strongly recommended to add a well-supplied and detailed documentation for the next milestones.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes


## Overall Conclusion on Documentation

Based on the reviewer's findings, this review should pass with notes.

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

## General Observations

Code's structure and readability is acceptable for this milestone, but code documentation and SDK documentation are expected to be improved before the completion of the project.


# Final Conclusion

The project provides the functionality described in the grant application and milestone acceptance criteria.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
