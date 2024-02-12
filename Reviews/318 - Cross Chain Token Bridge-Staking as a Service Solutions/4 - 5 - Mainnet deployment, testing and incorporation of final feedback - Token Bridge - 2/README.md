
Grant Proposal | [318 - Cross Chain Token Bridge-Staking as a Service Solutions](https://portal.devxdao.com/public-proposals/318)
------------ | -------------
Milestone | 4:5
Milestone Title | Mainnet deployment, testing and incorporation of final feedback - Token Bridge & Incorporate audit feedback and launch - Token Bridge
OP | nickodio_ferrum
Reviewer | David Tai

# Milestone Details

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

### Milestone 4

- Deploy bridge on mainnet 
- Incorporate audit feedback if audit is completed 
- Conduct internal testing 
- Share the bridge with DEVxDAO and incorporate the final feedback

### Milestone 5 

- Incorporate final audit feedback provided by a third party 
- Launching the bridge on production mainnet

**Acceptance criteria:**

### Milestone 4

- Ability to conduct swaps across below networks with Casper:
1. Casper <> Ethereum
2. Casper <> BSC
3. Casper <> Polygon

- Able to add/remove liquidity on all networks 

- DEVxDAO signs off on mainnet testing

### Milestone 5 

- Sign-off on audit completion by the third party auditor 
- Launch on production mainnet 
- Bridge is live and available to users to bridge token

**Additional notes regarding submission from OP:**

### Milestone 4

Mainnet deployment, testing and incorporation of final feedback - Token Bridge

Details of what will be delivered in milestone

- Deploy bridge on mainnet - Incorporate audit feedback if audit is completed - Conduct internal testing - Share the bridge with DEVxDAO and incorporate the final feedback

Acceptance criteria: Please enter the specific details on what the deliverable must do to prove this milestone is complete.

-Ability to conduct swaps across below networks with Casper: 1. Casper <> Ethereum 2. Casper <> BSC 3. Casper <> Polygon - Able to add/remove liquidity on all networks - DEVxDAO signs off on mainnet testing

### Milestone 5 

Incorporate audit feedback and launch - Token Bridge

Details of what will be delivered in milestone

- Incorporate final audit feedback provided by a third party - Launching the bridge on production mainnet

Acceptance criteria: Please enter the specific details on what the deliverable must do to prove this milestone is complete.

- Sign-off on audit completion by the third party auditor - Launch on production mainnet - Bridge is live and available to users to bridge token

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Milestone #4 and 5 OP Submission Notes: Below are the final testing links, links to relevant repos, and audit report. 

Testing url - https://casper-mainnet-bridge.netlify.app/

Bridge client-side repository : https://github.com/ferrumnet/casper-bridge-frontend

Bridge contract repository: https://github.com/ferrumnet/bridge-casper-smart-contracts

Repository | Revision Reviewed
------------ | -------------
https://github.com/ferrumnet/bridge-casper-smart-contracts | [5f445f3]
https://github.com/ferrumnet/casper-bridge-frontend | [27d3b33]

# Install & Usage Testing Procedure and Findings

Repos were initially missing both Security.md and Contributing.md.  These were added after the reviewer gave the team initial feedback.  The smart contracts repo built easily and the tests were able to pass:

```
cd contract && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 1.24s
cd counter-call && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.11s
cd erc20/erc20-token && cargo build --release --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.12s
wasm-strip contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm 2>/dev/null | true
wasm-strip counter-call/target/wasm32-unknown-unknown/release/counter-call.wasm 2>/dev/null | true
mkdir -p tests/wasm
cp contract/target/wasm32-unknown-unknown/release/bridge_pool.wasm tests/wasm
cp counter-call/target/wasm32-unknown-unknown/release/counter-call.wasm tests/wasm
cp erc20/target/wasm32-unknown-unknown/release/erc20_token.wasm tests/wasm/erc20.wasm
cd tests && cargo test
    Finished test [unoptimized + debuginfo] target(s) in 0.67s
     Running unittests src/integration_tests.rs (target/debug/deps/integration_tests-efdfaed98dceb0bc)

running 8 tests
test tests::should_be_able_to_install_and_allow_target ... ok
test tests::should_be_able_to_install_and_add_signer ... ok
test tests::should_be_able_to_install_and_add_liquidity ... ok
test tests::should_be_able_to_install_add_and_remove_signer ... ok
test tests::should_be_able_to_install_and_get_liquidity ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_remove_liquidity ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_swap ... ok
test tests::should_be_able_to_install_and_add_liquidity_and_withdraw_signed ... ok

test result: ok. 8 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 5.43s
```

The front end repo had various problems due to lack of pinned library versions in the package.json.  Even after getting the project to build, the reviewer could never quite get the tests to work even though manual testing the UI worked.

```
npm run test

> my-app@0.1.0 test
> jest --collectCoverage=false --silent

 FAIL  tests/CasperToBsc.test.tsx
  ● Test suite failed to run

    src/Routes.tsx:13:10 - error TS2786: 'Switch' cannot be used as a JSX component.
      Its instance type 'Switch' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.
            Type '{}' is not assignable to type 'ReactNode'.

    13         <Switch>
                ~~~~~~
    src/Routes.tsx:14:12 - error TS2786: 'Route' cannot be used as a JSX component.
      Its instance type 'Route<{}, "/withdraw">' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.

    14           <Route path="/withdraw" component={() => (
                  ~~~~~
    src/Routes.tsx:19:12 - error TS2786: 'Route' cannot be used as a JSX component.
      Its instance type 'Route<{}, "*">' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.

    19           <Route path="*" component={() =>
                  ~~~~~

 FAIL  tests/BscToCasper.test.tsx
  ● Test suite failed to run

    src/Routes.tsx:13:10 - error TS2786: 'Switch' cannot be used as a JSX component.
      Its instance type 'Switch' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.
            Type '{}' is not assignable to type 'ReactNode'.

    13         <Switch>
                ~~~~~~
    src/Routes.tsx:14:12 - error TS2786: 'Route' cannot be used as a JSX component.
      Its instance type 'Route<{}, "/withdraw">' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.

    14           <Route path="/withdraw" component={() => (
                  ~~~~~
    src/Routes.tsx:19:12 - error TS2786: 'Route' cannot be used as a JSX component.
      Its instance type 'Route<{}, "*">' is not a valid JSX element.
        The types returned by 'render()' are incompatible between these types.
          Type 'React.ReactNode' is not assignable to type 'import("/home/dtai/projects/node_modules/@types/react/index").ReactNode'.

    19           <Route path="*" component={() =>
                  ~~~~~

Test Suites: 2 failed, 2 total
Tests:       0 total
Snapshots:   0 total
Time:        4.104 s
```

The audit is attached with this review as `Ferrum Network (Casper Bridge) (Jul 10, 2023).pdf`.

## Overall Impression of usage testing

The project can be built by following hte instructions.  The project is functional but only at a proof of concept and not ready for mainnet launch including uncontrolled calls to the back end apis from the website instead of having a separate, secure listener.  The website is clearly not production ready per milestone 5.  It is missing many features, security, and the polish required for end users.  It also only supports the ferrum test token.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | FAIL - UX automated testing does not pass and Milestone 5 "Bridge is live and available to users to bridge token" is not delivered.

# Unit / Automated Testing

Repo [https://github.com/ferrumnet/bridge-casper-smart-contracts](https://github.com/ferrumnet/bridge-casper-smart-contracts):

This repository works and passes tests.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS 
Unit Tests - Additional path tests | PASS

Repo [https://github.com/ferrumnet/bridge-casper-smart-contracts](https://github.com/ferrumnet/casper-bridge-frontend):

This repository seems to work and but the tests do not seem to build outside of the developer's local environment.

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | FAIL
Unit Tests - At least one negative path test | FAIL 
Unit Tests - Additional path tests | FAIL

# Documentation

### Code Documentation

The project has sufficient code-level documentation and the critical classes and methods have comments but it can be improved.

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

The smart contract repo had an extraneous `cargo doc` comment in the README.md that did not do anything.  This has been removed.  Code level documentation while minimal was sufficient to understand the contracts. The repo had examples of commands and results. 

The website repo is a self expanitory create react app.  There was not a huge amount of documentation but anyone with experience with react should be able to understand.

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation

Documentation is minimal but sufficient

# Open Source Practices

## Licenses

The Project is released under the MIT License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Contributing policies were added.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Final Conclusion

The project while improved from the last review while technically sufficient except for the failing front-end test does not fulfill the delivery criteria of having a production ready product useable by end users.  Upon clarification with the grant givers that this was a hard requirement, the decision was to fail this milestone due to this.

# Recommendation

Recommendation | FAIL
------------ | -----------
