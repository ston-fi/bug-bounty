<h1 align="center">STON.FI Bug Bounty program</h1>

<p align="center">
    <img src="https://github.com/ston-fi/bug-bounty/blob/main/Banner.jpg" width="100%">
</p>

The STON.fi Bug Bounty program is focused around our smart contracts with a primary interest in the prevention of loss of user funds.

<h3> Program fund is 200 000 TON. </h3>

<h2 align="center">Rewards</h2>

<table align="center" width="100%">
  <tr align="center">
    <th width="400px">Level of vulnerability</th>
    <th width="400px">Amount</th>
  </tr>
  <tr align="center">
    <td>Critical</td>
    <td>Up to 20.000 TON</td>
  </tr>
  <tr align="center">
    <td>High</td>
    <td>2.000 TON</td>
  </tr>
  <tr align="center">
    <td>Medium</td>
    <td>1.000 TON</td>
  </tr>
</table>

These rewards may be increased in the future.

<h2 align="center">Smart Contracts</h2>

Currently the scope of program only includes contracts v1.0.0, the same ones that are used by DEX in the mainnet.
The scope might be extended with other versions in the future.

<table align="center" width="100%">
  <tr align="center">
    <th width="200px">Name of Contract</th>
    <th width="600px">Link</th>
  </tr>
  <tr align="left">
    <td>LP Account</td>
    <td>https://github.com/ston-fi/dex-core/blob/v1.0.0/contracts/lp_account.func</td>
  </tr>
  <tr align="left">
    <td>LP Wallet</td>
    <td>https://github.com/ston-fi/dex-core/blob/v1.0.0/contracts/lp_wallet.func</td>
  </tr>
  <tr align="left">
    <td>Pool</td>
    <td>https://github.com/ston-fi/dex-core/blob/v1.0.0/contracts/pool.func</td>
  </tr>
  <tr align="left">
    <td>Router</td>
    <td>https://github.com/ston-fi/dex-core/blob/v1.0.0/contracts/router.func</td>
  </tr>
</table>

The contracts version may be updated in the future.

<h2 align="center">Impacts in scope</h2>

Only the following impacts are accepted within this Bug Bounty program. All other impacts are not considered as in-scope, even if they affect something in the assets in scope table.

<table align="center" width="100%">
  <tr align="center">
    <th width="600px">Type</th>
    <th width="200px">Level</th>
  </tr>
  <tr>
    <td align="left">Direct theft of any user funds</td>
    <td align="center">Critical</td>
  </tr>
  <tr>
    <td align="left">Permanent freezing of funds</td>
    <td align="center">Critical</td>
  </tr>
  <tr>
    <td align="left">Protocol insolvency</td>
    <td align="center">Critical</td>
  </tr>
  <tr>
    <td align="left">Theft of unclaimed yield</td>
    <td align="center">High</td>
  </tr>
  <tr>
    <td align="left">Freeze ability of other users to trade</td>
    <td align="center">High</td>
  </tr>
  <tr>
    <td align="left">Temporary freezing of funds</td>
    <td align="center">High</td>
  </tr>
  <tr>
    <td align="left">Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)</td>
    <td align="center">Medium</td>
  </tr>
</table>

<h2 align="center">Rules</h2>

The following activities are prohibited by this Bug Bounty program:

- Any testing with mainnet.
- Any testing with pricing oracles or third party Smart Contracts
- Attempting phishing or other social engineering attacks against our employees and/or customers
- Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)
- Automated testing of services that generates significant amounts of traffic
- Any denial of service attacks

All testing should be done on testnet.
We specifically deployed smart contracts on the testnet.

Router address - `EQBsGx9ArADUrREB34W-ghgsCgBShvfUr4Jvlu-0KGc33Rbt`. Also you can see on [tonscan](https://testnet.tonscan.org/address/EQBsGx9ArADUrREB34W-ghgsCgBShvfUr4Jvlu-0KGc33Rbt).

And please see dex-core [repo](https://github.com/ston-fi/dex-core).

<h2 align="center">Non-issues</h2>

The following issues are excluded from the rewards for this Bug Bounty program:

- Lack of liquidity
- Best practice critiques
- Centralization risks
- Issues with information about user balances
- Cases with disguising one asset with another asset
- Issues with precision when providing liquidity: e.g. in certain case, if you provide liquidity and after that you directly burn it, you may receive a bit less of one jetton and a bit more of the other one
- Any kind of optimization/logic improvements/coding style improvements
- Wrong opcode in onchain getter call getter_lp_account_address (in 1.0.0 version)
- Issues related to lp jetton wallets
- Issues related to contract deletion caused by inability to pay rent
- Issues related to gas optimisation
- Issues related to loss of funds caused by price slippage: frontrunning, backrunning, sandwich attacks, etc.
- Possible loss of funds when attempting to perform a swap in non-initialized pool (before successful provideLP)

<h2 align="center">Experts</h2>

Experts involved in the evaluation of the reports:

- [Vyacheslav Baranov](https://github.com/SlavikBaranov) (STON.fi team)
- [Dario Tarantini](https://github.com/dariotarantini) (STON.fi team)
- [Narek Abovyan](https://github.com/Naltox) (Head of TonTech)
- [krigga](https://github.com/krigga) (TonTech developer)

<h2 align="center">Reports</h2>

All bug reports must include a Proof of Concept demonstrating how the vulnerability can be exploited to be eligible for a reward. This may be a Smart Contract itself or a transaction.
Only the reports that meet the requirements will be considered by the experts.

Please send reports to security@ston.fi

By submitting a vulnerability report you indicate your agreement to the [Terms of participation](https://github.com/ston-fi/bug-bounty/blob/main/Terms_of_participation.md).